<script>
  import Button from "$lib/components/ui/button/button.svelte";
</script>

<div class="mx-auto px-3 max-w-screen-sm pt-12 gap-2">
  <h1 class="flex w-fit items-center gap-2">
    <div class="bg-primary h-6 w-6 mt-1"></div>
    <span class="font-bold text-4xl">Resume</span>
  </h1>
  <div class="pt-16">
    <div class="flex justify-between items-center mb-2">
      <span class="text-2xl font-bold">Education</span>
      <Button class="">MY CV</Button>
    </div>
    <div class="bg-secondary p-8 shadow-2xl flex items-center gap-20">
      <div class="flex flex-col min-w-32">
				<span class="text-primary font-bold">2023 - present</span>
				<span class="font-bold">Computer science Bachelor</span>
				<span>Umm Al-Qura University</span>
			</div>
      <div>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis magni, quos minima ratione nulla quo sapiente est debitis temporibus, quis asperiores inventore eaque error! Amet pariatur eum impedit deleniti fugit!
				</p>
			</div>
    </div>
  </div>
</div>
