<script>
	import hero from '$lib/assets/images/hero-img.jpg';
	import club from '$lib/assets/images/poa.png';
	import duck from '$lib/assets/images/duck.png';
	import dental from '$lib/assets/images/dental.jpg';
	import maintenance from '$lib/assets/images/maintenance.jpg';

	import Card from '$lib/components/Card.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>

<main class="bg-background">
	<div class="relative">
		<img
			class="w-full brightness-60"
			src={hero}
			alt="School children receiving a care package from the Rotary Club of Durbanville"
		/>
		<h1
			class="absolute top-[50%] left-[5%] text-4xl font-bold text-white select-none md:text-6xl lg:text-8xl"
		>
			People of Action.
		</h1>
	</div>

	<div class="flex flex-col items-center justify-evenly p-5 md:flex-row">
		<p
			class="text-md my-8 text-center align-middle font-semibold text-rotary-blue select-none md:max-w-1/2 md:text-2xl"
		>
			The Rotary Club of Durbanville is dedicated to uplifting its community through local
			collaboration. We partner with local businesses and organizations to bring value to the
			Durbanville community; and the funds we raise are used for projects that improve the
			Durbanville area.
		</p>

		<img src={club} alt="" class="w-10/12 rounded-xl object-cover md:max-w-1/3" />
	</div>

	<div class="flex flex-col items-center bg-[#c6bcd000] p-4">
		<h1 class="mt-8 text-center text-3xl font-bold text-rotary-blue md:text-4xl">
			Where you've seen us recently
		</h1>
		<div class="flex flex-wrap justify-center bg-[#c6bcd000]">
			<Card
				title="Duck Derby"
				image={duck}
				desc="The Duck Derby offers a thrilling day out for families to sponsor and support their duck as it competes against hundreds more. Racing down our watercourse at the scenic Bloemendal Trail Park, each duck affords an opportunity to win grand prizes!"
			/>
			<Card
				title="Community Health Day"
				image={dental}
				desc="Our club hosts a Community Health Day once year in Klipheuwel and Fisantekraal, offering high-quality healthcare services to the local community. Medical students get an opportunity to gain practical experience and participate in outreach."
			/>
			<Card
				title="School maintenance"
				image={maintenance}
				desc="Rotary Club of Durbanville supports 9 under-resourced schools in the Northern Suburbs, providing essential maintenance and resources; ensuring the learners&rsquo; right to education is upheld."
				imageOptions="object-[25%_100%]"
			/>
		</div>
	</div>

	<Footer />
</main>
