<script>
	import Card from '$lib/components/Card.svelte';
	import spidey from '$lib/assets/images/spiderman.jpeg';
	import duck from '$lib/assets/images/duck.png';
	import easter from '$lib/assets/images/THANK YOU.png';
	import maintenance from '$lib/assets/images/maintenance.jpg';
	import academic from '$lib/assets/images/prize_giving.jpg';
	import mandela from '$lib/assets/images/mandela.png';
	import dental from '$lib/assets/images/dental.jpg';
	import oomPiet from '$lib/assets/images/oom_piet_cast.jpeg';
	import Footer from '$lib/components/Footer.svelte';
</script>

<main class="bg-background">
	<div class="flex flex-col items-center p-4 select-none">
		<h1
			class="mt-4 text-4xl font-bold text-rotary-blue underline decoration-rotary-gold decoration-2 underline-offset-4"
		>
			Our Events
		</h1>
		<h2 class="mt-2 text-2xl font-light text-rotary-blue">How we enrich the community</h2>
	</div>

	<div class="flex flex-wrap justify-center">
		<Card
			title="Oom Piet's Christmas Party"
			image={spidey}
			desc="We&rsquo;ve been hosting our flagship event in Durbanville for over 10 years. This annual event brings families together for a wondrous evening show featuring your child&rsquo;s favourite friends, firefighters, magicians, and of course Santa."
		/>
		<Card
			title="Durbanville Duck Derby"
			image={duck}
			desc="The Duck Derby offers a thrilling day out for families to sponsor and support their duck as it competes against hundreds more. Racing down our watercourse at the scenic Bloemendal Trail Park, each duck affords an opportunity to win grand prizes!"
		/>
		<Card
			title="Easter Egg Hunt"
			image={easter}
			desc="Our annual children&rsquo;s Easter Egg Hunt allows children to explore and hunt for hidden Easter eggs with their friends; as well as take part in some friendly competitions with awesome prizes on offer."
		/>
	</div>

	<div class="mx-auto mt-15 h-0.5 w-4/6 bg-rotary-gold"></div>

	<div class="mt-15 flex flex-col items-center p-4 select-none">
		<h1
			class="mt-4 text-4xl font-bold text-rotary-blue underline decoration-rotary-gold decoration-2 underline-offset-4"
		>
			Our Projects
		</h1>
		<h2 class="mt-2 text-2xl font-light text-rotary-blue">How we use our funds</h2>
	</div>

	<div class="flex flex-wrap justify-center">
		<Card
			title="Commnunity Health Day"
			image={dental}
			desc="Our club hosts a Community Health Day once year in Klipheuwel and Fisantekraal, offering high-quality healthcare services to the local community. Medical students get an opportunity to gain practical experience and participate in outreach."
		/>
		<Card
			title="School maintenance"
			image={maintenance}
			desc="Rotary Club of Durbanville supports 9 under-resourced schools in the Northern Suburbs, providing essential maintenance and resources; ensuring the learners&rsquo; right to education is upheld."
			imageOptions="object-[25%_100%]"
		/>
		<Card
			title="Recognising academic brilliance"
			image={academic}
			desc="We host an annual academic prize-giving for our supported schools, recognizing learners&rsquo; achievements with a donation of items that supports their future education. This initiative promotes real ambition in our next generation."
		/>
		<Card
			title="Mandela Day"
			image={mandela}
			desc="We honour the legacy of Madiba by orchestrating a large-scale food drive that provides balanced meals to over 3 500 empoverished school children."
		/>
		<Card
			title="Interact"
			image={oomPiet}
			desc="The Rotary Club of Durbanville proudly sponsors the Interact Clubs of Fairmont High and Curro Durbanville High. Interactors are given opportunities to plan and execute on their own community improvement initiatives."
		/>
	</div>

	<Footer />
</main>
