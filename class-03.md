#lists

There are lots of occasions when we need to use lists. 
HTML provides us with three different types:

Ordered lists ● are lists where each item in the list is numbered. For example, the list might be a set of steps for a recipe that must be performed in order, or a legal contract where each point needs to be identified by a section number. 
Unordered lists ● are lists that begin with a bullet point (rather than characters that indicate order).
Definition lists ● are made up of a set of terms along with the definitions for each of those terms.

<ol>
The ordered list is created with the <ol> element. 

<li>
Each item in the list is placed between an opening <li> tag and a closing </li> tag. (The li stands for list item.)

Browsers indent lists by default.
Sometimes you may see a type attribute used with the <ol> element to specify the type of numbering (numbers, letters, roman numerals and so on). It is better to use the CSS liststyle-type property 

<ol> 
<li>Chop potatoes into quarters</li> 
<li>Simmer in salted water for 15-20 minutes until tender</li> 
<li>Heat milk, butter and nutmeg</li> 
<li>Drain potatoes and mash</li> 
<li>Mix in the milk mixture</li> 
</ol>


<ul>
The unordered list is created with the <ul> element. 
<li>
Each item in the list is placed between an opening <li> tag and a closing </li> tag. (The li stands for list item.)
Browsers indent lists by default.
Sometimes you may see a type attribute used with the <ul> element to specify the type of bullet point (circles, squares, diamonds and so on). 
It is better to use the CSS list-styletype property

<ul> 
<li>Chop potatoes into quarters</li> 
<li>Simmer in salted water for 15-20 minutes until tender</li> 
<li>Heat milk, butter and nutmeg</li> 
<li>Drain potatoes and mash</li> 
<li>Mix in the milk mixture</li> 
</ul>







# Boxes

By default a box is sized just big enough to hold its contents. To set your own dimensions for a box you can use the height and width properties.
The most popular ways to specify the size of a box are to use pixels, percentages, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size.
When you use percentages, the size of the box is relative to the size of the browser window or, if the box is encased within another box, it is a percentage of the size of the containing box.
When you use ems, the size of the box is based on the size of text within it. Designers have recently started to use percentages and ems more for measurements as they try to create designs that are flexible across devices which have different-sized screens.

Some page designs expand and shrink to fit the size of the user's screen. In such designs, the min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide.
These are very helpful properties to ensure that the content of pages are legible (especially on the smaller screens of handheld devices). For example, you can use the max-width property to ensure that lines of text do not appear too wide within a big browser window and you can use the min-width property to make sure that they do not appear too narrow.
You may find it helpful to try this example out in your browser so that you can see what happens when you increase or decrease the size of the browser window.

<tr> 
<td><img src="images/rhodes.jpg" width="200"    height="100" alt="Fender Rhodes" /></td> 
<td class="description">The Rhodes piano is an    
electro-mechanical piano, invented by Harold    
Rhodes during the fifties and later    
manufactured in a number of models ...</td> 
<td>$1400</td> 
</tr> 


td.description { 
min-width: 450px; 
max-width: 650px; 
text-align: left; 
padding: 5px; 
margin: 0px;
}

In the same way that you might want to limit the width of a box on a page, you may also want to limit the height of it. This is achieved using the min-height and max-height properties.
The example on this page demonstrates these properties in action. It also shows you what happens when the content of the box takes up more space than the size specified for the box. 
If the box is not big enough to hold the content, and the content expands outside the box it can look very messy. To control what happens when there is not enough space for the content of a box, you can use the overflow property, which is discussed on the next page.

<h2>Fender Mustang</h2> 
<p>The Fender Mustang was introduced in 1964 as the   
basis of a major redesign of Fender's ...</p> 
<h2>Fender Stratocaster</h2> 
<p>The Fender Stratocaster or "Strat" is one of the   
most popular electric guitars of all time ...</p> 
<h2>Gibson Les Paul</h2> 
<p>The Gibson Les Paul is a solid body electric   
guitar that was first sold in 1952 ...</p> 



h2, p { 
width: 400px; 
font-size: 90%; 
line-height: 1.2em;
} 
h2 { 
color: #0088dd; 
border-bottom: 1px solid #0088dd;
} 
p { 
min-height: 10px; 
max-height: 30px;
}
