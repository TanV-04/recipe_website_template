<script>
  export let y;

  export let tabs = [
    { name: "HOME", link: "/" }, // or #HOME or /#HOME
    { name: "ABOUT", link: "/about"},
    { name: "RECIPES", link: "/recipes" },
    { name: "START HERE", link: "/startHere" },
  ];

  let isOpen = false;

  function toggleMenu() {
    isOpen = !isOpen;
  }
</script>

<header
  class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border-b border-solid" +
    (y > 0
      ? " py-4 bg-slate-950 border-violet-450 text-white"
      : " py-6 bg-transparent border-transparent") +
    " lg:px-12 xl:px-24"}
>
  <h1
    class="font-medium text-2xl md:text-3xl cursor-pointer"
    on:click={() => window.scrollTo(0, 0)}
  >
    <span class="inconsolata font-bold">pinch</span>
    <span class="playwrite font-medium text-purple-900">of</span>
    <span class="inconsolata font-bold">salt</span>
  </h1>

  <!--hamburger menu-->

  <button
    class="block sm:hidden text-xl focus:outline-none"
    aria-label="Toggle Menu"
    on:click={toggleMenu}
  >
    <svg
      class="h-6 w-6"
      fill="none"
      stroke="currentColor"
      viewBox="0 0 24 24"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="2"
        d="M4 6h16M4 12h16m-7 6h7"
      ></path>
    </svg>
  </button>

  <!--mobile menu-->

  {#if isOpen}
    <div
      class="sm:hidden absolute top-12 right-6 bg-white shadow-lg rounded-lg py-2 px-2 mt-2"
    >
      {#each tabs as tab, index}
        <a href={tab.link} class="block py-1 hover:text-violet-500 {y > 0 ? 'text-black' : 'text-black'}">
          <p>{tab.name}</p>
        </a>
      {/each}
    </div>
  {/if}

  <div class="sm:flex ml-auto pr-4 items-center gap-4 hidden text-xl">
    {#each tabs as tab, index}
      <a
        href={tab.link}
        class="duration-200 hover:text-violet-500 hidden sm:block"
      >
        <p>{tab.name}</p>
      </a>
    {/each}
  </div>

  <hr class="mt-4 border-b-2 border-gray-400" />
</header>

<style>
  button svg {
    fill: none;
    stroke: currentColor;
    stroke-linecap: round;
    stroke-linejoin: round;
    stroke-width: 2;
  }

  .absolute {
    background-color: #f9f9f9;
    transition: all 0.3s ease-in-out;
    z-index: 999;
  }

  header {
    width: 100%;
    background-color: transition all 0.2s ease-in-out;
  }

  header.scrolled {
    background-color: #f5f5f5;
  }

  .sm:hidden {
    display: none;
    position: absolute;
    top: 12px;
    right: 6px;
    background-color: #b88c8c;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    border-radius: 0.5rem;
    padding: 8px;
    z-index: 999;
  }

  @media (min-width: 1024px) {
    header {
      padding-left: 6rem; /* Adjust as needed */
      padding-right: 6rem; /* Adjust as needed */
    }
  }
</style>
