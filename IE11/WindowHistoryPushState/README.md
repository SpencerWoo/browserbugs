# window.history.pushState

https://web.archive.org/web/20171215235533/https://developer.microsoft.com/en-us/microsoft-edge/platform/issues/9383036/

**Reported :** October 17, 2017

**Status :** Reproducible

**Demo :** TODO : add demo link maps.google.com

**Steps To Reproduce :** 

Using IE11

Create HTML with button to call window.history.pushState with random new url-parameter (Or just use the one provided below)
add link-rel favicon
load the html and click the button

 1. Open sample.html
 2. Click the button

**Expected Results :** 

The favicon is visible.

**Actual Results :** 

The favicon disappears on interaction.