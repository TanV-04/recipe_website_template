<script>
  import Step from "./Step.svelte";
  import image from "$lib/pastaSaladBowl.jpg";
  import summerImg from "$lib/summerBowl.jpg";
  import dessertImg from "$lib/brownie.jpg";
  import sbowl from "$lib/saladBowl3.jpg";
  import snack from "$lib/snackie.jpg";
  let steps = [
    { name: "Summer", src: summerImg, href: "/summer"},
    { name: "Salads", src: sbowl},
    { name: "Desserts", src: dessertImg},
    { name: "Snacks", src: snack},
  ];
</script>

<main class="flex flex-col items-center justify-center flex-1 p-4">
  <section
    id="introPage"
    class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
  >
    <div
      class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
    >
      <h2 class="cutive font-semibold text-2xl sm:text-3xl md:text-4xl">
        SIMPLE RECIPES MADE FOR
      </h2>
      <p class="comfort text-base text-5xl sm:text-6xl md:text-6xl">
        real. actual. everyday. life.
      </p>

      <div class="flex items-center justify-center">
        <p
          class="cookie px-6 py-3 rounded-full beige text-slate-950 font-medium text-lg sm:text-xl md:text-2xl lg:text-3xl mt-4"
        >
          Scroll for More! &darr;
        </p>
      </div>
    </div>
    <div class="relative shadow-2xl grid place-items-center">
      <img
        src={image}
        alt="pasta bowl"
        class="object-cover z-[2] max-h-[70vh]"
      />
    </div>
  </section>

  <div
    id="more"
    class="py-20 lg:py-32 flex flex-col gap-24 grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10"
  >
    <Step step={steps[0]}>

    </Step>
    <Step step={steps[1]}>

    </Step>
    <Step step={steps[2]}>

    </Step>
  </div>
</main>

<style>
  .beige {
    background-color: #52482d;
    color: rgb(238, 235, 229);
  }
</style>
