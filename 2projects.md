---
layout: page
title: Projects
permalink: /projects/
---

<div class="projects-hero-container">
	<img id="hero-logo" class="projects-hero-logo" src="/assets/cryptotracker/logo-wide-dark.png">
	<img id="hero-img" class="projects-hero-img" src="https://raw.githubusercontent.com/ismaelestalayo/CryptoTracker/master/Screenshots/promo/Laptop_front_home_light.png"/>
	<div class="project-hero-descr">
		<span>
			<li>Support for more than 100+ crypto-coins including alt-coins.</li>
			<hr>
			<li>Keep track of your purchases with the Portfolio section, and be up to date with the News section.</li>
			<hr>			
			<li>Portfolio and News sections to keep up to date.</li>
		</span>
		<div style="text-align: center; padding: 15px 0">
			<a href="CryptoTracker">Read more...</a>		
		</div>
	</div>
</div>

<script>
	function changeTheme(){
		
		applyTheme();
	}
	
	function applyTheme(){
		if(window.localStorage.getItem("mode") == "dark"){
			document.getElementById("hero-logo").src = "/assets/cryptotracker/logo-wide-light.png";
			document.getElementById("hero-img").src = "https://raw.githubusercontent.com/ismaelestalayo/CryptoTracker/master/Screenshots/promo/Laptop_front_home_dark.png";
		} else{
			document.getElementById("hero-logo").src = "/assets/cryptotracker/logo-wide-dark.png";
			document.getElementById("hero-img").src = "https://raw.githubusercontent.com/ismaelestalayo/CryptoTracker/master/Screenshots/promo/Laptop_front_home_light.png";
		}
	}
	applyTheme();
</script>

<!-- {% for project in site.projects %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endfor %}  -->
