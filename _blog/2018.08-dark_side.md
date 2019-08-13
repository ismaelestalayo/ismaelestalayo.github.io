---
layout: post
title: Crypto Tracker
description: Simple yet powerful crypto-currency tracker for Windows 10.
img: /assets/1.jpg
visible: false
---


```HTML
<script>
	document.addEventListener('DOMContentLoaded', (event) => {
        ((localStorage.getItem('mode') || 'dark') === 'dark') ? document.querySelector('body').classList.add('dark') : document.querySelector('body').classList.remove('dark')
    })
</script>
```


```HTML
<a onclick="localStorage.setItem('mode', (localStorage.getItem('mode') || 'dark') === 'dark' ? 'light' : 'dark'); localStorage.getItem('mode') === 'dark' ? document.querySelector('body').classList.add('dark') : document.querySelector('body').classList.remove('dark'); changeTheme()">
	<img src="/assets/profile1.jpg" />
</a>
```

While the CSS media query `prefers-color-scheme: light` is really handy for quick color changes to the styles, there's no option 

```HTML
<script>
	const darkModeMediaQuery = window.matchMedia('(prefers-color-scheme: dark)');
  	darkModeMediaQuery.addListener((e) => {
    	const darkModeOn = e.matches;
		// this functions are to be created on each HTML that needs to make changes that CSS can't
    	darkModeOn ? darkTheme() : lightTheme();
  });
</script>	
```