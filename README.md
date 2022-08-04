# HTML-projects
Hola ! This repository consists of all html based projects that i have done

HTML stands for hypertext markup language.
It is used to define the structure of webpages and determines the how content is displayed online.
HTML5 is the current major version of HTML in use. W3c(worldwideweb) consortium is responsible for layout the specifications of HTML which is followed by all browsers
-- Designing a web application involves displaying data from server, handling client side operations, serverside operations and database manipulation
-- To ensure smooth execution of these operations we use a combination of programming languages, tools and frameworks called a technology stack or tech stack.

-- Tech stack is generally visualized in two parts :
	front end : It refers to the technologies used for interactions with the user.
	backend : it refers to the technologies used on server for processing the user inputs and interacting with database.

At the start of a project, it is essential to identify the right tech stack to speedup development and ease of work of the developer.

There are variou stacks available for this purpose namely
LAMP -- linux, apache, mysql, php 
MERN -- mongodb, express.js, react, node.js
MEAN --mongodb, express.js, angular, node.js


The main reasons to adopt JS(MERN/MEAN) stack over other stacks are :

1. opensource technologies
2. common language
3. cost effective
4. usage of JSON

structure of webapplication
--------------------------
to make things easier , the application is divided into client side and serverside .

client side(front end): An application running on the end user's machine 	such as PC, notebook,mobile,lap etc. which will communicate with 	the server to fetch the required information. 
server side(backend): the business logic and validations required for processsing the request or data that is sent by client is hosted on the server side.


flow of data :
--------------
Asssume you are using google for learning something which is built using JS(MERN/MEAN)stack
1. when you enter a domain name(www.google.com) in the search bar,you are actually entering Universal Resource Locator(URL) of lex web page.

2.when you hit enter button , a request is made for the requested webpage document using Hypertext tranfer protocol(HTTP) . The chrome webpage that you see can be built using the angular/react framework.

3. when you click on the webcourse that you wanted to study, the click action creates a request which is sent to the node server.

4.the incoming user request is redirected to the appropriate request handler.

5. The request is processed and call to the database is made to fetch requested course.

6. the webpage in which the requested video is embedded is sent back to the node server.

7.the node server returns the response to the webbrowser

8. the response is then rendered on the web browser.


 Uniform resource locator(URL) :
---------------------------------------
It is used to identify the particular resource uniquely on the internet.
It has the following components :

protocol://host:port/path

protocol : the protocol is used to communicate with the server.

host : name of the server to connect to

port : every protocol on the internet operates on a unique TCP/IP port. if port is not explicitly specified in URL, default port for that protocol is assumed. The standard port for HTTP is 80

path : specifies the path of the resource on the server(usually starts with '/' which is sometimes known as webroot)

HTTP response 
--------------

The server responds to the client through HTTP response. An HTTP response has a status line, a header, and a message body.

-- to inform the browser regarding the status of the request made to the server, the HTTP response contains a field called status code. that is issued by server.

DIfferent HTTP Response

status-code     titile			description
------------------------------------------------------
1**		informational response		it indicates that the request was received and understood and also alerts the client to wait for a final response.
2**		success				indicates that the request was received , understood accepted and successfully processed.
3**        	redirection			indicates that the client must take additional action to complete the request.
4**		client error		intended for situations where the client has caused the error. The server specifies wheather the error caused is temporary or permanent.
5** 		server error		intended for situations when the server failed to fulfil the request.


some of the most familiar status codes 
200 ok
403 forbidden
404 not found
500 internal server error

To inform client about the incoming data format from the server, the HTTP response contains a content-type field. The value for this field will be among the MUltipurpose Internet Mail Extensions(MIME) standard datatypes.

MIME :
------
-- It is a standardized way to indicate the nature and format of the response.
-- server inserts MIME type as a value in the contenttype attribute of the response header before sending a response to the client.

--clients use this content type or media type header to select an appropriate viewer application for the type of data the header indicates.

some familiar content-types are :

