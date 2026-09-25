<script>
	const { text, link, additionalClasses = '' } = $props();
</script>

<a href={link}>
	<button
		class="mx-1.5 cursor-pointer rounded-md px-4 py-2 font-semibold text-white duration-200 select-none hover:bg-white hover:text-rotary-blue {additionalClasses}"
		>{text}</button
	>
</a>
