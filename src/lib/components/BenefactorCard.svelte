<script>
	let { title, image, desc } = $props();
</script>

<div
	class="m-8 mx-auto flex max-h-40 max-w-10/12 gap-4 rounded-xl border-2 border-rotary-blue bg-rotary-blue p-2 text-white select-none"
>
	<img src={image} alt={title} class="aspect-square w-40 rounded-lg" />
	<div class="">
		<div class="text-2xl font-bold">
			<h2>{title}</h2>
		</div>
		<div class="">
			<p>{desc}</p>
		</div>
	</div>
</div>
