<script>
	import jake from '$lib/images/jake.gif';
	import android from '$lib/images/android.gif';
	import apple from '$lib/images/apple.gif';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="My phone rings, dings, and things" />
</svelte:head>

<div class="container">
	<h1>MY RINGS AND DINGS</h1>
	<div class="flex">
		<div class="cards">
			<a target="_blank" href="https://drive.google.com/drive/folders/1PayBBzTE8n_sFuBD5MBt1c-RrvQJJ0Jm">
			<h2>Main Content</h2>
		
			<img src={jake} alt="Jake" />
			</a>
		</div>
		<div class="cards">
		<a href="/android">
			<h2>Android</h2>
			<img src={android} alt="Android" />
			
		</a>
	</div>
	<div class="cards">
		<a href="/iphone">
			<h2>iPhone</h2>
			<img src={apple} alt="iphone" />
			
		</a>
	</div>
</div>
	
<div class="grid">
	<p>
		Throughout the course of my life, trying to get my ringtones the way I wanted often left me simmering with rage. There is already enough in life to bring frustration and rage, and ringtones should not be one of them. I created this site to one, make it easier for people to enjoy regardless of the color of your phone's skin or place of birth. Reason number two is the need to elicit smiles, laughs, and bobbing of heads all around the globe. (Search "Bobbing" to bob head). 
	</p>
	<p>
		Some people are saying I am one of the true visionaries of our time. I don't say that, but some people do. I walk into a room, and people say, "You are a true visionary, Mr. President. One of the greatest the world has ever seen. Nobody does visions like you do, Sir. And you're a stable genius."
	</p>
</div>
</div>



<style>
	.container {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.4;
	}
h1, h2 {
	margin: 0;
}
	h1 {
		width: 100%;
	}

	h2 
	{
		font-size: 2em;
		font-weight: 400;
		font-style: bold;
		width: 100%;
	}
.grid {
	display:grid;
	grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
	gap: 2rem

}

p {
	font-size: 1.5em;
	font-weight: 300;
	font-style: italic;
	width: 100%;
}
	.flex{
			display: flex;
			justify-content: space-between; 
			margin: 1em 3em 1em 3em;
	}
	
	.cards{
		/* display: flex; */
		/* flex-direction: column; */
		width: 30%;
		border: 1px solid black;
		border-radius: 5px;
		padding: 10px;
		margin: 10px;
	}

	.cards a{
		text-decoration: none;
		color: black;
	}

	.cards a img{
		width: 100%;
	}
</style>
