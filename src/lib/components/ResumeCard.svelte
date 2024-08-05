<script lang="ts">
  export let date: string;
  export let title: string;
  export let company: string;
</script>

<div class="bg-secondary mb-4 p-8 shadow-2xl flex flex-col sm:flex-row items-center gap-16">
  <div class="flex flex-col min-w-32">
    <span class="text-primary font-bold">{date}</span>
    <span class="font-bold">{title}</span>
    <span>{company}</span>
  </div>
  <div class="flex justify-center items-center">

   <slot/>

  </div>
</div>
