<script lang="ts">
import DropdownBehavior from "./DropdownBehavior.svelte";
export let open = false;
export let align: 'right' | 'left' = 'left';
</script>
<div class="relative">
<DropdownBehavior let:toggle bind:open {align}>
  <button slot="trigger" type="button" on:click={() => toggle()} class="bg-svelte text-white rounded px-3 py-1">Toggle</button>
  <div class="border rounded shadow p-3 border-gray-500 dark:border-gray-100 bg-gray-300 dark:bg-black">
    Whatever
  </div>
</DropdownBehavior>
</div>