text : 
	text/plain
	text/html
	text/css
	text/javascript
image :
	image/png
	image/jpeg
	image/gif
application :
	application /json
	application/sql
	application/javascript
 
Why do we need HTML?
-------------------
for better looking and easy to understand the data

what is html?
--------------
HTML(HYpertext markup language)

	Hypertext refers to word,phrase or chunk of text that can be linked to another document/information. By clicking on the link(hypertext) user can jump to different content
	markup language is a combination of words and symbols, developed for the purpose of processing the information, which give instrutions on how a document should appear on web 

html is caseinsensitive
basic structure :

<html>
     <head>
           <title> Homepage </title>
     </head>
     <body>
           Hello World!
     </body>
</html>



	
what all can HTML do?

-publish documents with text,headlines and images etc
- create forms to collect user data
-includes videos,audioclips,flashmovies etc inside an HTML document
- access online information via hyperlinks
-run on different os without making any modifications


HTML elements
--------------
HTML elements are made up of 2 things: 
1. tags - Html instructions
2. content - on which html instructions should be applied

different categories of elements :
----------------------------------
types of elements :
1.container elements (contains both start and end tag)ex: <title></title>
2. empty element(contains only end tag)ex: <br/>

type of element
1. block level element(starts on a new line)Ex: h1,div
2. inline element (starts on the same line)ex: span, a

HTML attribute :
----------------
.. an HTML attribute modifies an HTML element to give certain characteristics to the element and provide additional information about it. They are always specified in the start tag.

syntax: <tagname attributename="value"></tagname>
ex: <htmllang="en-us"></html>

comments :
----------
As a developer, you may want to document your code, so that you can easily refer it in the feature.
for this comments can be used. comments are ignored by browser.

syntax :

<body>
<!-- this is comment-->
</body>

The skeleton of HTML5 page :
---------------------------------
<!DOCTYPE html>  <!-- DTD(document type definition)
                   It instructs web browser about the version of 
                   html in which the page is written in. -->
<html>          <!-- container for various html elements -->   
    <head>      <!-- container for various head elements
                     consists of metadata content -->
    </head>     
    <body>      <!-- contains all the contents of a html document -->
    </body>
</html>

elements(individual components in HTML document)
HTML meta data is data about HTML document. Metadata is not displayed but will be read by the machine. 
it involves information about the type of character encoding,author,description, refresh and much more.

Body element
------------
The <body> tag defines the document's body by containing all the contents of an HTML document, such as text, hyperlinks, images, tables, lists, etc.

syntax :

<body>
    <form>
        <input>
    </form>
    <table>    </table>
    <img>
    <audio></audio>
    <video></video>
    <br>
    <div></div>
    <span></span>
    <h1></h1>
</body>

In the above code snippet, 

The <form> tag is used to create a HTML form to get the user input.
The <input> tag specifies the input field where the user can enter the data.
The <table> tag defines a HTML table.
The <img>, <audio>, <video> tags are used to add the external content like image, audio,video to our HTML document.
The <br>, <div>, <span>, <h1> tags are used for the text and space formatting.

Title tag:
The <title> tag defines the title of the document in the browser toolbar.

The string specified between the opening and closing <title> tags is displayed when the web page is bookmarked or when added to favorites.

In order to see what the webpage looks like, create an HTML file travelDestiny.html and copy the below code.


<!DOCTYPE html>
<html lang="en">
<head>
    <title>Travel destiny</title>
</head>
<body>
    <!-- Page content comes here -->
</body>
</html>

so, it is concluded that the data as a title is displayed on the browser tab

--as a developer, if you want your web page to be listed in the result generated by the search engine then you should mention keywords based on content of your web page.
-- for mentioning keywords , meta element is used.

what is meta element?

In HTML, metadata is used to specify additional important information about a document in a variety of ways. The meta elements can be used to include key-value pairs describing properties of the HTML document, such as author, a list of keywords, document author, character encoding etc.

Meta element is defined within head element. It is machine readable, hence does not render anything on web page.

