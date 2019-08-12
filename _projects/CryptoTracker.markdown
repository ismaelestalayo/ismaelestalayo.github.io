---
layout: post
title: Crypto Tracker
description: a project with a background image
img: /assets/1.jpg
---

<!-- Simple yet powerful crypto-currency tracker for Windows 10. -->

<div class="hero-img">
</div>

<div class="project_descr">
	<img class="project_img" id="gridRow1" src="/assets/cryptotracker/top100_light.png"/>
	<div class="project_explanation">
		<h1>Supports over 100 cryptocurrencies</h1>
		<h5>Keep up to date with Bitcoin, Ethereum, Litecoin... and over a hundred alt-coins, all supporting the main exchanges and currencies all over the world.</h5>
	</div>
</div>

<div class="project_descr">
	<img class="project_img" id="gridRow2" src="/assets/cryptotracker/details_light.png"/>
	<div class="project_explanation">
		<h1>Detailed overview</h1>
		<h5>Compare the prices of the main exchanges, watch the traded volume of the last 24h, read information about the coin...</h5>
	</div>
</div>

<div class="project_descr">
	<img class="project_img" id="gridRow3" src="/assets/cryptotracker/portfolio_light.png"/>
	<div class="project_explanation">
		<h1>Your portfolio at a glance</h1>
		<h5>Keep track of your purchases with the Portfolio section, and stay up to date with
		the News section.</h5>
	</div>
</div>

<div style="">
	<a href="https://www.microsoft.com/store/apps/9n3b47hbvblc?ocid=badge?cid=personal">
		<img src="https://assets.windowsphone.com/85864462-9c82-451e-9355-a3d5f874397a/English_get-it-from-MS_InvariantCulture_Default.png" alt="Get it from Microsoft" class="img-center" style="width: 50%; max-width: 250px; margin-top: 10vw; ">
	</a>
</div>

<script>
	function changeTheme(){
		applyTheme();
	}
	
	function applyTheme(){
		if(window.localStorage.getItem("mode") == "dark"){
			document.getElementById("gridRow1").src = "/assets/cryptotracker/top100_dark.png";
			document.getElementById("gridRow2").src = "/assets/cryptotracker/details_dark.png";
			document.getElementById("gridRow3").src = "/assets/cryptotracker/portfolio_dark.png";
		} else{
			document.getElementById("gridRow1").src = "/assets/cryptotracker/top100_light.png";
			document.getElementById("gridRow2").src = "/assets/cryptotracker/details_light.png";
			document.getElementById("gridRow3").src = "/assets/cryptotracker/portfolio_light.png";
		}
	}
	applyTheme();
</script>