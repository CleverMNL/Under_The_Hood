https://youtu.be/OXGznpKZ_sA?si=ccj_8JvWmI4mfRft

The only resource needed really.

Projects using CSS will be under the folder path:
##### Notebook > Learning_Projects > CSS_Projects > "Project_Name"

---
Cascading Style Sheets is perfectly named because it is a styling format of keywords/syntax that is applied to a page alongside html to make it appear in a manner which we want to make it appear. The cascading part comes from the fact that the rule sets (the appearance we want to apply to it) are taken in a trickle down manner, a top-down rank where certain rules can be overwritten by a rule set after. 

The video lecture also does a cool job at explaining how some rgb values are written. To summarize: black is the absence of color so it is written as six zeros (000000), white on the other hand is written as six F's for full (FFFFFF) from this we can take that full red would be FF0000, full green would be 00FF00, and blue is 0000FF. Every other color (not every single one but a lot) derives from this hexadecimal representation. 

A shorthand was made for representing some hexadecimals using pairwise notation simply meaning that each pair could be written shorter. Black can be 000 because each zero represents the pair of 00, 00, 00. or white can be FFF for FF, FF, FF. 

---
The lecture also introduces a great resource to check for color contrast in order to be more legible and goes well into color theory; [[Color Theory applications]] includes the resource under contrast checker.

Here are some hexadecimal resources to find hexes that are nice:
[HTML Color Codes 🎨 (html-color.codes)](https://html-color.codes/)

[HTML Color Codes](https://htmlcolorcodes.com/)

[Web Colors (rapidtables.com)](https://www.rapidtables.com/web/color/index.html)

The ultimate colors guide for CSS:
[Colors Tutorial (w3schools.com)](https://www.w3schools.com/colors/default.asp)

---
##### Units and sizes:

Using pixels is the standard to be used. I personally like using % but it is good to know that projects will be using flexbox and grid to be more responsive than manually setting units/size. The fact that Dave (Gray)  understands this and makes reasonable assumptions of when we would use manual unit fixing and taking that form the user preference settings is why I enjoy the lecture. 

The resource used by Dave was this one:
[CSS values and units - Learn web development | MDN (mozilla.org)](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units)

Percentage is only relative to the parent element. Meaning that if I use a div box and change the percentage of the width of the paragraph in the div, the size of 100% would only be relative to the div and not the entire page. 

The lecture also does a great job of explaining REM and EM size units and basically shows that the one letter difference can make drastic changes to the sizing of an element because one is relative to the root size. 

One last point made that was only stated in passing but I see it as helpful was using the inspect elements feature of browser. Using a right click for Windows you can click inspect and see the HTML, CSS, and maybe JS used on a site. He mentioned using it only to check your progress and box model but this can be done to any website and you can see all its HTML structure and CSS applied. This developer tool can be set to console, element, and other modes which are helpful to explore. 

---
##### The box model:

Pretty much all html and css is a box. A div is a box, an article is a box, a section is a bow, etc. CSS works within those boxes.