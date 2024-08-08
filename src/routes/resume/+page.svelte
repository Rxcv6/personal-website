<script>
  import Button from "$lib/components/ui/button/button.svelte";
  import ResumeCard from "$lib/components/ResumeCard.svelte";
  import Title from "$lib/components/Title.svelte";
    import Continer from "$lib/components/Continer.svelte";

</script>
<svelte:head>
  <title>
    Badr - Resume
  </title>
</svelte:head>
<Continer >
  <Title title="Resume"></Title>
  <div class="pt-16 flex flex-col gap-8">
    <div class="flex justify-between items-center mb-2">
      <span class="text-2xl font-bold">Education</span>
      
    </div>
    <ResumeCard
      date="2023 - present"
      title="Computer Science Bachelor"
      company="Umm Al-Qura University"
    >
      </ResumeCard
    >
    
  </div>
</Continer>
