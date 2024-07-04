<!-- <script>
  import image from "$lib/search.png"
</script>

<main class="bg-grey-100">
  <div class="bg-purple-900 mt-5">
    <header class="pt-3 pb-12 px-4 md:pt-5 md:pb-28 md:px-2 md:max-w-4xl mx-auto text-center">
      <h1 class="text-center text-white text-5xl md:text-6xl mb-4 md:mb-8 domine">
        Recipes
      </h1>
      <p class="my-0 text-purple-100 md:text-2xl lg:mr-4 eb-garamond">
        We’ve organized these recipes every way we could think of so you don't
        have to! Dietary restrictions, weeknight dinners, meal prep recipes, some
        of our most tried-and-true… no matter how you browse, we’re sure you’ll
        find just what you were looking for.
      </p>
    </header>
  </div>

  <div class="search-wrapper absolute left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-white shadow-lg rounded-lg py-2 px-4 mt-4" >
    <input type="search" id="search" class="w-full border-gray-300 focus:border-violet-500 focus:ring focus:ring-violet-500 focus:ring-opacity-50 rounded-md py-2 px-4" placeholder="Search By Keyword"/>
    <i class="fa-solid fa-magnifying-glass mr-2 text-gray-400"></i>

  </div>
</main>


<style>

</style> -->

<script>

  import Step2 from "../../components/Step2.svelte";
  import cookie from "$lib/cookies.jpg";
  import pancake from "$lib/pancake.jpg";
  import bread from "$lib/bread.jpg";
  import saladItalian from "$lib/italian_salad.jpg";
  import pie from "$lib/pie.jpg";
  import cauliflower from "$lib/cauliflower.jpg";

  let r = [
    {
      name: "chocolate chip cookies",
      description: "the best choco chip cookies you'll ever have",
      src: cookie,
      link: "/recipes/cookies"
      
    },
    {
      name: "miracle bread",
      description: "no knead bread!",
      src: bread
    },
    {
      name: "blueberry pancakes",
      description: "the fluffiest pancakes ever!",
      src: pancake
    },
    {
      name: "yummy italian salad",
      description: "fresh italian salad with herbs tossed with croutons, tomatoes and lettuce!",
      src: saladItalian
    },
    {
      name: "vegetarian shepherd's pie",
      description: "the best sheperd's pie loaded with veggies and savory lentils and topped with fluffy mashed potatoes",
      src: pie
    },
    {
      name: "Roasted Cauliflower Hummus Bowls",
      description: "These Roasted Cauliflower Hummus Bowls are LIFE-CHANGING. A bed of garlicky creamy hummus, piled high with spiced roasted cauliflower, and a speckling of fresh lemony tomatoes and herbs.",
      src: cauliflower
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
        Recipes
      </h1>
      <p class="my-0 text-purple-100 md:text-2xl lg:mr-4 eb-garamond">
        We’ve organized these recipes every way we could think of so you don't
        have to! Dietary restrictions, weeknight dinners, meal prep recipes,
        some of our most tried-and-true… no matter how you browse, we’re sure
        you’ll find just what you were looking for.
      </p>
    </header>
  </div>

  <!-- <div
    class="search-wrapper absolute left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-white shadow-lg rounded-lg py-2 px-4 mt-4"
  >
    <input
      type="search"
      id="search"
      class="montserrat w-full border-gray-300 focus:border-violet-500 focus:ring focus:ring-violet-500 focus:ring-opacity-50 rounded-md py-2 px-4"
      placeholder="Search By Keyword"
      data-search
    /> -->
  <!-- <i class="fa-solid fa-magnifying-glass mr-2 text-gray-400 ml-4"></i> -->
  <!-- </div>
  <div class="user-cards"></div>
  <template data-user-template>
    <div class="card">
      <div class="header"></div>
      <div class="body"></div>
    </div>
  </template> -->

  <div class="recipes py-20 lg:py-32 flex flex-col gap-24 grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
    <Step2 step={r[0]}>

    </Step2>
    <Step2 step={r[1]}>

    </Step2>
    <Step2 step={r[2]}>

    </Step2>
    <Step2 step={r[3]}>

    </Step2>
    <Step2 step={r[4]}>

    </Step2>
    <Step2 step={r[5]}>

    </Step2>

  </div>
</main>

<style>
  .search-wrapper {
    display: flex;
    align-items: center;
    flex-direction: column;
    gap: 0.25rem;
  }

  input {
    font-size: 1rem;
  }

  .user-cards {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
    gap: 0.25rem;
    margin-top: 1rem;
  }

  .card {
    background-color: transparent;
    border-radius: 0.5rem;
    overflow: hidden;
  }

  .card > .header {
    margin-bottom: 0.25rem;
    background-color: #f0f0f0;
  }

  .card > .body {
    font-size: 0.8rem;
    color: #777;
    padding: 0.5rem;
  }

  .hide {
    display: none;
  }
</style>
