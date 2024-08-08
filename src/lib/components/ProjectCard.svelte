<script lang="ts">
  export let title: string;
  export let subtitle: string;
  export let imageSrc: string;
</script>

<div
  class="bg-secondary text-secondary-foreground flex flex-col sm:flex-row shadow-2xl   gap-4"
>
 <div class="flex flex-col gap-4 pt-8 ">
	<div class="flex flex-col min-w-32 border-primary ps-4 border-s-8">
    <span class="font-bold text-primary">{title}</span>
    <span class="font-bold text-primary">{subtitle}</span>
  </div>
   <div class="ps-8 pb-8">
    <slot />
   </div>
 </div>
  <img src={imageSrc}  alt="photo"  class="w-auto sm:w-64 object-cover" />
</div>
