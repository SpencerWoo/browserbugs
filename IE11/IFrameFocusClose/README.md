# IFrame Open / Set Focus / Close

https://developer.microsoft.com/en-us/microsoft-edge/platform/issues/872182/

**Reported :** September 24, 2014

**Status :** Not Reproducible

**Demo :** https://spencerwoo.github.io/bugs/demo1.html

**Steps To Reproduce :** 

Using Windows 10

Using IE11

 1. Open page1.html.  Can type text in input or textarea
 2. Click button "Open page2.html"
 3. Type text into page2's input field
 4. Click button "Close page2.html"
 5. Click on input or text area to type

**Expected Results :** 

The text can be modified.  Typing is possible.

**Actual Results :** 

The text cannot be modified.  Typing is not possible.