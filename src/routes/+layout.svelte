<script>
  import "../app.css";
    import { ModeWatcher } from "mode-watcher";
    import NavBar from "$lib/components/NavBar.svelte";
</script>
<NavBar>
</NavBar>
<ModeWatcher />

<slot></slot>
