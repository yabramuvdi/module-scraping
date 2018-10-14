# Scraping

---

## Scraping

Scraping consists of: 

1. Making HTTP requests to servers for HTML content. 
2. Parsing that HTML content to: 
   1. Store desired information.
   2. Find links to follow (for each link, go back to 1.)

---

## Making HTTP Requests

Browsers make HTTP requests. 

Every major programming language also has a way to make HTTP requests. 

This is sometimes done via a third-party library. 

---

## Parsing HTML

HTML parsing is something you will use a trusted library for. 

HTML parsers, in every language, will take the raw HTML from an HTTP response, and turn it into a (usually custom) tree-like data structure or class that you can easily traverse, and from which you can easily extract the desired content. 

This functionality is completely separate from that of making the HTTP request. It will usually be included in a separate library, for this reason. 

You will need to learn the API, the interface, of the HTML parser you are using! 

Read the documentation.

---

## Following Links

The interesting part of scraping comes in deciding how to follow links. We will split crawling, and scraping, into two types: 

* Broad crawling
* Narrow crawling

---

## Broad Crawling

Broad crawling is what Google does. 

It consists of following ALL links on EVERY page in order to discover all the content on the web. 

We will not focus on broad crawling. 

---

## Narrow Crawling

We will focus on the use-case where: 

* You have one website you want to crawl
* The website has a particular structure that you know and expect to stay consistent (big assumption!)
* You want to grab a specific set of data from this single website. 

---

## Collecting Links


---
