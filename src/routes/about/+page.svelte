<script>
  import profile from "$lib/woman.jpg";
</script>

<!-- <main class="flex justify-center items-center min-h-screen bg-gray-100">
  <div class="flex flex-col gap-4 w-full md:w-1/2">
    <img src="src\lib\woman.jpg" class="rounded-full mx-auto w-82 h-82 object-cover"/>
  </div>

  <div class="text-center md:text-left">
    <h1>About Me</h1>
  </div>


</main> -->

<main class="flex flex-col items-center justify-center flex-1 p-4">
  <section
    id="aboutMe"
    class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
  >
    <div class="relative grid place-items-center lg:justify-items-start">
      <img
        src={profile}
        class="object-cover z-[2] max-h-[70vh] rounded-full w-[300px] lg:w-[400px] shadow-lg"
        alt="profileImg"
      />
    </div>
    <div
      class="flex flex-col justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
    >
      <h2
        class="cutive font-semibold text-2xl sm:text-3xl md:text-4xl text-purple-800"
      >
        About Me
      </h2>
      <p
        class="montserrat text-base text-lg sm:text-xl md:text-2xl lg:text-3xl"
      >
        Hi! My name is <span class="custom playwrite">Lindsay</span>!
      </p>
      <p class="montserrat text-base sm:text-xl md:text-2xl lg:text-2xl gap-4">
        And Pinch of Salt is my little corner of the internet. I'm the voice,
        author and creator behind Pinch of Salt.
      </p>
      <p class="montserrat text-base sm:text-xl md:text-2xl lg:text-2xl gap-4">
        What started as a hobby over a decade ago while I was still pursuing my
        higher education has now grown into a full-blown business (!) that
        reaches millions of people with fun recipes, with content that has been
        featured on The Kitchn, CNN, Refinery29, Brit + Co, POPSUGAR, Huffington
        Post, The Everymom, PureWow, and more.
      </p>
      <p class="montserrat text-base sm:text-xl md:text-2xl lg:text-2xl">
        I live in Los Angeles, with my dog Henry. My favorite things in life are
        food, reading and going to beaches.
      </p>
    </div>
  </section>

</main>

<style>
  .custom {
    font-style: italic;
  }
</style>
