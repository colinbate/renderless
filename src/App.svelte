<script lang="ts">
	import ModeSwitcher from './ModeSwitcher.svelte';
	import Tailwindcss from './Tailwindcss.svelte';
	import Dropdown from './dropdown/Dropdown.svelte';
</script>
<Tailwindcss />
<ModeSwitcher />
<main class="p-4 mx-auto max-w-3xl">
	<h1 class="uppercase text-6xl text-center leading-normal font-thin text-svelte">Renderless Components</h1>
	
	<h2 class="text-2xl my-4">Dropdown</h2>
	<Dropdown align="right"></Dropdown>

	<h2 class="text-2xl my-4">Dropdown List</h2>

	<h2 class="text-2xl my-4">Dropdown Toggle List</h2>
</main>