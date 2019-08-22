# CodeEditor
Blender Addon enhancing Text Editor


* Start and End with right-click in any Text-editor window (it also ends with F8 because when scripting an addon you need to reload with F8 and that is not possible because this addon is a modal operator. So you need F8 + F8 + Right-click>Start_again )

![enter image description here](https://i.stack.imgur.com/lznSW.png)
* When started it adjusts the text-editor to the addon preferences, so you don't have to set line_numbers, syntax_highlight, text_margin etc. every time you open new text-editor window (this is frustating blender behavior, these settings should be global..)

![enter image description here](https://i.stack.imgur.com/UyImH.png)
* It follows blender theme colors. The default ones are bad, so here I give you a good ones so its usable:

![enter image description here](https://i.stack.imgur.com/lwgVx.png)
* It adds a scrollable and clickable code minimap with syntax highlighting, which fades out when window is too small. It is done in another thread and has lazy updating to not lag the text-editor (python is slow for this). It can be disabled in preferences with just setting huge  *Hide Panel threshold* :

![enter image description here](https://i.stack.imgur.com/jOCEX.gif)
* It adds markers to visualize indentation, and it displays the scope of defs and classes (you can see it above in the gif). The scopes could be minimized but this didn't make it into this release because when blender crashes you would loose the hidden code parts (the lines were removed from text and stored in custom property). You can see the toggle icons when you hover over line numbers.
* Autocompletes brackets and "",'':

![enter image description here](https://i.stack.imgur.com/gv4j9.gif)
* Use Alt + C for magic:
* * put things in lists:

![enter image description here](https://i.stack.imgur.com/qIYin.gif)
  * evaluate expressions (it knows pi, e, phi(golden ratio) and g(grav accel)):
  
![enter image description here](https://i.stack.imgur.com/UDf4S.gif)

* stringify words when cursor just after the word:

![enter image description here](https://i.stack.imgur.com/qaNbj.gif)
* Correct <kbd>Home</kbd> and <kbd>Shift</kbd>+<kbd>Home</kbd> behavior. Will move to first letter of line or to the previous indent. <kbd>Alt</kbd>+<kbd>Home</kbd> now moves to the line beginning:

![enter image description here](https://i.stack.imgur.com/oC61Y.gif)
* Make comments with <kbd>Alt</kbd>+<kbd>D</kbd>. (Remove with <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>D</kbd> - this one is not new):

![enter image description here](https://i.stack.imgur.com/JYXRN.gif)
* With multiple text-files it displays tabs to quickly switch between (blender has tabs but does not use them where it should..)

![enter image description here](https://i.stack.imgur.com/mI0na.gif)

Text from:

https://blender.stackexchange.com/questions/31126/workflow-for-developing-add-on-script/31195#31195
