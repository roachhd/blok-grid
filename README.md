Blok Framework
==============
  
Responsive CSS Framework
------------------------
  
With Blok Framework, you can easily create a responsive layout with alternative viewport responses.  
  
* Uses sets of blocks
* Set of blocks have alternative folding options
* Has 3 viewport stages
* Golden ratio available
* Works with older IE browsers
* Uses box sizing for less rounding down
* Can easily nest for more layout options
  
This will work in older versions of Internet Explorer. I have decided to not make it responsive in versions of IE 8 and below, since there are no mobile devices running those browsers. Instead, I used a prefix system to evoke a 960 Grid type of system, except with percentages for nesting reasons. The box-sizing and .zero class for nesting works due to a polyfill created by Schepp. Please see the credit at the bottom.
  
When placing blocks, they must be the same type for the responses to work correctly. They must also be repeated by the number, so col_4 is repeated 4 times. Blocks should also be wrapped in a dive with a 'row' class so there are no conflicts with the nth-child property. 
  
Example
  
`<div class="row">`  
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
  
Credit to Schepp for the HTC polyfill for box-sizing in older IE browsers
https://github.com/Schepp/box-sizing-polyfill
  
Enjoy
