<script>
  import Step2 from "../../components/Step2.svelte";
  import mushroom from "$lib/mushroom.jpg";
  import spaghetti from "$lib/spaghetti.jpg";
  import bread from "$lib/bread.jpg";
  import saladItalian from "$lib/italian_salad.jpg";
  import pie from "$lib/pie.jpg";
  import cauliflower from "$lib/cauliflower.jpg";

  let r = [
    {
      name: "Grilled Chimichurri Portobellos with Goat Cheese Mashed Potatoes",
      description:
        "These Grilled Chimichurri Portobellos are OUT OF THIS WORLD. Marinated in a punchy and vibrant chimichurri before heading to the grill, then served on top of a mountain of creamy goat cheese mashed potatoes.",
      src: mushroom,
      link: "/summer/mushroom",
    },
    {
      name: "Spaghetti with Crispy Zucchini",
      description:
        "This Spaghetti with Crispy Zucchini is the perfect end-of-summer song! It doesn’t get much better than fresh summer zucchini coated in a crispy, cheesy breading piled high on top of spaghetti with fresh herbs. YUM!",
      src: spaghetti,
    },
    {
      name: "yummy italian salad",
      description: "the best choco chip cookies you'll ever have",
      src: saladItalian,
    },

  ];
</script>

<main class="bg-grey-100">
  <div class="bg-purple-900 mt-5">
    <header
      class="pt-3 pb-12 px-4 md:pt-5 md:pb-28 md:px-2 md:max-w-4xl mx-auto text-center"
    >
      <h1
        class="text-center text-white text-5xl md:text-6xl mb-4 md:mb-8 domine"
      >
        Summer Recipes
      </h1>
      <p class="my-0 text-purple-100 md:text-2xl lg:mr-4 eb-garamond">
        Looking for just the right thing to make for a backyard grill party? Or
        maybe your CSA has been bountiful but your recipe ideas...well, less so.
        Here, let us help! Some of our favorite recipes to cook up and enjoy
        while covered in sunshine and summertime.
      </p>
    </header>
  </div>

  <div
    class="recipes py-20 lg:py-32 flex flex-col gap-24 grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10"
  >
    <Step2 step={r[0]}></Step2>
    <Step2 step={r[1]}></Step2>

  </div>
</main>
