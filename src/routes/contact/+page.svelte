<script lang="ts">
  import Title from "$lib/components/Title.svelte";
  import Continer from "$lib/components/Continer.svelte";
  import Lab from "$lib/components/Lab.svelte";
  import Textarea from "$lib/components/ui/textarea/textarea.svelte";
  import Label from "$lib/components/ui/label/label.svelte";
  import Button from '$lib/components/ui/button/button.svelte';
</script>

<svelte:head>
  <title>
    Badr - Let's talk
  </title>
</svelte:head>
<Continer class="flex flex-col gap-10">
  <Title title="Let's talk"></Title>
  <form  action="https://formsubmit.co/9modi111@gmail.com" method="POST" 
  class="bg-secondary p-8 flex flex-col gap-4 text-secondary-foreground">
    <div>
      <Lab
        Type="text"
        For="name"
        Id="name"
        Name="name"
        AA="Full name"
        Placeholder="Write your name"
      ></Lab>
    </div>
    <div>
      <Lab
        Type="email"
        For="email"
        Id="email"
        Name="email"
        AA="Email"
        Placeholder="example@gmail.com"
      ></Lab>
    </div>
    <div>
      <Lab
        Type=""
        For="subject"
        Id="subject"
        Name="subject"
        AA="Subject"
        Placeholder="..."
      ></Lab>
    </div>
    <div>
      <Label for="Message">Message</Label>
      <Textarea required name="Message" id="Message" placeholder="..." />
    </div>
    <Button  class="max-w-32"  type="submit" >
        Send
    </Button>
  </form>
</Continer>
