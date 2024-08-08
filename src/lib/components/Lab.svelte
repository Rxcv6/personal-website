<script lang="ts">
  import Input from "$lib/components/ui/input/input.svelte";
  import Label from "$lib/components/ui/label/label.svelte";
  export let For: string;
  export let Id: string;
  export let Name: string;
  export let Placeholder: string;
  export let AA: string;
  export let Type:string;
</script>

<Label for={For}>{AA}</Label>
<Input required type={Type} name={Name} id= {Id} placeholder={Placeholder} />