<head>
    <meta attributes>
</head>

Attributes of meta element ;

attribute 		value			description

----------------------------------------------------------------
name			application name
			author			specifes name of meta data
			description
			generator
			keywords
	
http-equiv		content-type		provides http header for information/value of content attribute
			default-style
			refresh

content			text			gives the value associated with http-equiv or name attribute
charset			character_set		specifies character encoding for an HTML document


ex :
1. specifying tutorial and HTML as keywords for webpage content.
<meta name="keywords" content="tutorial,HTML">

2.specifying refresh-rate of 30 second for webpage
<meta http-equiv="refresh" content="30">

3. specifying that webpage uses characterset-encoding of UTF-8
<meta charset="utf-8">

Body element:
-------------
The <body> tag defines the document's body and is used to add content to the web page.

There can be only one <body> element in a HTML document

	
<!DOCTYPE html>
<html> 
    <head>
       <title>Travel Destiny</title>
    </head>
    <body>
	Destiny Tour and Travels <br/> You choose us! we never let you down!!
    </body>
</html>

note : <br/> tag is used to insert a line break.

what is form element ?

forms are used for collecting user information which may be for registration , payment etc. A form can contain text-fields,check boxes, radio-buttons etc. forms are used to pass user-data to a specified URL.
 To create form in HTML, <form> tag is used . let's see the syntax below.

syntax :

<form name="name of the form" action="link to server side program" method="HTTP Request method">
<!-- all the form elements will come here-->
</form>

In the above code snippet, 

The Name attribute is used for accessing the form data by the scripting language.
The Action attribute is used to specify the server-side programe that will be executed when the form is submitted.
The Method attribute is used to specify the HTTP request method that will be used to submit the form data to the server-side program.

Attributes of form element :

Attribute 		Description
-----------------------------------------
name			Unique name that identifies a form
	
action			URL of the destination page

method			commonly used HTTP Methods are GET & POST
			The default method is GET
			GET : when this used, form data will be appended to the URL and visible to everyone . Ex: /traveldestiny.html?username=Charan
			POST : when this method is used , form data is placed inisde HTTP Request body and not visible

nonvalidate		skips validation upon form submission

Other HTTP methods are PUT,DELETE,TRACE,HEAD,OPTIONS and CONNECT 
=-------------------------------------------------------------------


INPUT element
-----------

<input> tag specifies an input field used inside a form, where a user can enter data. 

syntax :

<input type="input type" value="element value">

In the above code snippet, 

The Type attribute is used to specify type of element.
The Value attribute is used to specify the element's value that will be send to the server program.

input types in HTML5 :

value 		Description
----------------------------
text		creates a string input field
	
password	creates a password input field in masked format

radio		creates a radio buttton

checkbox	creates a checkbox

button		creates a simple button

submit		creates a button to submit the form

reset		creates a button to reset form fields

date		input represents date(year,month,date) value without timezone

email		input represents an email address value

number		input represents a numerical value

url		input represents URL address value

file		input represents user to select a value

color		input that lets the user choose the color

range		input that lets the user choose a number from a range

datalist	defines a list of predefined value for  an input

-------------------------------------------------------------------------
Attributes of input element

The table below lists the attributes of <input> tag

Attribute 		Description
-------------------------------------
required		value required for form submission

value			specifies default value of input element

type			identifies the type of input element

name			name of input element used for form submission

size			identifies width of input text that the user can see

autofocus		focuses on particular form element automatically

maxlength		identifies the maximum length of input value

minlength		identifies the minimum length of the input value

pattern			specifies a pattern(regular expression) for entering input text

placeholder		displays text(hint) within an input control for the user

steps			specifies the legal number of intervals

formnovalidate		skips validations upon form submission, used with submit button.
=---------------------------------------------------------------------

Label element

-------------
A form contains field names and input fields. The <label> tag defines a label for an input element.

since, the user interacts with the page using the input elements, they are also called UI(userinterface) components.

syntax :

