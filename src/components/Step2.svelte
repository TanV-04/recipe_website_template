<script>
  export let step;
</script>

<a
  href={step.link}
  class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-violet-700 text-center group cursor-pointer hover:border-violet-400 duration-200 xs:w-full sm:w-[75%] mx-auto"
>
  <div
    class="relative overflow-hidden rounded-lg border border-violet-700 hover:border-violet-400"
  >
    <div
      class="absolute inset-0 bg-slate-950 bg-opacity-75 flex items-center justify-center transition-opacity opacity-0 group-hover:opacity-100 duration-200"
    >
      <p class="text-white text-2xl md:text-3xl font-semibold">Go to &rarr;</p>
    </div>

    <img
      class="aspect-ratio w-[100%] md:h-auto object-cover"
      src={step.src}
      alt={step.name}
    />
  </div>
  <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">{step.name}</h3>
  <h6 class="eb-garamond font-small text-sm sm:text-lg md:text-xl">{step.description}</h6>
  <slot />
</a>

<style>

</style>
