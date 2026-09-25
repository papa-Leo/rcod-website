<script>
	const { title, image, desc, imageOptions = 'object-[0%_25%]' } = $props();
</script>

<div
	class="m-8 max-w-10/12 rounded-xl border-2 border-rotary-blue bg-rotary-blue p-2 text-white select-none md:max-w-4/12 lg:w-3/12"
>
	<div class="rounded-lg">
		<img src={image} alt={title} class="h-60 w-full rounded-t-lg object-cover {imageOptions}" />
		<div class="rounded-t-md p-2 text-2xl font-semibold">
			<h3>{title}</h3>
		</div>
		<div class="rounded-b-md p-2">
			<p class="">{desc}</p>
		</div>
	</div>
</div>
