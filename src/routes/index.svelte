<script lang="ts">
	import IllustrationHero from "../../images/illustration-hero.svg";
	import IconMusic from "../../images/icon-music.svg";

	import '../app.css';
</script>

<svelte:head>
	<title>Order Summary Component | Frontend Mentor Challenge</title>
</svelte:head>

<div class="container">
	<div class="component">
		<div class="image">
			<img src={IllustrationHero} alt="Hero">
		</div>
		<div class="info">
			<h1>Order Summary</h1>
			<p class="text-gray">You can now listen to millions of songs, audiobooks, and podcasts on any device anywhere you like!</p>
			<div class="price">
				<div class="price__info">
					<div class="image">
						<img src={IconMusic} alt="IconMusic">
					</div>
					<div class="price__text">
						<h2>Annual Plan</h2>
						<p>$59.99/year</p>
					</div>
				</div>
				<a class="btn btn-normal change" href="/change">Change</a>
			</div>
			<button class="btn btn-primary">Proceed to Payment</button>
			<button class="btn btn-secondary">Cancel Order</button>
		</div>
	</div>
</div>

<style>
	.container {
		position: absolute;
		display: flex;
		align-items: center;
		justify-content: space-evenly;
		flex-direction: column;

		width: 480px;
		margin: 0 auto;
		top: 2rem;
		left: 2rem;
		border-radius: 20px;
	}

	.component {
		width: 500px;
	}

	.image {
		position: relative;
		height: 250px;
		width: 100%;
	}

	img {
		padding: absolute;
		width: 100%;
		height: 100%;
		border-top-left-radius: 20px;
		border-top-right-radius: 20px;
	}

	.info {
		display: flex;
		align-items: center;
		justify-content: space-around;
		flex-direction: column;

		padding: 2rem;
	}

	.info p {
		width: 300px;
		font-size: 1rem;
		font-weight: 500;
		text-align: center;
		line-height: 1.8rem;
	}

	p {
		color: var(--neutral-2);
	}

	.btn {
		padding: 15px 50px;
		border: none;
		color: var(--primary-1);
		border-radius: 8px;
		font-size: 0.9rem;
		cursor: pointer;
	}

	.btn-normal {
		color: var(--primary-2);
		font-size: 1rem;
	}

	.btn-primary {
		background: var(--primary-2);
		font-weight: 700;
	}

	.btn-secondary {
		background: var(--primary-1);
		color: var(--neutral-2);
	}

	.price {
		display: flex;
		align-items: center;
		justify-content: space-evenly;
		width: 50%;
		margin-top: 1rem;
	}

	.price__info {
		width: 90%;
		display: flex;
		align-items: flex-start;
		justify-content: flex-start;
		margin: 0 auto;
	}

	.price__info .image {
		height: 75px;
		width: 75px;
		margin-left: 2rem;
	}

	.price__info img {
		position: absolute;
		width: 75px;
		height: 75px;
	}
	
	.btn-normal {
		font-weight: 700;
	}

	.price__text {
		font-size: 0.6rem;
		text-align: center;
		line-height: 0;
	}

	.price__text h2 {
		font-size: 1.1rem;
	}
	
	.price__text p {
		font-size: 0.9rem;
	}

	@media only screen and (min-width: 1440px) {
		.container {
			width: 100vw;
		}
		
		.component {
			width: 500px;
		}
	}

</style>
