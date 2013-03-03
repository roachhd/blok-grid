Blok Grid System 
================

######***a work in progress***
  
***Responsive CSS Grid System, Now Built With Compass***

###What is Blok?
---

Blok helps get your websites up and running whilst not restricting you to a strict set of styling rules. 

It uses a custom made responsive grid system for all of the latest browsers and has a fallback for older IE8. 

There is also a custom SCSS/CSS file for setting your styles in.

###Important
---
If you wish to edit the SCSS directly, then you'll need to use it with Compass. By doing this, it offers far more options to you.

####Grid
---
The grid system works similar to other grid systems. You have 12 columns for all screen sizes and can select whatever size you like so long as it adds to 12. 

The difference with this framework is you can select different column sizes for each screen size. 

m - Mobile  
t - Tablet  
d - Desktop  

You have push and pull for each device and also have a nth option for when divs will stack. 

If using nth, you need to apply it for all screens that come after so they can cancel out. 

For example, if you use nth in mobile, you must use it for tablet and desktop. If you use it on desktop, then no need to cancel it out. 

So in other words, cascade your rules as needed.

####Internet Explorer
---
To make this compatible with older versions of Internet Explorer, the responsive nature of the grid has been removed. Blok uses prefixes to give it a fixed grid layout. You can still nest with this though as it also uses percentages. So the same rules apply, it just won't be responsive. 

There isn't any point in making it responsive for older versions of IE because modern mobile devices don't use it. 

If you have created a website and it doesn't look right in older versions of IE, then you can resolve issues with a prefix. You can use .iex to target all browsers or .ie6, .ie7, .ie8 for more specific targeting. If you're aiming to use this grid system for IE6 or IE7, then you'll need to use a box-sizing polyfil. 