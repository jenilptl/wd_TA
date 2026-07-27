# Lab No. 01 \| Exploring Websites & Understanding the Basics of the Internet and HTTP

# Learning Objectives

After completing this lab, you will be able to:

-   Understand what the Internet is.
-   Understand what the World Wide Web (WWW) is.
-   Explore the design of popular websites.
-   Identify common parts of a webpage.
-   Understand web browsers and search engines.
-   Learn common Internet protocols (HTTP, HTTPS, FTP).
-   Understand HTTP requests and responses.
-   Learn GET and POST requests.
-   Understand common HTTP status codes.
-   Compare website designs and identify good UI practices.

------------------------------------------------------------------------

# Why Are We Doing This Lab?

## What?

This lab introduces the basic concepts required before learning HTML,
CSS and JavaScript.

You will also observe how real websites are designed and understand how
browsers communicate with web servers.

------------------------------------------------------------------------

## Why?

Every website follows common design principles and communicates using
Internet protocols.

Before creating websites, we must understand how websites work.

------------------------------------------------------------------------

## When?

Whenever we open a website, search on Google, shop online, watch
YouTube, or book railway tickets, these concepts are working behind the
scenes.

------------------------------------------------------------------------

## How?

We will:

-   Visit popular websites.
-   Observe their design.
-   Compare them.
-   Learn Internet basics.
-   Learn browsers and search engines.
-   Learn HTTP, HTTPS and FTP.
-   Understand HTTP requests and responses.
-   Learn common HTTP status codes.

------------------------------------------------------------------------

# Concept Overview

## Key Concepts

-   Internet
-   World Wide Web (WWW)
-   Website
-   Webpage
-   Web Browser
-   Search Engine
-   HTTP
-   HTTPS
-   FTP
-   Client
-   Server
-   HTTP Request
-   HTTP Response
-   GET
-   POST
-   HTTP Status Codes
-   Responsive Web Design

------------------------------------------------------------------------

# Quick Theory

## What is the Internet?

The Internet is a worldwide network that connects millions of computers
and devices.

Real-life example:

Your laptop connects to Flipkart through the Internet.

------------------------------------------------------------------------

## What is the World Wide Web (WWW)?

The World Wide Web (WWW) is a collection of websites available through
the Internet.

Example websites:

-   www.flipkart.com
-   www.myntra.com
-   www.irctc.co.in

Think of it like this:

Internet = Road Network

Websites = Shops built on those roads.

------------------------------------------------------------------------

## Website vs Webpage

Website = Collection of webpages.

Webpage = One single page of a website.

Example:

Website: https://www.flipkart.com

Webpage: https://www.flipkart.com/mobiles

------------------------------------------------------------------------

## What is a Web Browser?

A browser is software used to open websites.

Examples:

-   Google Chrome
-   Microsoft Edge
-   Mozilla Firefox
-   Safari
-   Opera

------------------------------------------------------------------------

## What is a Search Engine?

A search engine helps us find websites.

Examples:

-   Google
-   Bing
-   DuckDuckGo
-   Yahoo

Browser != Search Engine

Chrome is a Browser.

Google is a Search Engine.

------------------------------------------------------------------------

# Understanding Website Design

Observe these websites:

-   www.flipkart.com
-   www.myntra.com
-   www.irctc.co.in

Notice:

-   Header
-   Navigation Bar
-   Search Box
-   Banner
-   Images
-   Buttons
-   Main Content
-   Footer
-   Colors
-   Fonts
-   White Space

Also compare:

-   Desktop view
-   Mobile view
-   Responsiveness

------------------------------------------------------------------------

# Internet Protocols

## What is a Protocol?

A protocol is a set of rules used for communication between computers.

Example:

Just like traffic rules help vehicles move safely, Internet protocols
help computers communicate correctly.

## HTTP

HTTP stands for HyperText Transfer Protocol.

It is used to transfer webpages.

Example:

http://example.com

HTTP is **not secure**.

------------------------------------------------------------------------

## HTTPS

HTTPS stands for HyperText Transfer Protocol Secure.

