<!-- YOU CAN DELETE EVERYTHING IN THIS PAGE -->

<script>
	import MyAccordion from "$lib/MyAccordion.svelte";
	
	let innerWidth = 0;
	let HIDE_HEADER_THRESHOLD = 1024; // measured in px
</script>

<svelte:window bind:innerWidth />

<div class="container h-full mx-auto flex justify-center items-center">
	{#if innerWidth < HIDE_HEADER_THRESHOLD}
		<div class="space-y-10 text-center flex flex-col items-center">
			<h2 class="h2 text-center">So you wanna ask how I'm doing? G!</h2>
			<MyAccordion />
		</div>
	{:else}
		<div class="space-y-10 text-center flex flex-row items-center">
			<h2 class="h2 text-center">So you wanna ask how I'm doing? G!</h2>
			<MyAccordion />
		</div>
	{/if}
</div>

<style lang="postcss">
	figure {
		@apply flex relative flex-col;
	}
	figure svg,
	.img-bg {
		@apply w-64 h-64 md:w-80 md:h-80;
	}
	.img-bg {
		@apply absolute z-[-1] rounded-full blur-[50px] transition-all;
		animation: pulse 5s cubic-bezier(0, 0, 0, 0.5) infinite,
			glow 5s linear infinite;
	}
	@keyframes glow {
		0% {
			@apply bg-primary-400/50;
		}
		33% {
			@apply bg-secondary-400/50;
		}
		66% {
			@apply bg-tertiary-400/50;
		}
		100% {
			@apply bg-primary-400/50;
		}
	}
	@keyframes pulse {
		50% {
			transform: scale(1.5);
		}
	}
</style>
