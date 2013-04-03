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
* gutters can be margins or padding
* can select between 1 and 24 columns
* can set a custom gutter size
* easy to customise to suit your needs


###Important
---
If you wish to edit the SCSS directly, then you'll need to use it with Compass. By doing this, it offers far more options to you.

Because Compass has not been heavily used, it is easy to remove and use without.

####Grid
---
The grid system works similar to other grid systems. It is set to work with 12 columns as standard, but this can be adjusted via the settings.scss. 

The difference with this framework is you can select different column sizes for each screen size. 

m - Mobile  
w - Wide (Landscape)  
t - Tablet  
d - Desktop  
s - Super Size Monitor

You have push and pull for each device and also have a nth option for when divs will stack. 

If using nth, you need to apply it for all screens that come after so they can cancel out. 

For example, if you use nth in mobile, you must use it for tablet and desktop. If you use it on desktop, then no need to cancel it out. 

You have full control of each element by giving it a set of instructions via classes in the markup.

####Internet Explorer
---
The is compatible with older versions of IE. It was using box-sizing and still can do. You can even use margins and box-sizing, however this will only make it compatible with EI8 and thats even depending on the users settings. 

You can uncomment the box-sizing include in the gridMobile.scss if you wish to use it. 

You can use a polyfill for this and make it work on older versions of IE, but that can conflict with another polyfill like PIE.htc. 

Anyway… Enjoy. Share. Fork. 

Jordan.

####Updates
---
03/04/13

* removed box-sizing and kept it as an option. 
* added margins to the columns
* margin size can be specified from the settings.scss
* added column number to the settings.scss so you can use between 1 and 24 columns
* added nth:child selectors for the extra column amounts.
* added another 2 breakpoints for landscape mobile and super size desktop
* only one grid.scss to edit and it is then distributed to the different grids needed using variables
* separated the custom scss for better oranisation
* added margin and padding helper classes to the grid
* included selectivizr for nth:child classes to work in older IE browsers