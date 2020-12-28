---
layout: page
title: My Projects
subtitle: Things I've made
---

# Kosher.com Print Restyler Bookmarklet

I created this bookmarklet to fix some of the more annoying default styles used by the print CSS that make it difficult to read the page.

## To Install (Desktop):
Drag this to your bookmarks bar:
[Kosher.com Print Restyler](javascript:(function(){let b='https://www.kosher.com/recipe/print/'+window.location.pathname.match(/\d+$/g);if(window.location.href!=b)window.open(b,'_blank');else{document.getElementsByTagName('header')[0].setAttribute('style','background-color:#fff');let a=document.styleSheets[2];a.insertRule('.print{font-size:14pt!important}'),a.insertRule('.recipe-print__directions ol>li{line-height:1.2!important}'),a.insertRule('.recipe-print__callout-meta-description{line-height:1.2!important}'),a.insertRule('.recipe-print__callout-meta-container::before{font-size:0!important;}'),a.insertRule('.recipe-print__callout{font-size:9pt!important}');let c=document.getElementsByTagName('use');for(let d=0;d<c.length;d++)c[d].setAttribute('fill','#000');window.print();}})())

## To Use (Desktop):
* Navigate to a recipe page: e.g. [https://www.kosher.com/recipe/quinoa-stuffed-chicken-2932](https://www.kosher.com/recipe/quinoa-stuffed-chicken-2932)
* Click on the bookmarklet
  * This will open the print page in a new tab
* Click on the bookmarklet again
  * This will apply the nicer style
* Print and Enjoy!

## To Install (iOS: Safari):

* Copy the code below by selecting all and then tapping "Copy" from the context menu:
```javascript
javascript:(function(){let b='https://www.kosher.com/recipe/print/'+window.location.pathname.match(/\d+$/g);if(window.location.href!=b)window.open(b,'_blank');else{document.getElementsByTagName('header')[0].setAttribute('style','background-color:#fff');let a=document.styleSheets[2];a.insertRule('.print{font-size:14pt!important}'),a.insertRule('.recipe-print__directions ol>li{line-height:1.2!important}'),a.insertRule('.recipe-print__callout-meta-description{line-height:1.2!important}'),a.insertRule('.recipe-print__callout-meta-container::before{font-size:0!important;}'),a.insertRule('.recipe-print__callout{font-size:9pt!important}');let c=document.getElementsByTagName('use');for(let d=0;d<c.length;d++)c[d].setAttribute('fill','#000');}})()
```
* Create a bookmark on the current page (don't worry you're gonna change it right away)
	* Share button
	* Add Bookmark
	* Rename the bookmark to something like "Kosher.com Better Print"
* Open Favorites
	* The open book icon between the share icon and the tabs icon
	* Make sure you're on the bookmarks tab (Open book icon at the top left)
	* Tap "Edit" (bottom right)
	* Find the bookmark you just created and tap on it
	* Tap on the 2nd textbox that currently contains a link to this page
	* Tap the little "x" on the far right side to clear the box
	* Tap again to show the context menu and tap on "Paste"
	* Rename the bookmarklet to something like "Kosher.com Better Print"
	* Tap "Done" x3

## To Use (iOS: Safari):
* Navigate to a recipe page: e.g. [https://www.kosher.com/recipe/quinoa-stuffed-chicken-2932](https://www.kosher.com/recipe/quinoa-stuffed-chicken-2932)
* Open your bookmarks and tap on the bookmarklet
  * This will open the print page in a new tab
* Click on the bookmarklet again
  * This will apply the nicer style
* Hold the phone horizontally
	* Open the Share sheet (while the phone is still horizontal)
		* (Share icon is in the top right) 
	* Swipe down until you find "Markup", tap on that (still horizontal)
	* Tap on the Share icon again (upper right corner)
		* Swipe down and find "Print" (you can now re-orient to vertical again)
* Print and Enjoy!