---
layout: page
title: My Projects
subtitle: Things I've made
---

# Kosher.com Print Restyler Bookmarklet

I created this bookmarklet to fix some of the more annoying default styles used by the print CSS that make it difficult to read the page.

## To use:

[Drag this to your bookmarks bar](javascript:(function(){let b='https://www.kosher.com/recipe/print/'+window.location.pathname.match(/\d+$/g);if(window.location.href!=b)window.open(b,'_blank');else{document.getElementsByTagName('header')[0].setAttribute('style','background-color:#fff');let a=document.styleSheets[2];a.insertRule('.print{font-size:14pt!important}'),a.insertRule('.recipe-print__directions ol>li{line-height:1.2!important}'),a.insertRule('.recipe-print__callout-meta-description{line-height:1.2!important}'),a.insertRule('.recipe-print__callout-meta-container::before{font-size:0!important;}'),a.insertRule('.recipe-print__callout{font-size:9pt!important}');let c=document.getElementsByTagName('use');for(let d in c)c[d].setAttribute('fill','#000');}})())

To Use:
* Navigate to a recipe page: e.g. [https://www.kosher.com/recipe/quinoa-stuffed-chicken-2932](https://www.kosher.com/recipe/quinoa-stuffed-chicken-2932)
* Click on the bookmarklet
  * This will open the print page in a new tab
* Click on the bookmarklet again
  * This will apply the nicer style
* Enjoy!