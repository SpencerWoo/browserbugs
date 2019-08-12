# Parent Container Focus

https://support.microsoft.com/en-us/help/4088339/parent-container-can-not-get-focus-if-display-inline-block-style-used

**Reported :** September 24, 2014

**Status :** Reproducible

**Demo :** https://spencerwoo.github.io/bugs/demo1.html

**Steps To Reproduce :** 

If the value of the CSS display property is set to inline-block, the focus may go to a SPAN or DIV element in a DIV container instead of to a parent container.

Using IE11

 1. Open page1.html.
 2. Select the image.
 3. Hit the left arrow key.

**Expected Results :** 

The cursor is moves and maintains focus.

**Actual Results :** 

The cursor loses focus.

**Resolution :**
Open Registry Editor.
Locate and then click the following registry subkey:

HKEY_CURRENT_USER\SOFTWARE\Microsoft\Internet Explorer\Main\FeatureControl
On the Edit menu, point to New, and then click Key.
Type FEATURE_SPAN_DIV_FOCUS_COMPAT, and then press Enter.
Locate and then click the following new registry subkey:

HKEY_CURRENT_USER\SOFTWARE\Microsoft\Internet Explorer\Main\FeatureControl\FEATURE_SPAN_DIV_FOCUS_COMPAT
On the Edit menu, point to New, and then click the DWORD (32 bit) value.
Type iexplore.exe, and then press Enter.
On the Edit menu, click Modify.
In the Value data box, type 1.
Exit Registry Editor.