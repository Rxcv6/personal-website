<script lang="ts">
  import { cn } from "$lib/utils";

     let className="";
     export{className as class}
</script>
<div class={cn("mx-auto px-3 max-w-screen-sm py-16", className)}>
    <slot></slot>
</div>