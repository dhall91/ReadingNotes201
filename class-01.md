#how PeoPLe access the weB

People access websites using software called a web browser. Popular examples include Firefox, Internet Explorer, Safari, Chrome, and Opera.
In order to view a web page, users might type a web address into their browser, follow a link from another site, or use a bookmark.
Software manufacturers regularly release new versions of browsers with new features and supporting new additions to languages. It is important, however, to remember that many computer owners will not be running the latest versions of these browsers. Therefore you cannot rely on all visitors to your site being able to use the latest functionality offered in all browsers.


When you ask your browser for a web page, the request is sent across the Internet to a special computer known as a web server which hosts the website.
Web servers are special computers that are constantly connected to the Internet, and are optimized to send web pages out to people who request them.
Some big companies run their own web servers, but it is more common to use the services of a web hosting company who charge a fee to host your site.

Screen readers are programs that read out the contents of a computer screen to a user. They are commonly used by people with visual impairments.
In the same way that many countries have legislations that require public buildings to be accessible to those with disabilities, many laws have also been passed that require websites be accessible to those with disabilities.
Throughout this book you will see several references to screen readers. These notes will help ensure that the sites you create are accessible to people who use such software.
It is interesting to note that technologies similar to those employed by screen readers are also being used in other areas where people are unable read a screen, such as when they are driving or jogging.


When you are looking at a website, it is most likely that your browser will be receiving HTML and CSS from the web server that hosts the site. The web browser interprets the HTML and CSS code to create the page that you see. 
Most web pages also include extra content such as images, audio, video, or animations and this book will teach you how to prepare them for use on the web and then how to insert them into your web pages. 
Some sites also send JavaScript or Flash to your browser, and you will see how to add JavaScript and Flash in your web pages. Both of these technologies are advanced topics that you can go on to learn more about once you have mastered HTML and CSS, if you want to.


Small websites are often written just using HTML and CSS.
Larger websites — in particular those that are updated regularly and use a content management system (CMS), blogging tools, or e-commerce software — often make use of more complex technologies on the web server, but these technologies are actually used to produce HTML and CSS that is then sent to the browser. So, if your site uses these technologies, you will be able to use your new HTML and CSS knowledge to take more control over how your site looks.
Larger, more complex sites like these may use a database to store data, and programming languages such as PHP, ASP.Net, Java, or Ruby on the web server, but you do not need to know these technologies to improve what the user sees. The skills you'll learn in this book should be enough to help you on that road.


In the browser window you can see a web page that features exactly the same content as the Word document you met on the page 18. To describe the structure of a web page, we add code to the words we want to appear on the page.
You can see the HTML code for this page below. Don't worry about what the code means yet. We start to look at it in more detail on the next page. Note that the HTML code is in blue, and the text you see on screen is in black.
<html> 
<body>  
<h1>This is the Main Heading</h1>  
<p>This text might be an introduction to the rest of     
the page. And if the page is a long one it might     
be split up into several sub-headings.<p>  
<h2>This is a Sub-Heading</h2>  
<p>Many long articles have sub-headings so to help     
you follow the structure of what is being written.     
There may even be sub-sub-headings (or lower-level     
headings).</p>  
<h2>Another Sub-Heading</h2>  
<p>Here you can see another sub-heading.</p> 
</body> 
</html>



The HTML code (in blue) is made up of characters that live inside angled brackets — these are called HTML elements. Elements are usually made up of two tags: an opening tag and a closing tag. (The closing tag has an extra forward slash in it.) Each HTML element tells the browser something about the information that sits between its opening and closing tags.



#thE Evolution of htMl

Since the web was first created, there have been several different versions of HTML

Each new version was designed to be an improvement on the last (with new elements and attributes added and older code removed).
There have also been several versions of each browser used to view web pages, each of which implements new code. Not all web users, however, have the latest browsers installed on their computers, which means that not everyone will be able to view all of the latest features and markup

Although HTML 4 had some presentational elements to control the appearance of pages, authors are not recommended to use them any more. (Examples include the <center> element for centering content on a page, <font> for controlling the appearance of text, and <strike> to put a line through the text — all of these can be achieved with CSS instead.) 

In 1998, a language called XML was published. Its purpose was to allow people to write new markup languages. Since HTML was the most widely used markup language around, it was decided that HTML 4 should be reformulated to follow the rules of XML and it was renamed XHTML. This meant that authors had to follow some new, more strict rules about writing markup. For example:
Every element needed a  ● closing tag (except for empty elements such as <img />). Attribute names had to be in  ● lowercase. All attributes required a value,  ● and all values were to be placed in double quotes. Deprecated elements should  ● no longer be used. Every element that was  ● opened inside another element should be closed inside that same element.


The examples in this book all follow these strict rules of XML.
One of the key benefits of this change was that XHTML works seamlessly with other programs that are written to create and process XML documents.
It could also be used with other data formats such as Scalable Vector Graphics (SVG) — a graphical language written in XML, MathML (used to mark up mathematical formulae), and CML (used to mark up chemical formulae).
In order to help web page authors move to this new syntax, two main flavors of XHTML 1.0 were created: Strict XHTML 1.0 ● , where authors had to follow the rules to the letter Transitional XHTML 1.0 ● , where authors could still use presentational elements (such as <center> and <font>).
The transitional version of XHTML was created because it allowed authors to continue to follow older practices (with a less strict syntax) and use some of the elements and attributes that were going to be removed from future versions of HTML.
There was also a third version of XHTML 1.0 called XHTML 1.0 Frameset, which allowed web page authors to partition a browser window into several "frames," each of which would hold a different HTML page. These days, frames are very rarely used and are being phased out.
In HTML5, web page authors do not need to close all tags, and new elements and attributes will be introduced. At the time of writing, the HTML5 specification had not been completed, but the major browser makers had started to implement many of the new features, and web page authors were rapidly adopting the new markup.
Despite the fact that HTML5 is not yet completed, you can safely take advantage of the new features of the language as long as you endeavour to ensure that users with older browsers will be able to view your pages (even though some of the extra features will not be visible to them).


#Layout

For a long time, web page authors used <div> elements to group together related elements on the page (such as the elements that form a header, an article, footer or sidebar). Authors used class or id attributes to indicate the role of the <div> element in the structure of the page.

The <header> and <footer> elements can be used for:
The main header or footer  ● that appears at the top or bottom of every page on the site. A header or footer for an  ● individual <article> or <section> within the page.
In this example, the <header> element used to contain the site name and the main navigation. The <footer> element contains copyright information, along with links to the privacy policy and terms and conditions. Each individual <article> and <section> element can also have its own <header> and <footer> elements to hold the header or footer information for that section within the page. 
For example, on a page with several blog posts, each individual post can be thought of as a separate section. The <header> element can therefore be used to contain the title and date of each individual post, and the <footer> might contain links to share the article on social networking sites.





























