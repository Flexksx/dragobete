<script>
	export let imagePath = '/src/lib/images/your-image.jpg';
	// Generate a unique pattern id to avoid conflicts if multiple instances are rendered
	const patternId = `imagePattern-${Math.random().toString(36).substring(2, 9)}`;
</script>

<svg
	xmlns="http://www.w3.org/2000/svg"
	version="1.1"
	xmlns:xlink="http://www.w3.org/1999/xlink"
	xmlns:svgjs="http://svgjs.dev/svgjs"
	viewBox="0 0 800 800"
>
	<defs>
		<pattern id={patternId} patternUnits="userSpaceOnUse" width="800" height="800">
			<image href={imagePath} x="0" y="0" width="800" height="800" />
		</pattern>
	</defs>
	<g
		fill={`url(#${patternId})`}
		stroke-width="6"
		stroke="#dd6eb5"
		id="cloud"
		data-darkreader-inline-stroke=""
		style="--darkreader-inline-stroke: var(--darkreader-text-b517a7, #e953dc);"
	>
		<path
			d="M 124.85029940119762 298.50299401197606 A 50 50 0 1 1 200 200 A 50 50 0 1 1 314.07185628742513 214.37125748502996 A 50 50 0 1 1 554.7904191616765 228.14371257485033 A 50 50 0 1 1 643.1137578358905 317.3652848112369 A 50 50 0 1 1 480.53892215568857 473.65269461077844 A 50 50 0 1 1 298.50299401197606 478.7425149700598 A 50 50 0 1 1 124.85029940119762 298.50299401197606 Z"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
	</g>
</svg>
