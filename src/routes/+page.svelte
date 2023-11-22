<script>
	let choices = [{ value: 'DNC' }, { value: 'SCADA' }, { value: 'Training' }, { value: 'Tooling' }];
	let wwy = choices[0].value;

	function tab(i) {
		wwy = choices[i].value;
	}
</script>

<svelte:head>
	<title>Automated</title>
	<meta name="description" content="Automated.sh" />
</svelte:head>

<section>
	<div id="logo">AUTOMATED</div>

	<div id="wwy">
		Solutions for <span id="keyword" bind:innerHTML={wwy} contenteditable="false" />
	</div>
	<p id="topP">
		Lorem ipsum dolor sit amet consectetur adipisicing elit. Nesciunt iure nisi vitae optio deleniti
		dolores, soluta voluptas porro repellat hic distinctio assumenda sed illum. Rerum optio quasi
		eius alias distinctio.
	</p>
	<div>
		<a href="#shop"><div class="btn">Our Products</div></a>
	</div>
	<div>
		<div id="tabs">
			{#each choices as choice, i}
				{#if choice.value == wwy}
					<!-- svelte-ignore missing-declaration -->
					<!-- svelte-ignore a11y-click-events-have-key-events -->
					<!-- svelte-ignore a11y-no-static-element-interactions -->
					<div
						class="selected"
						on:click={() => {
							tab(i);
						}}
					>
						{choice.value}
					</div>
				{:else}
					<!-- svelte-ignore missing-declaration -->
					<!-- svelte-ignore a11y-click-events-have-key-events -->
					<!-- svelte-ignore a11y-no-static-element-interactions -->
					<div
						on:click={() => {
							tab(i);
						}}
					>
						{choice.value}
					</div>
				{/if}
			{/each}
		</div>
		<div id="section">
			{#if wwy == 'DNC'}
				<div>
					<h2>Core 100 IH</h2>
					<div class="sideBySide section">
						<div>
							<h3>Features</h3>
							<ul>
								<li>Remote Uploading</li>
								<p>Upload Files to your machine from anywhere</p>
								<li>Plotter</li>
								<p>Preview your parts before you run them</p>
								<li>Multi USB Support</li>
								<p>use multiple USB drives at the same time</p>
							</ul>
						</div>
						<div class="img">
							<img src="https://placehold.co/400x350" alt="" />
						</div>
					</div>
				</div>
			{:else if wwy == 'Tooling'}
				<div>
					<h2>Tooling</h2>
					<div class="sideBySide section">
						<div>
							<h3>Features</h3>
						</div>
						<div class="img">
							<img src="https://placehold.co/400x350" alt="" />
						</div>
					</div>
				</div>
			{:else if wwy == 'Training'}
				<div>
					<h2>Training Tools</h2>
					<div class="sideBySide section">
						<div>
							<h3>Features</h3>
						</div>
						<div class="img">
							<img src="https://placehold.co/400x350" alt="" />
						</div>
					</div>
				</div>
			{/if}
		</div>
	</div>

	<div id="bullets">
		<div class="bullet cOne">
			<h2>One Time Purchase</h2>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Error atque saepe eum sunt
				perspiciatis ut ullam vero itaque. Harum reprehenderit quia distinctio consequuntur expedita
				accusamus cum cumque. Officia, dolores consequuntur.
			</p>
		</div>
		<div class="bullet cTwo">
			<h2>Continuous Support</h2>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Error atque saepe eum sunt
				perspiciatis ut ullam vero itaque. Harum reprehenderit quia distinctio consequuntur expedita
				accusamus cum cumque. Officia, dolores consequuntur.
			</p>
		</div>
		<div class="bullet cThree">
			<h2>Built to Last</h2>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Error atque saepe eum sunt
				perspiciatis ut ullam vero itaque. Harum reprehenderit quia distinctio consequuntur expedita
				accusamus cum cumque. Officia, dolores consequuntur.
			</p>
		</div>
	</div>
</section>
<div id="shop">
	<h2>Shop</h2>
	<div>
		<h3>Hardware</h3>
		<div class="row scroll">
			<div class="card">
				<img src="https://placehold.co/500x500" alt="" />
				<h4>Core 100 IH</h4>
				<div class="sideBySide">
					<div>$399</div>
					<div class="pur">View More</div>
				</div>
			</div>
			<div class="card">
				<img src="https://placehold.co/500x500" alt="" />
				<h4>TEKO (Headless)</h4>
				<div class="sideBySide">
					<div>$129</div>
					<div class="pur">View More</div>
				</div>
			</div>
			<div class="card">
				<img src="https://placehold.co/500x500" alt="" />
				<h4>Other Product</h4>
				<div class="sideBySide">
					<div>$599</div>
					<div class="pur">View More</div>
				</div>
			</div>
			<div class="card">
				<img src="https://placehold.co/500x500" alt="" />
				<h4>Other Product</h4>
				<div class="sideBySide">
					<div>$599</div>
					<div class="pur">View More</div>
				</div>
			</div>
			<div class="card">
				<img src="https://placehold.co/500x500" alt="" />
				<h4>Other Product</h4>
				<div class="sideBySide">
					<div>$599</div>
					<div class="pur">View More</div>
				</div>
			</div>
			<div class="card">
				<img src="https://placehold.co/500x500" alt="" />
				<h4>Other Product</h4>
				<div class="sideBySide">
					<div>$599</div>
					<div class="pur">View More</div>
				</div>
			</div>
			<div class="card">
				<img src="https://placehold.co/500x500" alt="" />
				<h4>Other Product</h4>
				<div class="sideBySide">
					<div>$599</div>
					<div class="pur">View More</div>
				</div>
			</div>
			<div class="card">
				<img src="https://placehold.co/500x500" alt="" />
				<h4>Other Product</h4>
				<div class="sideBySide">
					<div>$599</div>
					<div class="pur">View More</div>
				</div>
			</div>
		</div>
	</div>
	<div>
		<h3>Software</h3>
		<div class="grid">
			<div class="card2">
				<h4>Online CNC</h4>
				<img src="https://placehold.co/300x150" alt="" />
			</div>
			<div class="card2">
				<h4>Online CNC</h4>
				<img src="https://placehold.co/300x150" alt="" />
			</div>
			<div class="card2">
				<h4>Online CNC</h4>
				<img src="https://placehold.co/300x150" alt="" />
			</div>
		</div>
	</div>
</div>

<style>
	#logo {
		font-size: 30px;
		font-weight: 600;
		z-index: 2;
		width: 100%;
		background: #000;
	}
	#wwy {
		margin: auto;
		max-width: 550px;
		text-align: center;
		font-size: 50px;
		font-weight: 600;
		color: #e6e6e6;
		margin-top: 100px;
	}
	#tabs {
		width: 100%;
		display: flex;
		margin-top: 30px;
	}

	#tabs > div {
		border: 2px solid #fff;
		margin-right: 10px;
		padding: 10px;
		margin-bottom: -2px;
		border-top-left-radius: 5px;
		border-top-right-radius: 5px;
		width: 100px;
		cursor: pointer;
	}

	.selected {
		border-bottom: 2px solid #000 !important;
	}

	#section {
		border: 2px solid #fff;
		border-radius: 10px;
		border-top-left-radius: 0;
		min-height: 500px;
		padding: 0 20px;
	}
	#bullets {
		margin: 150px 0;
	}
	.bullet {
		margin-bottom: 50px;
		background: #ffffff;
		padding: 20px;
		border-radius: 10px;
		color: #000;
	}
	.bullet > h2 {
		font-size: 40px;
		margin-bottom: 0px;
	}
	#topP {
		width: 50%;
		min-width: 400px;
		margin: auto;
		color: #a5a5a5;
		text-align: center;
		margin-top: 50px;
		margin-bottom: 50px;
	}

	.cOne {
		background-color: coral;
	}
	.cTwo {
		background-color: lightseagreen;
	}
	.cThree {
		background-color: lightcoral;
	}
	#keyword {
		color: lightcoral;
	}
	#shop {
		width: calc(100% - 40px);
		height: 100vh;
		height: auto;
		background: #fff;
		/* position: absolute; */
		/* left: 0; */
		color: #000;
		padding: 20px;
		padding-bottom: 100px;
	}
	#shop > h2 {
		font-size: 50px;
		border-bottom: 2px solid #000;
		width: 70%;
	}
	.btn {
		width: 200px;
		height: 40px;
		background-color: fuchsia;
		text-decoration: none;
		color: #fff;
		text-align: center;
		line-height: 40px;
		font-size: 22px;
		margin: auto;
		border-radius: 3px;
		font-weight: 600;
		margin-top: 50px;
		margin-bottom: 50px;
		cursor: pointer;
	}
	a {
		all: unset;
	}
	.card {
		width: 300px;
		padding: 10px;
		border: 2px solid #000;
		margin-right: 50px;
		margin-bottom: 20px;
	}
	.card > img {
		width: 300px;
	}
	.sideBySide {
		display: flex;
		justify-content: space-between;
	}
	.row {
		display: flex;
		overflow-x: auto;
	}
	.pur {
		background: #000;
		color: #fff;
		padding: 4px;
		border-radius: 2px;
	}
	.card2 {
		width: 300px;
		height: 150px;
		position: relative;
		border-radius: 5px;
		margin: 30px;
	}
	.card2 > img {
		position: absolute;
		top: 0;
		left: 0;
		border-radius: 5px;
	}
	.card2 > h4 {
		position: absolute;
		z-index: 2;
		left: 20px;
		top: -5px;
	}
	.grid {
		display: flex;
		flex-wrap: wrap;
		justify-content: left;
	}
	section {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
		overflow-x: hidden;
	}

	@media screen and (max-width: 480px) {
		.grid {
			justify-content: center;
		}
		.section {
			margin: 20px;
			flex-direction: column-reverse;
			align-items: center;
		}
		.img {
			max-width: 90%;
		}
		.img > img {
			max-width: 100%;
		}
	}
</style>
