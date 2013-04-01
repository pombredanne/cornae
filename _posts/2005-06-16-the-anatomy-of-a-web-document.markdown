---
layout: post
title: The structure of xHTML
summary: An article on the usage of (x)HTML and the application of the Document Object Model (DOM).
avatar: avatar-anatomy.png
---

## The Document Object Model

Do you remember the time as well I do, in which it was so utterly difficult to make things looks equally the same in a user agent such as Netscape Navigator as in Microsoft Internet Explorer? The usual strategy was to just optimise a website for one certain web browser. This has eventually, because of their rapidly growing market share, worked out to the advantage of Microsoft. This way all problems seemed te be solved. Yet, it's still annoying to be constantly dependent of one particular browser vendor. This is also what Tim Berners Lee of [the World Wide Web Consortium (W3C)][1] must have thought. For that reason the W3C stated a number of recommendations, in which he describes how language, such as (X)HTML and CSS aught to be interpreted by any web browser and how web developers should apply them. Furthermore, the W3C has suggested a model that describes how content on page should be put in so called 'objects' within a logical tree-structure, called the document tree. This model, called the Document Object Model (DOM), enables web browsers to manipulate the presentation of all these objects independently by means of (Java)scripts en styling languages. This collection of recommendations is often referred to as *the web standards*.

Where as in old times the code of web pages consisted of text mixed with layout information. In modern times, a document that is constructed by the rules of the DOM method, consists of objects, or elements, brought together in a tree structure. This way the content becomes a property of the element, rather than the other way around and thus plays an inferior role towards the structure of the document.

## The Document structure

By the rules of the DOM, each document is split up in roughly two parts: 'head' and 'body'. The element head contains information on the content of the document. The element body contains all information intended to be presented to the end user.

The animation below ([Apple Quickitme](http://www.apple.com/nl/quicktime/download/) required) explains the structure of the DOM with an abstract model.

<video>
	<source="{{ site.media }}/structure-of-xhtml.mov" />
	<a href="{{ site.media }}/structure-of-xhtml.mov">Video the structure of xHTML</a>
</video>

The language that's been used on the internet for the creation of these documents is the well known HTML-format. HTML, which means 'Hypertext Markup Language', was born in the seventies out of the wish to link individual text documents together by assigning the addresses of other documents to certain words. This concept is well known as 'hyperlinking'. Over the years, a number of different versions of the HTML standard have succeeded each other to meet the growing desire for web pages with more advanced scripting possibilities and complex graphical layouts.

## xHTML

The HTML version that makes the best out of the Document Object Model is the [XHTML family][2]. [Elsewhere on this site][3] you may read what requirements an XHTML-document needs to meet and how to structure it.

## Other recent articles:

*   [![Dealing with Labels][5]][5] 
    ##### [Dealing with Labels][5] by Cornelis G. A. Kolbach — February 1, 2009 
    
    As suggested in the article [Form Follows Function and Achieving Thereof][6], every input element on a form should ideally have a label. Labels give more meaning to input elements and makes them accessible. This article dives into dealing with labels and input fields for postal addresses on forms.
    
    [Read more...][7] 
*   [![Form follows function and achieving thereof][9]][9] 
    ##### [Form follows function and achieving thereof][9] by Cornelis G. A. Kolbach — February 1, 2009 
    
    Forms can be dreadfully tricky to style and structure properly. Several articles that are out there focus on best practises for building forms using HTML en CSS. This article focusses in a non technical fashion on the use of meaningful nomenclature and how form semantics relate to elements that current markup standards have to offer. It may help you recognise structural patterns and to compose forms properly.
    
    [Read more...][10] 
*   [![ Gregorian date input diversity ][12]][12] 
    ##### [ Gregorian date input diversity ][12] by Cornelis G. A. Kolbach — February 1, 2009 
    
    One of the most common interaction patterns one can find on forms is the date input group. They appear in all shapes and sizes in various applications and sign up forms on websites. Certain forms of appearance seem to be more popular in certain geographical areas than other. But other than that it is hard to find any pattern or rationale why one website has chosen for model X while the other has chosen model Y. The suspicion would rise that the date input method is often dictated by the way the backend would 'like' it. This is a situation which neither we, as interaction designers and consultants, nor the end user should settle for.
    
    [Read more...][13] 
*   [![AJAX and the Old World][15]][15] 
    ##### [AJAX and the Old World][15] by Cornelis G. A. Kolbach — November 19, 2006 
    
    Most of us know that HTML was designed in such a way that it would enable one to (single) click on certain underlined words in a text, that would link to another page. Initially, these hyperlinks were the only clickable items on web pages. Soon enough, besides using hyperlinks in an inline fashion, they would be grouped on pages so they would form a menu which would help people to navigate between pages that belonged to a certain group of pages. The *web site* was born.
 
    
    Today, complex layout methods have made it possible to borrow from interaction patterns of desktop applications, including drop down menu bars, expanding trees and tabs. It's this exact inevitable shift of desktop application design patterns to the page metaphor that has more than often led to confusion amongst both web designers and end users. In this era of AJAX and RIAs, the possibilities for user interface designers have become infinite. Hence the question arises: **Have all of these developments actually led to an improved user experience?**
    
    [Read more...][16] 

* * *

 [1]: http://www.w3c.org
 [2]: http://www.w3.org/MarkUp/
 [3]: http://www.cornae.com/articles/the-structure-of-xhtml
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