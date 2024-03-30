<script lang="ts">
	import '../app.postcss';
	import { AppShell, AppBar } from '@skeletonlabs/skeleton';

	let innerWidth = 0;
	let HIDE_SOCMED_TEXT_THRESHOLD = 770; // measured in px
</script>

<svelte:window bind:innerWidth />

<!-- App Shell -->
<AppShell>
	<svelte:fragment slot="header">
		<!-- App Bar -->
		<AppBar>
			<svelte:fragment slot="lead">
				<strong class="text-xl uppercase">DevelUP Kamustahan</strong>
			</svelte:fragment>
			<svelte:fragment slot="trail">
				{#if innerWidth > HIDE_SOCMED_TEXT_THRESHOLD}
					<a
						class="btn btn-sm variant-ghost-surface"
						href="https://discord.com/users/242108300966100993"
						target="_blank"
						rel="noreferrer"
					>
						<i class="fa-brands fa-discord pr-2"/> morthodox
					</a>
					<a
					class="btn btn-sm variant-ghost-surface"
					href="https://github.com/Dox-Dev"
					target="_blank"
					rel="noreferrer"
					>
						<i class="fa-brands fa-github pr-2"/> Dox-Dev
					</a>
					<a
						class="btn btn-sm variant-ghost-surface"
						href="https://www.facebook.com/joseellis.caluag/"
						target="_blank"
						rel="noreferrer"
					>
						<i class="fa-brands fa-facebook pr-2"/> Jose Ellis Miguel Caluag
					</a>
				{:else}
					<a
						class="btn-icon variant-ghost-surface"
						href="https://discord.com/users/242108300966100993"
						target="_blank"
						rel="noreferrer"
					>
						<i class="fa-brands fa-discord"/>
					</a>
					<a
					class="btn-icon variant-ghost-surface"
					href="https://github.com/Dox-Dev"
					target="_blank"
					rel="noreferrer"
					>
						<i class="fa-brands fa-github"/>
					</a>
					<a
						class="btn-icon variant-ghost-surface"
						href="https://www.facebook.com/joseellis.caluag/"
						target="_blank"
						rel="noreferrer"
					>
						<i class="fa-brands fa-facebook"/>
					</a>
				{/if}
			</svelte:fragment>
		</AppBar>
	</svelte:fragment>
	<!-- Page Route Content -->
	<slot />
</AppShell>