It encrypts data before sending it.

Example:

https://www.flipkart.com

Most modern websites use HTTPS.

------------------------------------------------------------------------

## FTP

FTP stands for File Transfer Protocol.

It is used to upload or download files between computers.

Example:

A web developer uploads website files from a computer to a web server
using FTP.

------------------------------------------------------------------------

# Client and Server

Client

-   Browser
-   Mobile App

Server

-   Computer storing website files

Communication

Client ----Request----\> Server

Client \<---Response---- Server

Example

You open Flipkart.

Browser requests homepage.

Server sends webpage.

Browser displays webpage.

------------------------------------------------------------------------

# HTTP Request

An HTTP Request is sent by the client to the server.

Common Request Methods

  Method   Purpose
  -------- --------------------------
  GET      Request data from server
  POST     Send data to server

## GET Example

Searching products on Flipkart.

Browser asks:

"Show me laptops."

Server sends laptop list.

## POST Example

Login form.

Username and password are sent to the server.

Server checks credentials.

Returns login success or failure.

------------------------------------------------------------------------

# HTTP Response

The server sends back an HTTP Response.

It contains:

-   Status Code
-   Headers
-   Webpage Data

Example

Browser requests Flipkart homepage.

Server returns:

Status: 200 OK

HTML page

Images

CSS

JavaScript

------------------------------------------------------------------------

# HTTP Status Codes

Status codes tell whether the request was successful.

  ------------------------------------------------------------------------
  Code              Meaning                      Example
  ----------------- ---------------------------- -------------------------
  200 OK            Request successful           Flipkart homepage loads
                                                 normally

  201 Created       New resource created         New account registered

  301 Moved         Page moved                   Old website redirects to
  Permanently                                    new URL

  302 Found         Temporary redirect           Temporary login redirect

  400 Bad Request   Invalid request              Wrong form data

  401 Unauthorized  Login required               Protected dashboard

  403 Forbidden     Permission denied            Trying to access admin
                                                 page

  404 Not Found     Page does not exist          Wrong webpage URL

  500 Internal      Server problem               Website crashes
  Server Error                                   unexpectedly

  503 Service       Server temporarily           Website under maintenance
  Unavailable       unavailable                  
  ------------------------------------------------------------------------

------------------------------------------------------------------------

# Practical Activities

## Task 1

Open:

-   www.flipkart.com
-   www.myntra.com
-   www.irctc.co.in

------------------------------------------------------------------------

## Task 2

Observe:

-   Header
-   Navigation Bar
-   Main Content
-   Footer
-   Images
-   Buttons
-   Colors
-   Fonts
-   White Space
-   Responsive Design

------------------------------------------------------------------------

## Task 3

Prepare a comparison table.

  Website   Likes   Dislikes   Best Features   Ideas to Reuse
  --------- ------- ---------- --------------- ----------------

------------------------------------------------------------------------

## Task 4

Write short notes on:

-   Internet
-   World Wide Web

------------------------------------------------------------------------

## Task 5

List five web browsers and five search engines.

------------------------------------------------------------------------

## Task 6

Explain:

-   HTTP
-   HTTPS
-   FTP

------------------------------------------------------------------------

## Task 7

Explain HTTP Request and HTTP Response with one example.

------------------------------------------------------------------------

## Task 8

Write the difference between GET and POST with one real-life example
each.

------------------------------------------------------------------------

## Task 9

Explain these HTTP Status Codes:

-   200
-   201
-   301
-   302
-   400
-   401
-   403
-   404
-   500
-   503

------------------------------------------------------------------------

# Common Mistakes

  -----------------------------------------------------------------------
  Mistake               Correct Understanding
  --------------------- -------------------------------------------------
  Internet and WWW are  WWW is a service that runs on the Internet
  the same              

  Browser and Search    Browser opens websites; Search Engine finds
  Engine are the same   websites

  HTTP is secure        HTTPS is secure

  GET and POST are      GET retrieves data, POST sends data
  identical             

  Every webpage returns Different requests can return different status
  200                   codes
  -----------------------------------------------------------------------
