---
layout: post-minimal

description: Simple yet powerful crypto-currency tracker for Windows 10.
img: /assets/1.jpg
redirect_from: /CryptoTracker
---

<style>
	.hero-blur-background {
		background: url('/assets/cryptotracker/hero-img.png') repeat;
		background-size: cover;
		background-attachment: fixed;
		background-position: center;
		bottom: 0;
		filter: blur(5px);
		height: 100vh;
		left: 0;
		overflow: hidden;
		position: relative;
		position: absolute;
		right: 0;
		top: 0;
		z-index: -1;
		-webkit-mask-image: linear-gradient(0deg, transparent 0%, black 100vh);
	}

	.hero-blur-descr {
		color: white;
		font-size: 32px;
		font-weight: 500;
		text-align: center;
	}

	.hero-blur-descr h1 {
		font-size: 1em;
		font-weight: 400;
		line-height: 1.3em;
		margin: 5vw auto;
		text-align: center;
		width: 80%;
	}

	.hero-blur-descr img {
		margin-left: auto;
		display: block;
		margin: 0 auto;
		width: 75%;
	}

	@media (max-width: 700px) {
		.hero-blur-background {
			background-attachment: scroll;
		}

		.hero-blur-descr img {
			width: 95%;
		}
	}

	@media (prefers-color-scheme: light) {
		.hero-blur-descr h1 {
			filter: drop-shadow(1px 1px 4px #00000088)
		}

		.hero-blur-descr img {
			filter: drop-shadow(1px 1px 4px #00000088)
		}
	}

	@media (prefers-color-scheme: dark) {
		.hero-blur-descr h1 {
			filter: drop-shadow(1px 1px 4px #ffffff88)
		}

		.hero-blur-descr img {
			filter: drop-shadow(1px 1px 4px #ffffff88)
		}
	}
</style>

<div class="site-content" style="position: relative; height: 90vh; width: 100vw;">
	<div class="hero-blur-background">
	</div>
	<div class="hero-blur-descr maxwidth">
		<img id="hero-img"
			src="https://raw.githubusercontent.com/ismaelestalayo/CryptoTracker/master/CryptoTracker/Assets/Wide-D.png">
		<h1>Minimal yet powerful cryptocurrency tracker.</h1>
	</div>
</div>

<div class="site-content maxwidth">
	<div class="project-descr">
		<picture class="project_img">
			<source srcset="/assets/cryptotracker/top100D.png" media="(prefers-color-scheme: dark)">
			<img src="/assets/cryptotracker/top100L.png" loading="lazy">
		</picture>
		<div class="project_explanation">
			<h1>Supports over 300 cryptocurrencies</h1>
			<h5>Keep up to date with over three hundred alt-coins, all of them supporting the main exchanges and
				currencies from all over the world.</h5>
		</div>
	</div>
	<div class="project-descr">
		<picture class="project_img">
			<source srcset="/assets/cryptotracker/detailsD.png" media="(prefers-color-scheme: dark)">
			<img src="/assets/cryptotracker/detailsL.png" loading="lazy">
		</picture>
		<div class="project_explanation">
			<h1>Detailed overview</h1>
			<h5>Historic prices, insightful information, global and coin stats, volume... and all from a single page.
			</h5>
		</div>
	</div>
	<div class="project-descr">
		<picture class="project_img">
			<source srcset="/assets/cryptotracker/portfolioChartD.png" media="(prefers-color-scheme: dark)">
			<img src="/assets/cryptotracker/portfolioChartL.png" loading="lazy">
		</picture>
		<div class="project_explanation">
			<h1>Your portfolio at a glance</h1>
			<h5>Keep track of all your purchases with a <span class="highlighted">clear overview of your
					portfolio</span>,
				analyze its trend with the
				historic graph and see the total profits/losses of each purchase.</h5>
		</div>
	</div>
	<div class="project-descr">
		<picture class="project_img">
			<source srcset="/assets/cryptotracker/portfolioDetailsD.png" media="(prefers-color-scheme: dark)">
			<img src="/assets/cryptotracker/portfolioDetailsL.png" loading="lazy">
		</picture>
		<div class="project_explanation">
			<h1>Detailed portfolio manager</h1>
			<h5>Examine the performance of your investments one by one with a detailed view, and save a backup to the
				cloud to have all your devices synced.</h5>
		</div>
	</div>
	<div class="project-descr">
		<picture class="project_img">
			<source srcset="/assets/cryptotracker/newsD.png" media="(prefers-color-scheme: dark)">
			<img src="/assets/cryptotracker/newsL.png" loading="lazy">
		</picture>
		<div class="project_explanation">
			<h1>The latest news</h1>
			<h5>Stay up to date with the latest news of the crypto world, and filter them to the tags that matter to you
				the most.</h5>
		</div>
	</div>
</div>

<a href='//www.microsoft.com/store/apps/9n3b47hbvblc?cid=storebadge&ocid=badge'><img
		src='images/English_get-it-from-MS.png' alt='English badge' class="img-center"
		style='width: 284px; height: 104px; margin-top: 3vw;' /></a>


<script>
	function lightTheme() {
		document.getElementById("gridRow1").src = "/assets/cryptotracker/top100_light.png";
		document.getElementById("gridRow3").src = "/assets/cryptotracker/portfolio_light.png";
		document.getElementById("hero-img").src = "https://raw.githubusercontent.com/ismaelestalayo/CryptoTracker/master/CryptoTracker/Assets/Wide-D.png";
	}
	function darkTheme() {
		document.getElementById("gridRow1").src = "/assets/cryptotracker/top100_dark.png";
		document.getElementById("gridRow3").src = "/assets/cryptotracker/portfolio_dark.png";
		document.getElementById("hero-img").src = "https://raw.githubusercontent.com/ismaelestalayo/CryptoTracker/master/CryptoTracker/Assets/Wide-L.png";
	}
</script>