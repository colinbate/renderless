<script lang="ts">
import { fly } from 'svelte/transition';
export let open = false;
export let align: 'right' | 'left' = 'left';
function toggle(force?: boolean) {
  open = force ?? !open;
}
</script>
<slot {toggle} name="trigger" />
{#if open}
  <div class="overflow-hidden absolute" class:left-0={align === 'left'} class:right-0={align === 'right'}>
    <div transition:fly={{ y: -50 }}>
      <slot {toggle} />
    </div>
  </div>
{/if}