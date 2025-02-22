<script>
	import { fly, fade } from 'svelte/transition';
	import { onMount } from 'svelte';
	import Header from '$lib/components/custom/Header.svelte';

	let showContent = false;

	onMount(() => {
		showContent = true;
	});
</script>

{#if showContent}
	<div class="flex items-center justify-between">
		<div transition:fly={{ x: -200, duration: 1000 }}>
			<img src="/src/lib/images/flowers/flower2.png" width="90" alt="Flower 2" />
			<img src="/src/lib/images/flowers/flower8.png" width="60" alt="Flower 8" />
		</div>

		<div transition:fade={{ duration: 1000, delay: 200 }}>
			<Header />
		</div>

		<div transition:fly={{ x: 200, duration: 1000 }}>
			<img src="/src/lib/images/flowers/flower1.png" width="100" alt="Flower 1" />
		</div>
	</div>
{/if}
