<script>
	export let imagePath = '/src/lib/images/gf/Tudorita4.jpg';
	export let strokeColor = '#dd6eb5';

	// Generate a unique pattern id for this instance.
	const patternId = `imagePattern-${Math.random().toString(36).substring(2, 9)}`;
</script>

<svg
	xmlns="http://www.w3.org/2000/svg"
	width="200"
	height="200"
	viewBox="0 0 200 200"
	stroke="#5a0c25"
	stroke-width="2.5"
	stroke-linecap="round"
	stroke-linejoin="round"
>
	<defs>
		<pattern id={patternId} patternUnits="userSpaceOnUse" width="200" height="200">
			<image href={imagePath} x="0" y="0" width="200" height="200" />
		</pattern>
	</defs>
	<path
		fill={`url(#${patternId})`}
		stroke="none"
		transform="translate(-6,-10)"
		d="M61.221 137.275c-25.322-36.037-44.915-53.726 17-86 34.924-22.722 61.12-14.338 71.429 10.49 16.134 22.482 17.873 47.047-1.429 75.51-33.667 34.319-52.75 30.198-87 0Z"
	/>
	<path
		stroke={strokeColor}
		fill="none"
		d="M61.221 137.275c-25.322-36.037-44.915-53.726 17-86 34.924-22.722 61.12-14.338 71.429 10.49 16.134 22.482 17.873 47.047-1.429 75.51-33.667 34.319-52.75 30.198-87 0Z"
	/>
</svg>