<lable attribute="value" > text</label>

along with displaying the field names, the <label> element improves the usability for the user.
if the user clicks on the text within the <label> elment, it toggles the control. This is only done using for attribute.

A label can be bound to an input element by using the "for" attribute. Value of for attribute should be same as the value of id attribute in input element.


Table element
------------
A table element in html helps in representing content in terms of two dimensional structure. i.e; a combination of rows and columns.

The tag used for creating an HTML table is <table>

syntax for creating a table is as follows :

<table>
<thead><!--The <thead> tag is used to provide the heading to the table.-->
<tr><!-- The <tr> tag is used to create the rows in the table.-->
<th><!--The <th> tag is used to create the columns in the table -->
</th>
</tr>

<tbody><!--The <tbody> tag is used to enclose the content in table. -->
<tr>
<td>
</td>
</tr>
</tbody>
</table>

    <table border="6">
        <thead>
            <tr> <th>Employee Id</th> <th>Employee Name</th> </tr>
        </thead>
        <tbody>
            <tr> <td>1001</td> <td>charan</td> </tr>
            <tr> <td>1002</td> <td>Naga</td> </tr>
        </tbody>
    </table>

we can use <caption> tag for the title of the table .


Attributes of th and td element

table attributes
Attribute 	Description
------------------------------
colspan		Merges column
rowspan		Merges rows
----------------------------
colspan :

colspan attribute helps the cell to span across multiple columns. Suppose (as shown below) if you need to merge two columns. Let it be c1 & c2 then colspan="2" is used. simply if you want to merge third column as well i.e; c3.Then colspan value should be colspan="3"

<tr>
<td colspan="3">A </td>
<td>B</td>
<td>c</td>
</tr>

rowspan
--------
row span attribute helps the cell to span across multiple rows. lets take example as shown below. two rows R1 & R2 are to merged for column c1 only. then will definitely tags of c1 column you should write rowspan="2" so that R1 & R2 gets merged. Simmilarly for merging third row, rowspan="3" is used.

<tr>
<td rowspan="2">A</td>
<td>B</td>
<td>C</td>
<td>D</td>
</tr>

Aligning forms with Table elements :

--We all know that alignment is a very important and indispensable part of a webpage.


source code ;

<body>
    <form>
        <h2> Trainee Details:</h2>
        <label for="name">Name</label>
        <input type="text" id="name" /> <br>
        <label for="age">Age</label>
        <input type="number" id="age"><br>
        <label for="email">Email:</label>
        <input type="text" id="email"> <br>
        <label for="country">Nationality:</label>
        <select id="country">
            <option value="India">India</option>
            <option value="USA">USA</option>
            <option value="Europe">Europe</option>
            <option value="RestofWorld">Rest of the World</option>
        </select><br>
        <label>I am interested in</label>
        <input type="checkbox" name="technology" value="angular">Angular
        <input type="checkbox" name="technology" value="react">React
        <input type="checkbox" name="technology" value="vuejs">VueJS
        <br>
        <input type="button" value="Submit">
        <input type="button" value="Reset">
    </form>
</body>
Before align

After align
source code :

<body>
    <form>
        <h2> Trainee Details:</h2>
        <table>
            <tr>
                <td><label for="name">Name</label></td>
                <td><input type="text" id="name" /></td>
            </tr>
            <tr>
                <td><label for="age">Age</label></td>
                <td><input type="number" id="age"></td>
            </tr>
            <tr>
                <td><label for="email">Email</label></td>
                <td><input type="text" id="email"></td>
            </tr>
            <tr>
                <td><label for="country">Nationality</label></td>
                <td><select id="country">
                        <option value="India">India</option>
                        <option value="USA">USA</option>
                        <option value="Europe">Europe</option>
                        <option value="RestofWorld">Rest of the World</option>
                    </select>
                </td>
            </tr>
            <tr>
                <td><label>I am interested in</label></td>
                <td><input type="checkbox" name="technology" value="angular">Angular
                    <input type="checkbox" name="technology" value="react">React
                    <input type="checkbox" name="technology" value="vuejs">VueJS
                </td>
            </tr>
            <tr></tr>
            <tr><td><input type="button" value="Submit"></td>
            <td><input type="button" value="Reset"></td></tr>
        </table>
    </form>
