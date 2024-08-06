<script>
  import Button from "$lib/components/ui/button/button.svelte";
  import ResumeCard from "$lib/components/ResumeCard.svelte";
  import Title from "$lib/components/Title.svelte";
    import Continer from "$lib/components/Continer.svelte";

</script>

<Continer >
  <Title title="Resume"></Title>
  <div class="pt-16 flex flex-col gap-8">
    <div class="flex justify-between items-center mb-2">
      <span class="text-2xl font-bold">Education</span>
      <Button class="">MY CV</Button>
    </div>
    <ResumeCard
      date="2023 - present"
      title="Computer Science Bachelor"
      company="Umm Al-Qura University"
    >
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet nihil id
        eos labore dolor veniam libero ea harum dolore? Illum dolore fugit non
        odit expedita sint voluptate dignissimos eaque excepturi?
      </p></ResumeCard
    >
    <ResumeCard
      date="2023 - present"
      title="Computer Science Bachelor"
      company="Umm Al-Qura University"
    ></ResumeCard>
  </div>
</Continer>
