Blok Framework
==============
  
Responsive CSS Framework
------------------------
  
With Blok Framework, you can easily create a responsive layout with alternative viewport responses.  
  
* Uses sets of blocks
* Set of blocks have alternative folding options
* Has 3 viewport stages
* Golden ratio available
* Works with IE8 (needs a polyfill for below)
* Uses box sizing for less rounding down
* Can easily nest for more layout options
  

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
  
Enjoy
