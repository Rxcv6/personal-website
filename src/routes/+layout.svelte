<script>
  import "../app.css";
  import { ModeWatcher } from "mode-watcher";
  import NavBar from "$lib/components/NavBar.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<NavBar></NavBar>
<ModeWatcher />
<main class="min-h-[calc(100vh-13.5rem)]">
<slot></slot>
</main>

<Footer></Footer>
