<script>
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
	import hiroshima from '$lib/images/hiroshima.jpg'
</script>



<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>


	

<section>
	<span class="welcome">
		<picture>
			<img src={welcome_fallback} alt="Welcome" />
		</picture>
	</span>
	
	<h1>This man is a monkey!</h1>

	<p>
		<stronger>Brendan Hiroshima</stronger>
	</p>

	<h1>
		<span class="cheese">
			<picture>
				<img src={hiroshima} alt="Welcome" />
			</picture>
		</span>

	</h1>


</section>
<style>
		section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
		}
		.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
		}

		.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
		}

		.cheese {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
		}

</style>





