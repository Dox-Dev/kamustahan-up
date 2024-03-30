<script lang="ts">
	import '../app.postcss';
	import { AppShell, AppBar } from '@skeletonlabs/skeleton';
</script>

<!-- App Shell -->
<AppShell>
	<svelte:fragment slot="header">
		<!-- App Bar -->
		<AppBar>
			<svelte:fragment slot="lead">
				<strong class="text-xl uppercase">DevelUP Kamustahan</strong>
			</svelte:fragment>
			<svelte:fragment slot="trail">
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
			</svelte:fragment>
		</AppBar>
	</svelte:fragment>
	<!-- Page Route Content -->
	<slot />
</AppShell>
