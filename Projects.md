---
layout: page
title: My Projects
subtitle: Things I've made
---

# Kosher.com Print Restyler Bookmarklet

I created this bookmarklet to fix some of the more annoying default styles used by the print CSS that make it difficult to read the page.

### To Install (Desktop):
Simply drag this to your bookmarks bar:
[Kosher.com Print Restyler](javascript:(function(){let b='https://www.kosher.com/recipe/print/'+window.location.pathname.match(/\d+$/g);if(window.location.href!=b)window.open(b,'_blank');else{document.getElementsByTagName('header')[0].setAttribute('style','background-color:#fff');let a=document.styleSheets[2];a.insertRule('.print{font-size:14pt!important}'),a.insertRule('.recipe-print__directions ol>li{line-height:1.2!important}'),a.insertRule('.recipe-print__callout-meta-description{line-height:1.2!important}'),a.insertRule('.recipe-print__callout-meta-container::before{font-size:0!important;}'),a.insertRule('.recipe-print__callout{font-size:9pt!important}');let c=document.getElementsByTagName('use');for(let d=0;d<c.length;d++)c[d].setAttribute('fill','#7a087a');window.print();}})())

### To Use (Desktop):
1. Navigate to a recipe page: e.g. [https://www.kosher.com/recipe/quinoa-stuffed-chicken-2932](https://www.kosher.com/recipe/quinoa-stuffed-chicken-2932)
2. Click on the bookmarklet
  1. This will open the print page in a new tab
3. Click on the bookmarklet again
  1. This will apply the nicer style
4. Print and Enjoy!

## Install on Mobile
### iOS - Safari:

1. Copy the code below by selecting all and then tapping "Copy" from the context menu:
```javascript
javascript:(function(){let b='https://www.kosher.com/recipe/print/'+window.location.pathname.match(/\d+$/g);if(window.location.href!=b)window.open(b,'_blank');else{document.getElementsByTagName('header')[0].setAttribute('style','background-color:#fff');let a=document.styleSheets[2];a.insertRule('.print{font-size:14pt!important}'),a.insertRule('.recipe-print__directions ol>li{line-height:1.2!important}'),a.insertRule('.recipe-print__callout-meta-description{line-height:1.2!important}'),a.insertRule('.recipe-print__callout-meta-container::before{font-size:0!important;}'),a.insertRule('.recipe-print__callout{font-size:9pt!important}');let c=document.getElementsByTagName('use');for(let d=0;d<c.length;d++)c[d].setAttribute('fill','#7a087a');}})()
```
2. Create a bookmark on the current page (don't worry you're gonna change it right away)
	1. Tap on the share icon
	2. Scroll down and tap on "Add Bookmark" or "Add to Favorites"
	3. Rename the bookmark to something like "Kosher.com Better Print"
3. Open Favorites
	1. The open book icon between the share icon and the tabs icon
4. Make sure you're on the bookmarks tab (Open book icon at the top left)
	1. Tap "Edit" (bottom right)
	2. Find the bookmark you just created and tap on it
	3. Tap on the 2nd textbox that currently contains a link to this page
	4. Tap the little "x" on the far right side to clear the box
	5. Tap again to show the context menu and tap on "Paste"
	6. Rename the bookmarklet to something like "Kosher.com Better Print" if you haven't already
	7. Tap "Done" x3

## Use on Mobile
### iOS - Safari:
1. Navigate to a recipe page: e.g. [https://www.kosher.com/recipe/quinoa-stuffed-chicken-2932](https://www.kosher.com/recipe/quinoa-stuffed-chicken-2932)
2. Open your bookmarks and tap on the bookmarklet
  1. This will open the print page in a new tab
3. Click on the bookmarklet again
  1. This will apply the nicer style
4. Hold the phone horizontally
	1. Open the Share sheet (while the phone is still horizontal)
		1. (Share icon is in the top right) 
	2. Swipe down until you find "Markup", tap on that (still horizontal)
	3. Tap on the Markup Edit icon in the upper right corner, to turn off edit
		1. Turn the phone vertical again, and tap on the Share icon in the bottom left corner
		2. Swipe down and find "Print"
5. Print and Enjoy!