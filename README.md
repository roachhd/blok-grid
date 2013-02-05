Blok Grid System 
================

######***a work in progress***
  
***Responsive CSS Grid System***

###What is Blok?
---

Blok helps get your websites up and running whilst not restricting you to a strict set of styling rules. 

It uses a custom made responsive grid system for all of the latest browsers and has a fallback for older IE browsers. 

Everything has been organised for you to place your own styles in a manageable fashion.

####Grid
---
The grid system works similar to other grid systems. You have 12 columns for all screen sizes and can select whatever size you like so long as it adds to 12. 

The difference with is framework is you can select different column sizes for each screen size. 

m - Mobile  
t - Tablet  
d - Desktop  

You have push and pull for each device and also have a nth option for when divs will stack. 

If using nth, you need to apply it for all screens that come after so they can cancel out. 

For example, if you use nth in mobile, you must use it for tablet and desktop. If you use it on desktop, then no need to cancel it out. 

####Internet Explorer
---
To make this compatible with older versions of Internet Explorer, I have taken away the responsive nature of the grid. I have created a version with class prefixes to give it a fixed grid layout. you can still nest with this though, as I have also used percentages for this. So the same rules apply, it just won't be responsive. 

There isn't any point in making it responsive for older versions of IE in my opinion because modern mobile devices don't use it. 

If you hae created a website and it doesn't look right in older versions of IE, then you can copy the styles that you have issues with and prefix them with .iex or .ie6, .ie7, .ie8 for more specific targeting. 