<script>
	import Tab from './Tab.svelte';
	const tabs = ['Home', 'Projects', 'Contact'];
</script>

<div class="navbar">
	{#each tabs as tab}
		<Tab tabName={tab} />
	{/each}
	<div class="filler" />
</div>

<style>
	.navbar {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		height: fit-content;
		display: flex;
		justify-content: flex-start;
		align-items: center;
		padding: 0;
	}
	.filler {
		height: 2.5rem;
		flex-grow: 1;
		border-bottom: 1px solid var(--color-inactive);
	}
</style>
