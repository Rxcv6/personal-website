<script lang="ts">
  import Continer from "$lib/components/Continer.svelte";
  import ProjectCard from "$lib/components/ProjectCard.svelte";
  import Title from "$lib/components/Title.svelte";
  import Button from "$lib/components/ui/button/button.svelte";
</script>

<svelte:head>
  <title>Badr - Projects</title>
</svelte:head>
<Continer class=" flex flex-col gap-16">
  <Title title="Projects"></Title>

  <ProjectCard title="Calculator" subtitle="" imageSrc="/project1.png">
    <p class="pb-2.5">A simple, beautiful, and wonderful calculator.</p>
    <Button href="https://redstonecalculator.netlify.app/" target="_blank" variant="ghost">
      Try it</Button
    >
  </ProjectCard>
  <ProjectCard title="A To-Do list" subtitle="" imageSrc="/project2.png">
    <p class="pb-2.5">
      A user-friendly personal task tracker that makes it easy to add, delete,
      and view upcoming tasks.
    </p>
    <Button href="https://redstonetodolist.netlify.app/" target="_blank" variant="ghost">
      Try it</Button
    >
  </ProjectCard>
</Continer>
