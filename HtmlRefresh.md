## HTML Refresher

HTML stands for HyperText Markup Language.  It allows us to create websites!  HTML is used for defining how a browser should display information.  This is achieved through a standard set of tags, which tells the browser what to do with the text inside the tags.  

HTML works by creating a .html file (MyVideoGames.html for example).  Within the .html file, you define your page using special html tags.  Tags are the words between the greater than / less than brackets: <>. An example of a tag is \<b>.  

Every html file begins with \<!DOCTYPE html> and will have a beginning and ending \<html> tag.  An example html file looks like: 

\<!DOCTYPE html>

\<html>

\<head>

\<title>My Videogames</title>

\</head>

\<body>

\<p>This is a paragraph about my videogame.</p>

\</body>

\</html>

Explanation of tags: 

The header tag: 
The \<head> element is a container for all the head elements. The <head> element can include a title for the document, scripts, styles, meta information, and more. 

The p tag: The HTML <p> element represents a paragraph of text. 

The bold tag: 
\<b>
<b>These words will be bold because they are within the b tag</b> 
\</b>, but these words will not be bold.  The browser understands that anything within a \<b></b> should be displayed in bold lettering, and the browser is also smart enough to hide the tag.  

When we want to build large websites that have the same look and feel, repeating the same html tags in each .html file becomes repetitive and hard to manage.  This is where cascading style sheets (CSS) comes in!  

Cascading style sheets are used to control how a page is presented and make changing their display easier and more accessible.

Your html page will reference 

body {
    background-color: lightblue;
}

h1 {
    color: navy;
    margin-left: 20px;
}

To make games, we might not want to use JavaScript by itself and could use some help from HTML and CSS.  HTML and CSS can draw elements on webpages, while JavaScript can bring these objects to life.  We can use these technologies to create fun games, which we can share with our friends.  JavaScript tells the computer how to do things like keep track of score, move elements on the screen, and know when a game is won or lost.

If you want to brush up on your HTML and CSS, then take a look at the webpages below.  However, we will not be writing a lot of HTML and CSS.
* [HTML Tutorial](https://www.w3schools.com/html/)
* [CSS Tutorial](https://www.w3schools.com/css/)

