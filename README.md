Blok Framework 
==============

######***a work in progress***
  
***Responsive CSS Framework and more!***

###What is Blok?
---

Blok helps get your websites up and running whilst not restricting you to a strict set of styling rules. 

It uses a custom made responsive grid system for all of the latest browsers and has a fallback for older IE browsers. 

Everything has been organised for you to place your own styles in a managable fashion.

###Whats included?
---
* HTML5 Boilerplate <http://html5boilerplate.com>
* Blok Responsive Grid System
* Organised style.css for custom CSS
* Modernizr.js <http://modernizr.com>
* jQuery & jQuery UI <http://jquery.com>
* PIE CSS3 polyfill <http://css3pie.com>
* Boxsizing polyfill <https://github.com/Schepp/box-sizing-polyfill>

***coming soon***

* Responsive plugins built with jQuery
* Plugins will be able to be themed with jQuery Theme Roller
* Helper classes for buttons, tables, images, forms, lists and so on
  
####Features
---
* Covers mobile, tablet and desktop screen sizes
* Mobile first media queries
* Uses box-sizing for reduced rounding down in browsers
* Can easily be edited to use margins instead of box-sizing
* Alternate response options for block groups
* Uses nth-child so blocks can be repeated and respond correctly

####Grid Example
---
When using the responsive grid, make sure to repeat the same block class by the number of the col. So col_4 would usually be repeated 4 times and contained within a row.
  
`<div class="row">`  
    `<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
`</div>`  

If you wanted to create a gallery or have a repeated block, then you can do so by setting one of the blocks as a repeating region and the nth-child will take care of the layout for you. So you could have 8 blocks of col_4_alt_2 and they will still respond without gettings bunched up if one block has a height difference. 

`<div class="row">`  
   	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`   
`</div>` 
  
For the golden ratio, the rules are slightly different. The only have 2 sections. There is the sidebar and the content. If you use a left sidebar, then you need to use the right content. If an alt version is used, then you need to use the corresponding alt version for the other. 
  
`<div class="row">`  
	`<div class="col_golden_ct_l_alt_1"></div>`  
	`<div class="col_golden_sb_r_alt_1"></div>`  
`</div>`  

When you want to create responsive blocks within other blocks to create a more complex response, then you have the option to nest. The blocks will still behave in the same way. You also have the option to take away any box-sizing by adding the .zero class to the parent block

`<div class="row">`  
   	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2 zero">`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`  
	`</div>`  
	`<div class="col_4_alt_2"></div>`  
	`<div class="col_4_alt_2"></div>`     
`</div>`

####Internet Explorer
---
To make this compatible with older versions of Internet Explorer, I have taken away the responsive nature of the grid. I have created a version with class prefixes to give it a fixed grid layout. you can still nest with this though, as I have also used percentages for this. So the same rules apply, it just won't be responsive. 

There isn't any point in making it responsive for older versions of IE in my opinion because modern mobile devices don't use it. 

If you hae created a website and it doesn't look right in older versions of IE, then you can copy the styles that you have issues with and prefix them with .iex or .ie6, .ie7, .ie8 for more specific targeting. 