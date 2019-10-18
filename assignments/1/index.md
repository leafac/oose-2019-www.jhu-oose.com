# Assignment 1: Design Rudiments

<small>
Submit your assignment as a [Markdown](/toolbox#authoring-language-markdown) document at `assignments/1.md` in the `master` branch of your personal repository at `https://github.com/jhu-oose/{{site.course}}-student-<identifier>`.
</small>

# Working on Assignment

<video src="https://archive.org/download/jhu-oose/oose--assignments--1.mp4" controls preload="none"></video>

# Class Diagram

Before the Internet, one of the most interesting things you could do on a computer was playing Minesweeper. Remember the old times:

<figure>
<div id="game"><!-- minesweeper game initializes here --></div>
<figcaption markdown="1">
A clone of Minesweeper from Windows XP.  
A copyright infringement courtesy of <https://codepen.io/joelbyrd/pen/hdHKF>{:data-proofer-ignore="true"}.
</figcaption>
</figure>
<link rel="stylesheet" type="text/css" href="minesweeper.css" />
<script src="jquery.min.js"></script>
<script src="minesweeper.js"></script>
<style>
#game {
    text-align: center;
}
#game-container {
    text-align: left;
    display: inline-block;
}
</style>

## Diagram

<small>
**65 points**
</small>

Draw a high-level class diagram to communicate the logic of Minesweeper.

Include new games, different board sizes, flags (which you can test by right clicking), the flag counter (top left), marks (`?`) (which you can test by right clicking twice), mines, tiles that are open or closed, the timer (top right), opening tiles, creating a new game, wining the game, losing the game, and everything else you find the game.

Don’t include things like _controllers_, _repositories_, a _server_ and so forth. Your diagram could be implemented as a web server, as a desktop application, as a mobile application, and so forth.

## Implementation

<small>
**15 points**
</small>

Implement in Java at least two classes from the diagram you [drew above](#diagram). These classes must share some form of relationship (dependence, association, whole-part, inheritance, and so forth).

Your implementation must include the details that you omitted in the class diagram, for example, identifiers, getters and setters, the actual implementation of the methods, and so forth.

It’s okay if your code doesn’t compile because it depends on other parts of the application that you aren’t implementing in this exercise.

# Architecture

<small>
**10 points**
</small>

An HTTP request arrives at the [TODOOSE](https://github.com/jhu-oose/todoose) server asking for the list of items (see the `Get TODO items` request in Postman). Several parts of the server will be activated to respond to this request. Put the parts in the order in which they’ll be activated (that is, trace the request through the server):

- Model.
- View ([JSON Mapper](/toolbox#json-mapper-jackson)).
- Router.
- Repository.
- Controller.

# Technology

Continue watching the [TODOOSE video series](/todoose). We’re three weeks away from diving deep into the implementation, and by then you’ll have to know the basics.

## Server

<small>
**5 points**
</small>

Point out in the [code base](https://github.com/jhu-oose/todoose) where is the implementation for each of the server parts we discussed in the [Architecture](#architecture):

- Model.
- View ([JSON Mapper](/toolbox#json-mapper-jackson)).
- Router.
- Repository.
- Controller.

Your answer must be a range of lines of code, for example, if asked about where in the implementation the server connects to the database, you’d answer with [`todoose/src/main/java/com/jhuoose/todoose/Server.java:15-15`](https://github.com/jhu-oose/todoose/blob/90ca0901e09095460845eae20218bc5189bec565/src/main/java/com/jhuoose/todoose/Server.java#L15-15).

## Client

<small>
**5 points**
</small>

Which lines of code would you have to modify in the client part of TODOOSE so that it displays your name in the header? For example, if your name were `JHU OOSE Example Student`, then TODOOSE would look like this:

<figure markdown="1">
![TODOOSE Custom Header](todoose-custom-header.png){:width="408"}
</figure>

{% include assignment_submission_form.md assignment="1" %}
