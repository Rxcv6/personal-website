<script lang="ts">
  import Social from "$lib/components/Social.svelte";
</script>

<footer class=" bg-secondary text-secondary-foreground py-8 px-4">
  <div
    class="max-w-screen-2xl flex flex-row-reverse md:flex-row justify-between items-center mx-auto"
  >
    <span class=" self-end md:self-center"> ©{new Date().getFullYear()} </span>
    <div class=" flex flex-col md:flex-row gap-3 md:gap-14">
      <span class="flex gap-5 md:gap-0 md:flex-col items-center ">
        <span class="font-bold">Call </span>
        <a href="tel:0555032750" class="">0555032750 </a>
      </span>
      <span class="flex  gap-5 md:gap-0 md:flex-col items-center">
        <span class="font-bold">Email </span>
        <a href="mailto:9modi111@gmail.com">9modi111@gmail.com </a>
      </span>
      <span class="flex  items-center">
        <Social></Social>
      </span>
    </div>
  </div>
</footer>
