<script>
  import profile from "$lib/rigatoni.jpg";
  import emailjs from "emailjs-com";

  emailjs.init("YU1cDrC3r9VPzI4Xm")

  function validateInput(input) {
    const value = input.value.trim();
    let isValid = true;

    if (input.name === "firstName") {
      if (value === "") {
        alert("Please enter your first name");
        isValid = false;
      }
    } else if (input.name === "email") {
      const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
      if (!emailRegex.test(value)) {
        alert("Please enter a valid email address");
        isValid = false;
      }
    }
    return isValid;
  }

  function handleSubmit(event) {
    event.preventDefault();

    const firstNameInput = document.getElementById("firstNameInput");
    const emailInput = document.getElementById("emailInput");

    if (!validateInput(firstNameInput) || !validateInput(emailInput)) {
      return false;
    }

    const params = {
      name: firstNameInput.value,
      email: emailInput.value
    };

    const serviceID = "service_a0jei7p";
    const templateID = "template_56muxtj";

    emailjs.send(serviceID, templateID, params)
      .then((res) => {
        alert("Message sent successfully!");
        console.log(res);
        firstNameInput.value = "";
        emailInput.value = "";
      })
      .catch((err) => {
        console.error("Error sending email:", err);
        alert("Failed to send message. Please try again later.");
      });
    
      console.log("button is clicked.")
  }
</script>

<main class="flex flex-col items-center justify-center flex-1 p-4">
  <section id="aboutMe" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
    <div class="relative grid place-items-center lg:justify-items-start">
      <img
        src={profile}
        class="object-cover z-[2] max-h-[70vh] rounded-lg w-[400px] lg:w-[500px] shadow-lg"
        alt="profileImg"
      />
    </div>
    <div class="flex flex-col justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
      <h2 class="cutive font-semibold text-2xl sm:text-3xl md:text-4xl text-purple-800">
        Welcome to Pinch of Salt
      </h2>
      <p class="montserrat text-base text-lg sm:text-xl md:text-2xl lg:text-3xl">
        Let's talk food, <span class="custom playwrite">shall we </span>?
      </p>
      <p class="montserrat text-base sm:text-xl md:text-2xl lg:text-2xl gap-4">
        Well, we hope that’s why you’re here. Our recipes are designed for real,
        actual, every day life, and we try to focus on real foods and healthy
        recipes (which honestly means a lot of different things to us, including
        the perfect chocolate chip cookie and cheese on cheese on cheese,
        because health is all about balance, right?).
      </p>
      <p class="montserrat text-base sm:text-xl md:text-2xl lg:text-2xl gap-4">
        This is the place to find those recipes — everything from our most
        popular, to meal prep, to Instant Pot recipes, or if you just, like,
        have some sad greens in your fridge to use up and you need some
        inspiration.
      </p>
      <p class="montserrat text-base sm:text-xl md:text-2xl lg:text-2xl">
        You’re here! Have fun. We hope you find something (many things) you
        love.
      </p>
    </div>
  </section>

  <div class="sign-up py-4 flex flex-col justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
    <p class="custom playwrite text-base text-lg sm:text-xl md:text-xl lg:text-2xl">
      Sign up <span class="cutive text-purple-600">FOR EMAIL UPDATES</span>
    </p>
    <div class="input-container flex flex-col sm:flex-row lg:flex-row gap-4">
      <input
        type="text"
        placeholder="First Name"
        class="py-3 px-3 rounded-lg shadow-lg border border-black"
        name="firstName"
        id="firstNameInput"
      />
      <input
        type="email"
        placeholder="Email"
        class="py-3 px-3 rounded-lg shadow-lg border border-black"
        name="email"
        id="emailInput"
      />
    </div>
    <button
      on:click={handleSubmit}
      type="submit"
      class="btn-orange px-4 py-2 rounded-md text-base font-medium text-center text-white bg-orange-400 hover:bg-orange-400 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-orange-500 mt-4"
    >
      GO
    </button>
  </div>
</main>
