
There's a fork of a Cameron's resume project https://github.com/udacity/frontend-nanodegree-mobile-portfolio
with performance optimization for it.

You can check the work using this link:
http://sergey-vaysman.github.io/fewdn-project4-website-optimization

What's changed in index.html:
* Added a media query for print.css.
* Google Analytics js invokes async. Also added an analytics profile id for its correct work.
* Change to invoke minified version of perfmatters.js
* Any image gets without additionally scaling it after receiving.
* Any image is compressed.
* Created a minified version of font.css. This css is inlined into html file.
* Created a minified version of style.css. This css is also inlined into html file.
Also the same changes are added for projects pages.

What's changed in main.js:
* Use getElementsById and getElementsByClassName instead of querySelector and querySelectorAll respectively.
* Get constant object at once, outside loops.
* Use image compressing and avoid image scalling.
* Decrease the number of objects depending on screen resolution.
* Avoid Layout step by using style transform instead of left position.