</body>

what is Anchor element ?

-- Any text or image that provides a link to another webpage is called "hyperlink"

-- A website consists of multiple webpages. Generally webpages need to be linked with one another to make it navigable. To link webpages , anchor element is used.

It is defined using <a> --</a> tag.

syntax :

<a href="url" target="value">Text</a>

In the above code snippet, 

The href attribute is used to specify the url of the webpage that needs to be linked.
The target attribute is used to specify where to open the linked webpage.

note : text/image can be used as link

ex ;
 < a href="demo.html" > view demo</a>

Appearence of links based on their state :

. An unvisited link is underlined and blue
. A visited link is underlined and purple
. An active link is underlined and red

Now let's understand the attributes for <a> tag

	Anchor tag attributes
Attribute		Description
-----------------------------------
href			specifies reference URL for creating hyperlink

target			Specifies where to display the linked resource

------------------------------------------------------------------------


Attributes of anchor element

following are the possible values for target attribute

	target Attribute
Value		Description
-----------------------------
_blank		linked resource will open in a new window
	
_self		linked resource will open in a current window
	
_parent		linked resource will open in the parent of the current window(if no parent it behaves like _self)

_top		linked resource will open in the top most level window of the current windwo(if no parent it behaves like _self)

------------------------------------------------------------[

ex: <a href="https://charanItsolutions.com/"target="_blank">visit to  LEARN IT skills</a>


Note : When a link opens a URL in a new tab with target="_blank", it is very simple for the opened page to change the location of the original page because of usage of the JavaScript variable window. The Opener will not be null and thus "window.opener.location" can be set by the opened page. This exposes the user's information to phishing attacks. Hence security aspects with respect to this have to be taken care while developing applications. The simplest way to achieve security is to use rel attribute of anchor element. ( For e.g., 

<p> To visit charanIT solutions<a href="https://charanITsolution.in/home"target="_blank"rel="noreferrer noopener">Go to Skill Learn website</a></p>

Image Element
----------------
Embedded Elements :

Embedded elements
Content of your webpage may need to have multimedia components like image, audio, video or incorporation of another webpage in your webpage. To add such components, embedded elements  like image element, audio element and video element are used.

 
--Every embedded element generates a new request to fetch the embedded component from the server.

Image Element

-- Images can be inserted into HTML page by using <img/>tag
-- the <img/> tag is empty tag as it does not have a closing tag

Attributes of image element

Below are the list of Image element

			Image Attributes
Attribute		Description
--------------------------------------
src			specifies the path of the image

border			specifies the border of the image

width			specifies the width of the image

height			specifies the height of the image

alt			provides an alternative text describing the image if image is not available.
--------------------------------------------------------------------
syntax :

<img src="link of image"alt="alternative text"/>

can we make an image act as a link?
yes, images can be made to act as a link by placing <img>inside<a>element.

syntax :
<a href="demo.html">
<img src="image.jpg"alt="google homepage">
</a>

Audio element
--------------
The audio element is used to embed audio in webpage.
To play an audio file in HTML, use <audio>tag.

Attributes of audio tag
		
		Audio attributes

Attributes		Description
--------------------------------------
src			Specifies the url of the media resource

controls 		Media control features like play/pause will be displayed

loop			causes the media to play in a loop

autoplay		Media will play automatically on page load

muted 			Media will play in muted state
--------------------------------------------------------------------
syntax :

<audio src="link of the audio file" controls="controls">Your browser does not support the audio tag</audio>

In the above code snippet, 

The src attribute is use to specify the location of the audio file. 
The controls attribute is used to specify weather to display the player controls or not.

--content between <audio> and </audio> tag will be shown by browsers who do not support audio element


Attribute of Audio element
----------------------------
1.playing audio file in loop

<audio src="myAudio.mp3" controls="controls" loop>Your browser does not support the audio tag</audio>


2. autoplaying audio file

<audio src="myaudio.mp3"controls="controls" autoplay>your browser does not support audio tag</audio>

3. preloading metadata of the audio file

<audio src="myAudio.mp3" controls="controls" preload="metadata">Your browser does not support the audio tag</audio>

4. mutes audio file

<audio src="myAudio.mp3" controls="controls" muted>Your browser does not support the audio tag</audio>


Video element
---------------
The video tag specifies video such as a movieclip or other video streams. The <video> tag specifies a standardway to embed a video in a webpage.

		Video Attributes
Attributes 		Description
-----------------------------------------
src		specifies the url of the media resource

controls	media control features like play/pause will be displayed

loop		causes the media to play in a loop

autoplay	Media will play automatically on page load

muted		Media will play in a muted state

width		specifies width of the image in pixels

height		specifies the height of the image is pixels

poster		Represents frame for the video till the video is played
------------------------------------------------------------------------

syntax :

<video src="link of video file" controls="controls"> your browser does not support the video tag</video>

In the above code snippet, 

The src attribute is use to specify the location of the video file. 
The controls attribute is used to specify weather to display the player controls or not.

--content between <video>and </video> tag will be shown by browser who do not support video element.

Attributes of video element

1.Specifying Width & height for the video

<video src="myvideo.mp4"controls="controls" width="300"height="100">your browser doesnot support the video tag</video>

2. specifying poster for the video

<video src="myvideo.mp4"controls="controls"poster="firstframe.png">Your browser does not support the video tag</video>


Source Element

-- The <source> tag allows you to specify alternative multiple media resources for media elements, which the browser may choose from, based on its media type, codec support or media query.

-- You must list different media sources in order - most desirable to least desirable.

Note: <source> element is considered only when src attribute of media element is absent.

ex: <audio>
    <source src="myAudio.mp3" type="audio/mp3" >
    <source src="myAudio.ogg" type="audio/ogg" >
</audio>

<video>
    <source src="myAudio.mp4" type="video/mp4">
    <source src="myAudio.ogg" type="video/ogg" codecs="theora,vorbis" >
</video>

In the above code snippets,

--The src attribute is use to specify the location of the audio or video file. 

--The type attribute is used to specify the type of the file either audio or video file.

--The codecs attribute used to specify version of the codecs needed to play the audio or video file.


usage of <source>tag is to list multiple sources of media elements in HTML page.

Text formattting elements 

Heading elements
---------------------
HTML provides the elements like <h1>---<h6> in order to format headings.

Each HTML headings has a default size, where <h1>(32px) defines the most important heading and <h6>(10px) defines the least important heading.

users skim the contents in web pages by its headings

Headers in HTML

<!DOCTYPE html>
<html>
<body>
	<h4>Heading Tags</h4>
	<h1>Welcome to HTML</h1>
	<h2>Welcome to HTML</h2>
	<h3>Welcome to HTML</h3>
	<h4>Welcome to HTML</h4>
	<h5>Welcome to HTML</h5>
	<h6>Welcome to HTML</h6>
</body>
</html>


Text Formatting Elements

HTML defines the formatting elements for the text in the webpages.

Table below lists widely used text formatting elements supported in HTML5.

	various attributes of HTML5
Attribute		Description
--------------------------------------
<b>		describes bold text

<del>		describes deleted text

<em>		describes emphasized text

<i>		describes italicized text

<ins>		describes inserted text

<mark>		describes highlighted text

<small>		describes small text

<strong>	describes strong text

<sub>		describes subscripted text

<sup>		describes superscripted text
------------------------------------------------
list elements

-- the data in the webpages are better perceived when it is organized into lists. The lists can either be nubmbered(ordered list) or unnumbered(unordered).

there are 3 types of lists can be created in HTML :

types of list :

1.unordered list

2.ordered list

3.description list

1.unordered list
---------------------
--It groups a set of items with no particular order.

--An unordered list starts with the <ul> tag. Each list item starts with the <li> tag. The list items will be marked with disc (small black circles) by default.

syntax :

<ul type="disk">
    <li>List Item 1</li>
    <li>List Item 2</li>
    <li>List Item 3</li>
</ul>

In the above code snippet, 

The type attribute specifies the pattren of the bullet.


ex :

<ul type="circle">
    <li>Cake</li>
    <li>Biscuits</li>
    <li>Fruits</li>
</ul>

value of type attribute(unordered list)
value		description
------------------------------
disc		marked with black circle(default)

circle		marked with circle

square		marked with square
-----------------------------------------

2.ordered list
-----------------

-- ordered list groups a set of items in a spcific order

--An ordered list starts with the <ol> tag. Each list item starts with the <li> tag. An ordered list can be numerical or alphabetical. The list items will be marked with numbers by default.

syntax :

<ol type="1">
    <li>List Item 1</li>
    <li>List Item 2</li>
    <li>List Item 3</li>
</ol>

-- type attribute specifies numbering scheme.

values of type attribute(ordered list)
Value		Description
-----------------------------
1		marked with numbers(default)

A		marked with uppercase letters

a 		marked with smallcase letters

l 		marked with uppercase Roman Numbers

i 		marked with lowercase Roman numbers
-----------------------------------------------------

3.description list
--------------------
-- Description Lists displays a list of terms and their descriptions. The <dl> tag defines the description list, the <dt> tag defines the description term, and the <dd> tag contains the definition of the description term.

syntax :

<dl>
  <dt>Description term 1</dt>
  <dd>Description detail 1</dd>
  <dt>Description term 2</dt>
  <dd>Description detail 2</dd>
</dl>

ex :
<dl>
  <dt>Books</dt>
  <dd>printed work consisting of pages glued along <br/>
one side and bound in covers</dd>
  <dt>Pencil</dt>
  <dd>a item used for writing</dd>
</dl>



character entities
----------------------

Some characters are reserved in HTML.

For e.g.: If you use the less than (<) or greater than (>) sign in your content, browser may mix them with tags.

Also some characters are absent on keyboard.

For e.g.: ©

To include such characters as content, Character entities are used.

Character entity references start with an ampersand (&) and end with a semicolon (;)


syntax :

&entity_name;
    or
&#entity_number;


		HTML Character Entities
character	Description	Entity Name	Entity Number
-------------------------------------------------------------
<space>		non-breaking space	&nbsp;		&#160;

<		less than		&lt;		&#60;

>		greaterthan		&gt;		&#62;

&		ampersand		&amp;		&#38;

copyright(symbol) copyright		&copy;		&#169;

TM		trademark		&trade;		&#153;

Registered		RegisteredTrademark	&reg;	 &#174;
trademark(symbol) 

----------------------------------------------------------------
<hr>can be used to insert a thematic break.

		semantic elements
-- To keep varied content of webpage organized , it is good UI practice to arrange them in different sections.

--organizing content in section, also provides better semantics(meaning) to content.
 For this, semantic elements are used.

Below are few sectioning elements supported by HTML5.

		Different sectioning elements by HTML5
sectioning element		Description
--------------------------------------------------
main				defines the main content of document

section				represents a group of related content
	
article				defines individual self-contained content

header				defines the header for the document or a section

footer				defines a footer for the document or a section

nav				Defines the navigation links

aside				Defines content part from the page content

address				defines contact information for an article or webpage

h1,h2,h3,h4,h5,h6		defines heading
-----------------------------------------------------------------------
he better organized the content of web page is, the better semantics the developers have followed.

The better semantics the web pages have followed, the better the pages are handled by computer programs.

Hence, as a web developer, you should use appropriate sectioning elements to leverage their benefits. You should also ensure that the elements are defined in the right order. Using a footer tag before a header tag will lead to header information appearing after the footer information!

