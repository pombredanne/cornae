---
layout: post
category: articles
title: Anatomy of a (web) document
summary: An article on the usage of (x)HTML and the application of the Document Object Model (DOM).
avatar: avatar-anatomy.png
---

## The Document Object Model

Do you remember the time as well I do, in which it was so utterly difficult to make things looks equally the same in a user agent such as Netscape Navigator as in Microsoft Internet Explorer? The usual strategy was to just optimise a website for one certain web browser. This has eventually, because of their rapidly growing market share, worked out to the advantage of Microsoft. This way all problems seemed te be solved. Yet, it's still annoying to be constantly dependent of one particular browser vendor. This is also what Tim Berners Lee of [the World Wide Web Consortium (W3C)][1] must have thought. For that reason the W3C stated a number of recommendations, in which he describes how language, such as (X)HTML and CSS aught to be interpreted by any web browser and how web developers should apply them. Furthermore, the W3C has suggested a model that describes how content on page should be put in so called 'objects' within a logical tree-structure, called the document tree. This model, called the Document Object Model (DOM), enables web browsers to manipulate the presentation of all these objects independently by means of (Java)scripts en styling languages. This collection of recommendations is often referred to as *the web standards*.

Where as in old times the code of web pages consisted of text mixed with layout information. In modern times, a document that is constructed by the rules of the DOM method, consists of objects, or elements, brought together in a tree structure. This way the content becomes a property of the element, rather than the other way around and thus plays an inferior role towards the structure of the document.

## The Document structure

By the rules of the DOM, each document is split up in roughly two parts: 'head' and 'body'. The element head contains information on the content of the document. The element body contains all information intended to be presented to the end user.

An [animation]({{ site.media }}/structure-of-xhtml.mov) in  [Apple Quicktime](http://www.apple.com/nl/quicktime/download/) format is available to illustrate the structure the DOM by mean of an abstract model.

<!--The animation below ([Apple Quickitme](http://www.apple.com/nl/quicktime/download/) required) explains the structure of the DOM with an abstract model.-->

<!--<video><source="{{ site.media }}/structure-of-xhtml.mov" /><a href="{{ site.media }}/structure-of-xhtml.mov">Video the structure of xHTML</a></video>-->

The language that's been used on the internet for the creation of these documents is the well known HTML-format. HTML, which means 'Hypertext Markup Language', was born in the seventies out of the wish to link individual text documents together by assigning the addresses of other documents to certain words. This concept is well known as 'hyperlinking'. Over the years, a number of different versions of the HTML standard have succeeded each other to meet the growing desire for web pages with more advanced scripting possibilities and complex graphical layouts.

## xHTML

The HTML version that makes the best out of the Document Object Model is the [XHTML family][2]. [Elsewhere on this site][3] you may read what requirements an XHTML-document needs to meet and how to structure it.

 [1]: http://www.w3c.org
 [2]: http://www.w3.org/MarkUp/
 [3]: {{ site.baseurl }}/2005/06/16/the-structure-of-html.html
 []: http://www.cornae.com/articles/dealing-with-labels
 [5]: http://www.cornae.com/articles/dealing-with-labels
 [6]: http://www.cornae.com/form-follows-function-and-achieving-thereof "Legends of the Form"
 [7]: http://www.cornae.com/articles/dealing-with-labels
 []: http://www.cornae.com/articles/form-follows-function-and-achieving-thereof
 [9]: http://www.cornae.com/articles/form-follows-function-and-achieving-thereof
 [10]: http://www.cornae.com/articles/form-follows-function-and-achieving-thereof
 []: http://www.cornae.com/articles/gregorian-date-input-diversity
 [12]: http://www.cornae.com/articles/gregorian-date-input-diversity
 [13]: http://www.cornae.com/articles/gregorian-date-input-diversity
 []: http://www.cornae.com/articles/ajax-and-the-old-world
 [15]: http://www.cornae.com/articles/ajax-and-the-old-world
 [16]: http://www.cornae.com/articles/ajax-and-the-old-world  