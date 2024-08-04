<script lang="ts">
  import Button from "$lib/components/ui/button/button.svelte";
  import { page } from "$app/stores";
  import MenuIcon from "./MenuIcon.svelte";
  import * as Sheet from "$lib/components/ui/sheet";
  import ThemeSwitch from "$lib/components/ThemSwitch.svelte";
  import ThemSwitch from "$lib/components/ThemSwitch.svelte";

  const links = [
    {
      text: "About Me",
      href: "/",
    },
    {
      text: "resume",
      href: "/resume",
    },
    {
      text: "Projects",
      href: "/projects",
    },
    {
      text: "contact",
      href: "/contact",
    },
  ];
  let isOpen = false;
</script>

<div class=" bg-secondary text-secondary-foreground py-8 px-4">
  <nav class="max-w-screen-2xl flex justify-between items-center mx-auto">
    <div class="flex gap-2 items-center">
      <div class="bg-primary h-6 w-6 me-3"></div>
      <a href="/">
        <div class=" flex items-end gap-2">
          <span class="font-bold text-3xl">Badr Al yasi </span>

          <span class="text-xl uppercase hidden sm:flex">
            / Computer science</span
          >
        </div>
      </a>
    </div>
    <div class="flex">
      <ThemSwitch />
      <div class="uppercase hidden lg:flex">
        {#each links as link}
          <Button
            class=" {$page.url.pathname == link.href && 'text-primary'}"
            href={link.href}
            variant="link">{link.text}</Button
          >
        {/each}
      </div>
      <Sheet.Root bind:open={isOpen}>
        <Sheet.Trigger class="flex lg:hidden">
          <Button size="icon" variant="ghost"><MenuIcon></MenuIcon></Button
          ></Sheet.Trigger
        >
        <Sheet.Content class="flex flex-col justify-center">
          {#each links as link}
            <Button
              on:click={() => (isOpen = false)}
              class=" {$page.url.pathname == link.href && 'text-primary'}"
              href={link.href}
              variant="link">{link.text}</Button
            >
          {/each}
        </Sheet.Content>
      </Sheet.Root>
    </div>
  </nav>
</div>
