<script>
	const { image, name, title = '', desc, imageOptions = '' } = $props();
</script>

<div
	class="m-8 flex w-10/12 flex-col justify-start rounded-lg border-2 border-rotary-blue bg-rotary-blue p-2 text-white md:max-w-4/12 lg:w-2/12"
>
	<div>
		<img
			src={image}
			alt={name}
			class="mx-auto aspect-square w-5/6 rounded-full object-cover {imageOptions}"
		/>
		<div class="rounded-t-md p-2 font-semibold">
			<h2 class="text-xl">{name}</h2>
			<h4 class="text-md text-rotary-gold">{title}</h4>
		</div>
	</div>
	<div class="rounded-b-md p-2">
		<p class="">{desc}</p>
	</div>
</div>
