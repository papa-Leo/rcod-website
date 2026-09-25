<script>
	import { currentYear } from '$lib/scripts/currentYear.js';
</script>

<footer>
	<div id="footer" class="flex flex-col justify-between bg-rotary-blue p-4 md:flex-row">
		<span class="text-white"
			>The Rotary Club of Durbanville is a proud member of <a
				href="https://www.rotary.org"
				class="duration-200 hover:text-rotary-gold">Rotary International</a
			>
			|
			<a href="https://d9350.co.za/" class="duration-200 hover:text-rotary-gold">District 9350</a
			></span
		>
		<span class="mt-6 text-white md:mt-0">© Rotary Club of Durbanville {currentYear()}</span>
	</div>
</footer>
