Blok Grid System 
================

######***a work in progress***
  
***Responsive CSS Grid System***

###What is Blok?
---

Blok helps get your websites up and running whilst not restricting you to a strict set of styling rules. 

It uses a custom made responsive grid system for all of the latest browsers and has a fallback for older IE8. 

There is also a custom SCSS/CSS files for setting your styles in.

* responsive or adaptive
* only one distributed grid so it's easy to edit
* can select between 1 and 24 columns
* can set a custom gutter size
* easy to customise to suit your needs


###Important
---
If you wish to edit the SCSS directly, then you should use it with Compass. It is lightly integrated, so is easy enough to adjust for use without it. 

####Grid
---
The grid system works similar to other grid systems. It is set to work with 12 columns as standard, but this can be adjusted via the variables.scss. 

The difference with this framework is you can select different column sizes for each screen size. [Example](http://blokgrid.co.uk/?custom_type=how-the-grid-works)

m - Mobile  
t - Tablet  
d - Desktop  

You have push and pull for each device and also have a nth option for when divs will stack. 

If using nth, you need to apply it for all viewports to cancel out nth-child rules that already exist. 

For example, if you use nth in mobile, you must use it for tablet and desktop. If you use it on desktop, then no need to cancel it out. 

You have full control of each element by giving it a set of instructions via classes in the markup.

####Internet Explorer
---
The is compatible with IE8.  

You can use a polyfill for making box-sizing work with older versions of IE, but that can conflict with another polyfill like PIE.htc. 

Anyway… Enjoy. Share. Fork. 

Jordan.