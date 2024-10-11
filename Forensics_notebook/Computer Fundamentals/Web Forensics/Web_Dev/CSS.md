https://youtu.be/OXGznpKZ_sA?si=ccj_8JvWmI4mfRft

The only resource needed really.

Projects using CSS will be under the folder path:
##### Notebook > Learning_Projects > CSS_Projects > "Project_Name"

---
Cascading Style Sheets is perfectly named because it is a styling format of keywords/syntax that is applied to a page alongside html to make it appear in a manner which we want to make it appear. The cascading part comes from the fact that the rule sets (the appearance we want to apply to it) are taken in a trickle down manner, a top-down rank where certain rules can be overwritten by a rule set after. 
 
The video lecture also does a cool job at explaining how some RGB values are written. To summarize: black is the absence of color so it is written as six zeros (000000), white on the other hand is written as six F's for full (FFFFFF) from this we can take that full red would be FF0000, full green would be 00FF00, and blue is 0000FF. Every other color (not every single one but a lot) derives from this hexadecimal representation. 

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

Pretty much all html and CSS is a box. A div is a box, an article is a box, a section is a box, etc. CSS works within those boxes.  Padding is interesting an goes (top, right, bottom, left) and it can assume things for you. For example, if you wanted padding on top of a div box of 15px with a bottom padding of 10px and a left and right padding of 14px, it would be written as (padding: 15px 14px 10px). Here the renderer assumes for you that both left and right padding are to be 14px. Using dashes is a great way to learn about the box model or when using grid. (use border-style: dashed). For any questions about HTML and CSS, one of the best resources is [W3Schools Online Web Tutorials](https://www.w3schools.com/)

---
##### Typography:

This is an entire field of study that looks at how a character is arranged and presented (it deals with the visuals of text). It can go into details on letter size, letter spacing, centering, etc. Some other things that can make you think about what typography is are italics, or underlines. They are things that affect how a piece of text looks like/is read. It is extremely helpful to understand. 

As I searched for more resources to learn about Typography, I saw a rabbit hole (I didn't realize people were so obsessed with the appearance of text), and stuck my head in for a peek. 

[25 Free Typography Resources to Inspire Your Designs | Domestika](https://www.domestika.org/en/blog/10571-25-free-typography-resources-to-inspire-your-designs)

[20 great free resources for learning typography | Creative Bloq](https://www.creativebloq.com/features/20-great-free-resources-for-learning-typography)

[The 5 Best Free Online Typography Courses (makeuseof.com)](https://www.makeuseof.com/best-free-online-typography-courses/)

These are only a dip and they feel overwhelming as people have dedicated decades of work into this field alone and feel passionate as "writers". 

---
##### List stuff:

There is a lot of interesting things that can be done with lists in HTML and CSS. Images can be added to bullet points, roman numerals can be set at different beginning numbers, spaces can be added for clarity, points can be hidden entirely, etc. List- "action" such as -style, -height, -style-image, -style-position, -style-type. Setting type to none would remove the bullet point.  

You can even add specific words as the bullet points by using the "content" property. 
Exp. 
    content: "The amount moved: "; 
    would display a list item like so: 
			The amount moved: 345 dollars

---
##### Display property: 

This impacts the display of an item by creating its own space and explicitly defining its appearance. display: inline-block is a type of property and value. 

A thing to look at just to help streamline workflow would be to **learn about Emmet Abbreviation** means because once it is learned, a lot of writing can be avoided. 

---
##### Working with floating boxes:

A pretty cool feature to explore as it adds readability to some pages but not to be overused. Limit use to Letters or a small image that aids the words. Floats are always outside the flow of a page and add tedious reworking and fixing since other boxes will not directly interact with the float box. There are simple workarounds but always recall graceful degradation for backward compatibility meaning, we still want it to work with older versions of HTML and CSS since not all browsers accept them. 

--- 
##### Using Columns:

These are more based on appearance and do not have to be used if there are better alternatives. One of the more practical takeaways from this section is actually on fonts and Unicode that goes into HTML or CSS and how to use it to get typographical effects. For example making quotations like:
		"What is evil, that which springs from weakness." **-** Friedrich Nietchze 

---
##### Position just makes sense:

Keeping the page sections separate is a fun feature and adding pure functionality is the best feature which will help and avoid any unnecessary code using JS. 

---
##### Using Flexbox and Using Grid:

Almost always in use somewhere. I enjoy it over grid but Kevin Powell mentioned there are tradeoff for using either, grid is better at somethings and flexbox is better at others (or less worse). Shows a visual explanation of how flexbox looks like. 