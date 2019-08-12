---
layout: post-minimal

description: Simple yet powerful crypto-currency tracker for Windows 10.
img: /assets/1.jpg
---

<style>
.div1{
	background: url('/assets/cryptotracker/hero-img.png') repeat;
	background-size: cover;
	background-attachment: fixed;
	background-position: center;
	overflow: hidden;
	z-index: -1;
	position: relative;
	height: 100vh;
	filter: blur(2px);
	position: absolute;
	left: 0;
	right: 0;
	bottom: 0;
	top: 0;"
}
.div2{
	text-align: center;
	font-size: 32px;
	color: white;
	font-weight: 500;
}
.div2 h1{
	font-size: 7vw;
	line-height: 1.3em;
	filter: drop-shadow(1px 1px 4px black);
}
.div2 img{
	margin-left: auto;
	filter: drop-shadow(1px 1px 4px black);
	display: block;
	margin: auto;
	margin-top: 25vh;
	width: 90%;
}
</style>

<div class="page-content" style="position: relative; height: 100vh; width: 100vw;">
	<div class="div1">
	</div>
	<div class="div2">
		<img src="/assets/cryptotracker/logo-wide-light.png"> <h1>Simple yet powerful crypto-currency tracker for Windows 10.</h1>
	</div>
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