

#Header tags

<h1>This is a Main Heading</h1> 
<h2>This is a Level 2 Heading</h2> 
<h3>This is a Level 3 Heading</h3> 
<h4>This is a Level 4 Heading</h4> 
<h5>This is a Level 5 Heading</h5> 
<h6>This is a Level 6 Heading</h6> 

##Semantic Mark Up

The <em> element that allows you to indicate where emphasis should be placed on selected words and the <blockquote> element which indicates that a block of text is a quotation.
Browsers often display the contents of these elements in a different way. For example, the content of the <em> element is shown in italics, and a <blockquote> is usually indented. But you should not use them to change the way that your text looks; their purpose is to describe the content of your web pages more accurately.
The reason for using these elements is that other programs, such as screen readers or search engines, can use this extra information. For example, the voice of a screen reader may add emphasis to the words inside the <em> element, or a search engine might register that your page features a  quote if you use the <blockquote> element.

The use of the <strong> element indicates that its content has strong importance. For example, the words contained in this element might be said with strong emphasis.
By default, browsers will show the contents of a <strong> element in bold

The <em> element indicates emphasis that subtly changes the meaning of a sentence.
By default browsers will show the contents of an <em> element in italic.

The <blockquote> element is used for longer quotes that take up an entire paragraph. Note how the <p> element is still used inside the <blockquote> element. 
Browsers tend to indent the contents of the <blockquote> element, however you should not use this element just to indent a piece of text — rather you should achieve this effect using CSS. 

The <address> element has quite a specific use: to contain contact details for the author of the page.
It can contain a physical address, but it does not have to. For example, it may also contain a phone number or email address.
Browsers often display the content of the <address> element in italics.
You may also be interested in something called the hCard microformat for adding physical address information to your markup.


###css
The <body> element creates the first box, then the <h1>, <h2>, <p>, <i>, and <a> elements each create their own boxes within it.
Using CSS, you could add a border around any of the boxes, specify its width and height, or add a background color. You could also control text inside a box — for example, its color, size, and the typeface used.


<!DOCTYPE html>
 <html> 
<head>  <title>Introducing CSS</title>  <link href="css/example.css" type="text/css"     rel="stylesheet" /> </head> 
<body>   
<h1>From Garden to Plate</h1>  
<p>A <i>potager</i> is a French term for an     ornamental vegetable or kitchen garden ... </p>  
<h2>What to Plant</h2>  
<p>Plants are chosen as much for their functionality     as for their color and form ... </p> 
</body> 
</html>
body { font-family: Arial, Verdana, sans-serif;} h1, h2 { color: #ee3e80;} p { color: #665544;}
