## The main goal — pixels on the screen

> The Critical Rendering Path is the sequence of steps the browser goes through to convert the HTML, CSS, and JavaScript into pixels on the screen. Optimizing the critical render path improves render performance. The critical rendering path includes the Document Object Model (DOM), CSS Object Model (CSSOM), render tree and layout.

>  The document object model is created as the HTML is parsed. The HTML may request JavaScript, which may, in turn, alter the DOM. The HTML includes or makes requests for styles, which in turn builds the CSS object model. The browser engine combines the two to create the Render Tree. Layout determines the size and location of everything on the page. Once layout is determined, pixels are painted to the screen.
https://developer.mozilla.org/en-US/docs/Web/Performance/Critical_rendering_path

## Store and access data
1960s, navigational DBMS
1970s, relational DBMS
Late 1970s, SQL DBMS
2000s, NoSQL and NewSQL

https://en.wikipedia.org/wiki/Database

## HTML

### Invention of HTML: document markup for CERN

https://en.wikipedia.org/wiki/Hypertext
https://en.wikipedia.org/wiki/History_of_hypertext

"The concept Borges described in 'The Garden of Forking Paths'—in several layers of the story, but most directly in the combination book and maze of Ts'ui Pen—is that of a novel that can be read in multiple ways, a hypertext novel. Borges described this in 1941, prior to the invention (or at least the public disclosure) of the electromagnetic digital computer. Borges also mentions how hypertext has three similarities of frued to a labyrinth in which each link brings the navigator to a set of new links, in an ever expanding maze. Not only did he invent the hypertext novel—Borges went on to describe a theory of the universe based upon the structure of such a novel."

Tim Berners-Lee, CERN
March 1989, May 1990

First tags set: http://info.cern.ch/hypertext/WWW/MarkUp/Tags.html

https://www.w3.org/History/1989/proposal.html
https://lists.w3.org/Archives/Public/www-talk/1991SepOct/0003.html

Web server: streaming text (srtings)

fisrt web server https://en.wikipedia.org/wiki/CERN_httpd

CERN httpd (later also known as W3C httpd) is an early, now discontinued, web server (HTTP) daemon originally developed at CERN from 1990 onwards by Tim Berners-Lee, Ari Luotonen[2] and Henrik Frystyk Nielsen.[1] Implemented in C, it was the first web server software.

Get data from HTML files on file system

Filesystem HTML files => Server listens requests and reads files => TCP/IP/HTML => Client

### Using Databases

Database => Server listens requests and runs server-side language (perl/PHP/C/Java) => Template engine => HTML on server side streams to TCP/IP/HTML => Client

### Standartisations

Server => HTML => Client

### Javascript

Server => HTML => Client + node replacement 
Server => JSON => Client + HTML generation + node replacement

### DOM
srting-based client side template enginges

> DOM construction is incremental. The HTML response turns into tokens which turns into nodes which turn into the DOM Tree. A single DOM node starts with a startTag token and ends with an endTag token. Nodes contain all relevant information about the HTML element. The information is described using tokens. Nodes are connected into a DOM tree based on token hierarchy. If another set of startTag and endTag tokens come between a set of startTag and endTags, you have a node inside a node, which is how we define the hierarchy of the DOM tree. https://developer.mozilla.org/en-US/docs/Web/Performance/Critical_rendering_path

## JSON streaming
gmail
AJAX (X - XML, but :))


### vDOM + reconciliation

Server => JSON => Client + node reconciliation 

Server => HTML => Client + Hydration
Server => JSON => Client

direct update


## HTML streaming renaissance
https://hotwired.dev
