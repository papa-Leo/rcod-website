<script>
	import Profile from '$lib/components/Profile.svelte';
	import Footer from '$lib/components/Footer.svelte';

	import club from '$lib/assets/images/dental_brief.jpg';
	import volunteer from '$lib/assets/images/volunteer.jpg';
	import graham from '$lib/assets/images/rotarians/Graham Harmsworth.jpg';
	import maureen from '$lib/assets/images/rotarians/maureen-harmsworth.jpg';
	import mel from '$lib/assets/images/rotarians/mel-downey.jpg';
	import mike from '$lib/assets/images/rotarians/Mike Downey.jpg';
	import leandro from '$lib/assets/images/rotarians/leandro-consani.gif';
	import robert from '$lib/assets/images/rotarians/Robert Consani.jpg';
	import luana from '$lib/assets/images/rotarians/luana-consani.jpg';
	import ben from '$lib/assets/images/rotarians/Ben Lomnitz.jpg';
	import judith from '$lib/assets/images/rotarians/judith-viljoen.jpg';
	import jd from '$lib/assets/images/rotarians/jd-aucamp.jpeg';
	import eugene from '$lib/assets/images/rotarians/EugeneVisser2026.jpeg';

	let innerWidth = $state(window.innerWidth);
	let isMobile = $derived(innerWidth < 768);
</script>

<svelte:window bind:innerWidth />

<main class="bg-background">
	<div class="flex flex-col justify-evenly p-5 md:flex-row">
		{#if isMobile}
			<img src={volunteer} alt="" class="rounded-xl object-cover md:max-w-1/3" />
		{/if}

		<p
			class="text-md my-auto text-center align-middle font-semibold text-rotary-blue md:max-w-1/2 md:text-xl"
		>
			<strong>Want to get involved?</strong> We have a wonderful group of volunteers who help to
			make the club&rsquo;s vision come true; including Interactors, Inner Wheelers, family,
			friends, and neighbours. We welcome anyone willing to assist with our projects and make
			Durbanville a better place - no hard commitments!
			<a href="https://linktr.ee/durbanvillerotary" class="text-rotary-orange"
				>Click here for more info.</a
			>
		</p>

		{#if !isMobile}
			<img src={volunteer} alt="" class="rounded-xl object-cover md:max-w-1/3" />
		{/if}
	</div>

	<div class="flex flex-col justify-evenly p-5 md:flex-row">
		<img src={club} alt="" class="rounded-xl object-cover md:max-w-1/3" />

		<p
			class="text-md my-auto text-center align-middle font-semibold text-rotary-blue md:max-w-1/2 md:text-xl"
		>
			<strong>More?</strong> Becoming a Rotarian gives you the chance to develop skills like public speaking,
			project management, and event planning. You&rsquo;ll meet interesting people from our district and
			around the world; and you&rsquo;ll tackle local and international issues that are important to you
			and your fellow club members.
		</p>
	</div>

	<div class="mx-auto mt-15 h-0.5 w-4/6 bg-rotary-gold"></div>

	<div class="flex flex-col items-center p-4 select-none">
		<h1
			class="mt-4 text-4xl font-bold text-rotary-blue underline decoration-rotary-gold decoration-2 underline-offset-4"
		>
			Rotarians
		</h1>
	</div>
	<div class="flex flex-wrap justify-center">
		<Profile
			image={graham}
			name="Graham Harmsworth"
			title="President"
			desc="Graham is among the oldest serving members of the club, having been a Durbanville Rotarian since 19xx. He maintains a high reputation for his work as President."
		/>
		<Profile
			image={mel}
			name="Melinde &ldquo;Mel&rdquo; Downey"
			title="Secretary"
			desc="Mel is the main visionary force behind the Rotary Club of Durbanville, constantly bringing fresh ideas forward and expanding the club's reach."
		/>
		<Profile
			image={mike}
			name="Michael &ldquo;Mike&rdquo; Downey"
			title="Treasurer"
			desc="Mike is a notable member of the club&rsquo;s technical team, responsible for workshopping ideas and driving the club closer to its mission."
		/>
		<Profile
			image={robert}
			name="Robert Consani"
			title="PP, PHF++"
			desc="As the most senior Rotarian in our club, having served since 19xx, Robert&rsquo;s extensive experience makes him an invaluable mentor for the club in it&rsquo;s endeavours."
		/>
		<Profile
			image={luana}
			name="Luana Consani"
			title="HR, IW, PHF+"
			desc="As both an Inner Wheeler and Honourary Rotarian, Luana brings a wealth of experience to the club - on top of her constant joyful energy."
		/>
		<Profile
			image={maureen}
			name="Maureen Harmsworth"
			title="HR, IW, PHF"
			desc="Maureen is a dual Inner Wheeler and Honourary Rotarian. Her warm, welcoming touch can be felt throughout the club&rsquo;s work."
		/>
		<Profile
			image={ben}
			name="Ben Lomnitz"
			title="PP, PHF"
			desc="Ben is the club&rsquo;s most recent Paul Harris Fellow, an award which he has clearly earned through many committed years of service."
		/>
		<Profile
			image={leandro}
			name="Leandro Consani"
			title="Rotarian"
			desc="As the youngest Rotarian in the club, Leandro wants to use his passion and skills to improve the community in which he lives."
		/>
		<Profile
			image={eugene}
			name="Eugène Visser"
			title="Rotarian"
			desc="Although he ranks amoung the newer members, Eugène contributes great expertise and skill to the Rotary Club of Durbanville."
		/>
		<Profile
			image={judith}
			name="Judith Viljoen"
			title="Rotarian"
			desc="Judith brings her superior networking skills and permanent well of positive energy to the club and all its projects."
		/>
		<Profile
			image={jd}
			name="JD Aucamp"
			title="Rotarian"
			desc="As the newest member of the club, JD hopes to leave a positive mark in our community through his work."
		/>
	</div>

	<Footer />
</main>
