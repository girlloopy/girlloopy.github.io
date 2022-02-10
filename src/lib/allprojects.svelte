<script>
	// add file names here
	const images = [
		'favicon.png',
		'wm crim dell.jpg',
		'wm fall.jpg',
		'favicon.png',
		'wm crim dell.jpg',
		'wm fall.jpg',
		'favicon.png',
		'wm crim dell.jpg',
		'wm fall.jpg',
		'favicon.png',
		'wm crim dell.jpg',
		'wm fall.jpg',
		'favicon.png',
		'wm crim dell.jpg',
		'wm fall.jpg'
	];
</script>

<div class="parent">
	<table>
		{#each images as img}
			<tr class="row">
				<td class><img src="static/{img}" alt="test" /> </td>
				<td>
					Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has
					been the industry's standard dummy text ever since the 1500s, when an unknown printer took
					a galley of type and scrambled it to make a type specimen book. It has survived not only
					five centuries, but also the leap into electronic typesetting, remaining essentially
					unchanged. It was popularised in the 1960s with the release of Letraset sheets containing
					Lorem Ipsum passages, and more recently with desktop publishing software like Aldus
					PageMaker including versions of Lorem Ipsum.
				</td>
			</tr>
		{/each}
	</table>
</div>

<style>
	/* change the height for each  */
	tr {
		scroll-snap-align: start;
		height: 100vh;
	}

	td {
		height: 50%;
		width: 50%;
		position: relative;
		justify-content: center;
		text-align: center;
		padding: 20px;
		background-color: black;
	}

	img {
		height: 500px;
		width: 500px;
	}

	.parent {
		overflow: auto;
		scroll-snap-points-y: repeat(100vh);
		scroll-snap-type: y mandatory;

		background-color: pink;
		height: 100vh;
		width: 100vw;
		border-radius: 6px;
		padding: 1rem;
	}
	/* custom scrollbar */
	::-webkit-scrollbar {
		width: 20px;
	}

	::-webkit-scrollbar-track {
		background-color: transparent;
	}

	::-webkit-scrollbar-thumb {
		background-color: pink;
		border-radius: 20px;
		border: 6px solid transparent;
		background-clip: content-box;
	}

	::-webkit-scrollbar-thumb:hover {
		background-color: #a8bbbf;
	}
</style>
