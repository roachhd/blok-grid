Blok Grid System 
================

######***a work in progress***
  
***Responsive CSS Grid System***

####Grid
---
The grid system works similar to other grid systems. It is set to work with 12 columns as standard, but this can be adjusted via the variables.scss. 

You can select different column sizes for each screen size.

m - Mobile  
t - Tablet  
d - Desktop  

You have push and pull for each device and also have a nth option for when divs may stack. 

If using nth, you need to apply it for all viewports to cancel out nth-child rules that already exist. 

For example, if you use nth in mobile, you must use it for tablet and desktop. If you use it on desktop, then no need to cancel it out. 

You have full control of each element by giving it a set of instructions via classes in the markup.

##Dependencies

Compass for using the SCSS files.
  
  
  
  
  
Enjoy. Share. Fork. 