<script>
	export let imagePath = 'images/gf/Tudorita.jpg';
	export let strokeColor = '#dd6eb5';

	// Generate a unique id for this pattern instance.
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
		transform="translate(-5,-5)"
		d="m98.814 56.902.695.338.679-.37c9.809-5.35 18.517-8.146 25.732-8.852 7.222-.707 12.839.684 16.637 3.56 3.762 2.848 5.945 7.309 6.035 13.215.089 5.93-1.942 13.3-6.648 21.752l-44.886 64.923L57.047 86.63c-4.617-10.114-6.627-18.184-6.545-24.28.082-6.055 2.213-10.04 5.817-12.335 3.695-2.352 9.24-3.128 16.52-2.015 7.25 1.108 16.025 4.061 25.975 8.902Z"
	/>
	<path
		fill="none"
		stroke={strokeColor}
		d="m98.814 56.902.695.338.679-.37c9.809-5.35 18.517-8.146 25.732-8.852 7.222-.707 12.839.684 16.637 3.56 3.762 2.848 5.945 7.309 6.035 13.215.089 5.93-1.942 13.3-6.648 21.752l-44.886 64.923L57.047 86.63c-4.617-10.114-6.627-18.184-6.545-24.28.082-6.055 2.213-10.04 5.817-12.335 3.695-2.352 9.24-3.128 16.52-2.015 7.25 1.108 16.025 4.061 25.975 8.902Z"
	/>
</svg>
