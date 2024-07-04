<script>
  import cookie from "$lib/mushroom.jpg";
</script>

<main>
  <div class="bg-purple-900 mt-5 rounded-lg">
    <header
      class="pt-3 pb-12 px-4 md:pt-5 md:pb-18 md:px-2 md:max-w-4xl mx-auto text-center"
    >
      <!-- <div
        class="relative overflow-hidden rounded-full border border-violet-700 md:h-80 md:w-80 sm:w-40 sm:h-40 mt-5 mb-5 lg:ml-64 ml-76"
      >
        <div
          class="absolute inset-0 bg-slate-950 bg-opacity-75 flex items-center justify-center opacity-0 md:h-80 md:w-80 sm:w-40 sm:h-40 mt-5 mb-5"
        >
        </div>
        <img src={cookie} alt="cookie" class="rounded-full aspect-ratio md:h-80 md:w-80 sm:w-40 sm:h-40 object-cover " />
      </div> -->
      <div class="flex justify-center">
        <img
          src={cookie}
          alt="cookie"
          class="rounded-full border border-violet-700 md:h-40 md:w-40 sm:h-25 sm:w-25 lg:w-40 lg:h-40 h-40 w-40 mt-4 mb-6"
        />
      </div>
      <h1
        class="text-center text-white text-5xl md:text-6xl mb-4 md:mb-8 domine"
      >
        Grilled Chimichurri Portobellos with Goat Cheese Mashed Potatoes
      </h1>
      <p class="my-0 text-purple-100 md:text-2xl lg:mr-4 eb-garamond">
        These Grilled Chimichurri Portobellos are OUT OF THIS WORLD. Marinated
        in a punchy and vibrant chimichurri before heading to the grill, then
        served on top of a mountain of creamy goat cheese mashed potatoes.
      </p>

      <div class="flex justify-center mt-4 mb-4 gap-2">
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
      </div>

      <p class="para eb-garamond text-white">5 from 44 reviews</p>

      <div class="flex justify-center gap-10 mt-4 text-lg">
        <div class="flex items-center gap-3">
          <i class="fa-solid fa-clock"></i>
          <p class="domine"><strong>TOTAL TIME</strong>: 45 minutes</p>
        </div>

        <div class="flex items-center gap-3">
          <i class="fa-solid fa-utensils"></i>
          <p class="domine"><strong>YIELD</strong>: 4</p>
        </div>
      </div>
    </header>
  </div>

  <div class="border border-violet-900 rounded-lg">
    <h1 class="cutive2 mt-4 mb-4">
      Grilled mushrooms CAN be the star of your grill this summer, and not just
      for vegetarians or vegans, in case you were wondering. This meatless meal
      is a real beauty. Portobellos get a nice soak in quick, vibrant, and very
      punchy chimichurri before heading to the grill, where they become both
      tender and flavorful and kind of meaty in a mushroom way. Those grill
      marks, I’m telling you.
    </h1>
    <hr class="border-violet-900" />

    <h1 class="domine mt-5 font-bold text-xl ml-2">INGREDIENTS</h1>

    <h4 class="domine mt-5 font-bold text-lg ml-2">
      Cilantro Chimichurri and Mushrooms
    </h4>

    <div class="mt-4 ml-2">
      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >1/2 cup of <strong class="eb-garamond">olive oil</strong></label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >2 tablespoons <strong class="eb-garamond">red wine vinegar</strong
          ></label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >1/2 cup finely chopped <strong class="eb-garamond">cilantro</strong>
          <span class="ita eb-garamond">(not traditional)</span>
          or <strong class="eb-garamond">parsley</strong>
          <span class="ita eb-garamond">(traditional)</span></label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >1 teaspoon <strong class="eb-garamond">vanilla</strong></label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >1 small <strong class="eb-garamond">red serrano pepper</strong>,
          minced</label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >3 cloves <strong class="eb-garamond">garlic</strong>, minced</label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >1 teaspoon <strong class="eb-garamond">oregano</strong></label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >1 teaspoon <strong class="eb-garamond">kosher salt</strong></label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          ><strong class="eb-garamond">red pepper flakes</strong> to taste</label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >4 <strong class="eb-garamond">portobello mushroom caps</strong
          ></label
        >
      </div>

      <h4 class="domine mt-5 font-bold text-lg ml-2 ">Mashed Potatoes</h4>

      <div class="flex items-center mb-3 gap-1 mt-4">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >2 large <strong class="eb-garamond">russet potatoes</strong
          ></label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >4 tablespoons<strong class="eb-garamond">butter</strong
          ></label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >4 ounces <strong class="eb-garamond">goat cheese</strong
          ></label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >1/2 - 1 cup <strong class="eb-garamond">chicken or vegetable broth</strong
          ></label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >1 clove <strong class="eb-garamond">garlic</strong
          >, grated</label
        >
      </div>

      <div class="flex items-center mb-3 gap-1">
        <input type="checkbox" />
        <span class="checkmark"></span>
        <label class="container eb-garamond text-lg"
          >1 teaspoon <strong class="eb-garamond">salt</strong
          ></label
        >
      </div>

      <hr class="border-violet-900" />

      <h1 class="domine mt-5 font-bold text-lg mb-4 p-3">INSTRUCTIONS</h1>

      <ol class="list-decimal pl-4">
        <div class="p-3">
          <li class="domine list-item">
            <strong class="domine">Chimichurri</strong>: Mix sauce ingredients
            (olive oil through red pepper flakes) together in a small dish.
          </li>
          <div class="flex justify-center">
            <iframe
              loading="lazy"
              class="fitvidsignore"
              title="Grilled Chimichurri Portobellos with Goat Cheese Mashed Potatoes Step 1"
              src="https://player.vimeo.com/video/449359177?dnt=1&amp;app_id=122963&amp;autoplay=0&amp;muted=1&amp;autopause=0&amp;loop=1&amp;controls=1"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
            ></iframe>
          </div>

          <li class=" domine list-item">
            <strong class="domine">Potatoes</strong>: Cut potatoes into quarters
            and boil for 10-15 minutes until very soft. Drain and pull the skins
            off. Mash and mix with broth, butter, goat cheese, garlic, and salt.
          </li>
          <div class="flex justify-center">
            <iframe
              loading="lazy"
              class="fitvidsignore"
              title="Grilled Chimichurri Portobellos with Goat Cheese Mashed Potatoes Step 2"
              src="https://player.vimeo.com/video/449359518?dnt=1&amp;app_id=122963&amp;autoplay=0&amp;muted=1&amp;autopause=0&amp;loop=1&amp;controls=1"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
            ></iframe>
          </div>

          <li class="domine list-item">
            <strong class="domine">Marinade</strong>: While potatoes are
            cooking, brush mushrooms with a little bit of chimichurri on both
            sides. Marinate for 15-30 minutes.
          </li>

          <div class="flex justify-center">
            <iframe
              loading="lazy"
              class="fitvidsignore"
              title="Grilled Chimichurri Portobellos with Goat Cheese Potatoes Step 4"
              src="https://player.vimeo.com/video/449360271?dnt=1&amp;app_id=122963&amp;autoplay=0&amp;muted=1&amp;autopause=0&amp;loop=1&amp;controls=1"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
            ></iframe>
          </div>

          <li class=" domine list-item">
            <strong class="domine">Mushrooms</strong>: Heat a grill pan or grill
            over medium high heat. Add mushrooms and grill on both sides,
            brushing with more chimichurri, until soft and yummy and browned up
            with nice grill marks.
          </li>

          <div class="flex justify-center">
            <iframe
              loading="lazy"
              class="fitvidsignore"
              title="Grilled Chimichurri Portobellos with Goat Cheese Mashed Potatoes Step 5"
              src="https://player.vimeo.com/video/449360660?dnt=1&amp;app_id=122963&amp;autoplay=0&amp;muted=1&amp;autopause=0&amp;loop=1&amp;controls=1"
              frameborder="0"
              allow="autoplay; fullscreen; picture-in-picture; clipboard-write"
            ></iframe>
          </div>

          <li class="domine list-item">
            <strong class="domine">Done</strong>: Serve up a mushroom steak on a dollop of creamy potatoes and –
            you guessed it – spoon the last of your chimichurri over the top.
            Salt, pepper, red pepper flake it… and you’re good to go!
          </li>
        </div>
      </ol>
    </div>
  </div>
</main>

<style>
  .ita {
    font-style: italic;
  }

  .checked {
    color: orange;
  }

  .para {
    font-style: italic;
  }

  .cutive2 {
    font-size: medium;
    text-align: center;
  }

  .list-item {
    text-align: left; /* Ensure content aligns to the left */
    margin-bottom: 10px;
  }

  hr {
    margin-left: 2rem;
    margin-right: 2rem;
  }

  .fitvidsignore {
    width: 100%;
    height: 400px;
    border-radius: 12px;
    margin-top: 2px;
    margin-bottom: 5px;
  }
</style>
