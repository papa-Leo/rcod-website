<script>
	import BenefactorCard from '$lib/components/BenefactorCard.svelte';
	import leandro from '$lib/assets/images/rotarians/leandro-consani.jpeg';
</script>

<main>
	<div class="flex flex-col items-center p-4 select-none">
		<h1
			class="mt-4 text-4xl font-bold text-rotary-blue underline decoration-rotary-gold decoration-2 underline-offset-4"
		>
			Benefactors
		</h1>
		<h2 class="mt-2 text-center text-2xl font-light text-rotary-blue">
			These are the companies and people that helped us to achieve our goals this year
		</h2>
	</div>

	<BenefactorCard title="Ozow" image={leandro} desc="Ozow is a company" />
</main>
