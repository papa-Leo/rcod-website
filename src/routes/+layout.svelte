<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import Button from '$lib/components/Button.svelte';
	import logo from '$lib/assets/rcod_logo_dark.png';

	let { children } = $props();
</script>

<svelte:head
	><link rel="icon" href={favicon} />

	<nav class="sticky top-0 z-20 flex w-full items-center justify-around bg-rotary-blue shadow-xs">
		<a href="/">
			<img class="inline max-h-30" src={logo} alt="Logo for Rotary Club of Durbanville" />
		</a>

		<div class="mr-4 inline">
			<Button text="Home" link="/" />
			<Button text="Events & Projects" link="/projects-and-events" />
			<Button text="People" link="/people" />
			<Button text="Benefactors" link="/benefactors" />
			<Button text="More info" link="/more-info" />
		</div>
	</nav>
</svelte:head>

{@render children()}
