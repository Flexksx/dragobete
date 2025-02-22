<script>
	import { fly, fade } from 'svelte/transition';
	import { onMount } from 'svelte';
	import Header from '$lib/components/custom/Header.svelte';
	import HeartImage from '$lib/components/images/HeartImage.svelte';
	import RoundSquareImage from '$lib/components/images/RoundSquareImage.svelte';
	import CloudImage from '$lib/components/images/CloudImage.svelte';

	let showContent = false;

	onMount(() => {
		showContent = true;
	});
</script>

{#if showContent}
	<div class="flex items-center justify-between">
		<div>
			<div transition:fly={{ x: -200, duration: 1000, delay: 100 }}>
				<img src="images/flowers/flower2.png" width="90" alt="Flower 2" />
			</div>
			<div transition:fly={{ x: -200, duration: 1000, delay: 150 }}>
				<img src="images/flowers/flower8.png" width="60" alt="Flower 8" />
			</div>
		</div>

		<div transition:fade={{ duration: 1000, delay: 200 }}>
			<Header />
		</div>

		<div transition:fly={{ x: 200, duration: 1000, delay: 100 }}>
			<img src="images/flowers/flower1.png" width="100" alt="Flower 1" />
		</div>
	</div>
	<div class="mt-8 flex justify-between">
		<div transition:fly={{ y: 200, duration: 1000, delay: 100 }}>
			<HeartImage imagePath="images/gf/Tudorita.jpg" />
		</div>
		<div transition:fly={{ y: 200, duration: 1000, delay: 300 }}>
			<RoundSquareImage imagePath="images/gf/Tudorita3.jpg" />
		</div>
	</div>

	<div class="mt-8" transition:fly={{ y: 200, duration: 1000, delay: 500 }}>
		<CloudImage imagePath="images/gf/Tudorita5.jpg" />
	</div>
{/if}
