---
title: "Mandelbrot Set"
excerpt: "Fract'ol<br/><img src='/images/fractol.png'>"
collection: portfolio
---

<script>
	window.addEventListener('keydown', function(e) {
		if(e.keyCode === 32) {
			e.preventDefault();
  		} else if(e.keyCode === 38) {
			e.preventDefault();
		} else if(e.keyCode === 40) {
			e.preventDefault();
		} 
	});
	window.addEventListener('wheel', e => e.preventDefault(), { passive: false });
</script>
<iframe src="https://joonastuomi.fi/web" height=1020 width=1020></iframe>

<kbd>ArrowUp</kbd> or <kbd>ArrowDown</kbd> for vertical movement and <kbd>ArrowLeft</kbd> or <kbd>ArrowRight</kbd> to move sideways. Scroll wheel or pinch to zoom.

[Source code in GitHub](https://github.com/jotuel/fractol)
