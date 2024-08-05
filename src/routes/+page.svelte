<script lang="ts">
  import Button from "$lib/components/ui/button/button.svelte";
 import Social from "$lib/components/Social.svelte";
</script>

<div class=" flex justify-end pb-[30rem] lg:pb-0">
  <div
    class="bg-secondary relative min-h-[40vh] min-w-full lg:min-h-[calc(100vh-13.5rem)] lg:min-w-[60vw] items-center flex justify-center text-secondary-foreground pb-32"
  >
    <div
      class="bg-[#f4ece6] dark:bg-[#303030]  shadow-[0_30px_70px_-15px_rgba(0,0,0,0.6)] w-[20rem]  translate-y-[85%] lg:translate-y-[20%] absolute lg:start-10 lg:-translate-x-full flex flex-col items-center justify-between pt-8 gap-3 self-start "
    >
      <img
        src="/avater.jpg"
        class="w-60 h-56 grayscale rounded-full"
        alt="صورة شخصية"
      />
      <div class=" flex flex-col items-center gap-6  dark:text-white">
        <h1 class="font-bold text-4xl">Badr</h1>
        <hr class="w-20 border-primary border-2" />
        <h2 class="text-2xl">Programming</h2>
      </div>
      <div
        class="bg-secondary w-full flex justify-center p-2 mt-10 text-secondary-foreground"
      >
      <Social></Social>
      </div>
    </div>
    <div class="mx-10 max-w-[30rem] flex flex-col gap-8">
      <h1 class="text-8xl font-bold">Hello</h1>
      <h4>here's who I am & what I do</h4>
      <div class="flex gap-2">
        <Button class="w-32" href="/resume">Resume</Button>
        <Button variant="ghost"  class="w-32 border" href="/projects">Projects</Button>
      </div>
      <div>
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aliquid
          suscipit veritatis natus autem architecto? Mollitia doloremque, non
          beatae minus ea voluptatibus eum, quos aliquid enim ab sequi
          necessitatibus placeat aliquam.
        </p>
      </div>
    </div>
  </div>
  
</div>
