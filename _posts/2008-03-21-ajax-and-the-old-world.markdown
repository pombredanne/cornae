---
layout: post
title: AJAX and the old world
summary: Today, complex layout methods have made it possible to borrow from interaction patterns of desktop applications, including drop down menu bars, expanding trees and tabs. It's this exact inevitable shift of desktop application design patterns to the page metaphor that has more than often led to confusion amongst both web designers and end users. 
avatar: avatar-ajax.png
---

AJAX and the old world

Most of us know that HTML was designed in such a way that it would enable one to (single) click on certain underlined words in a text, that would link to another page. Initially, these hyperlinks were the only clickable items on web pages. Soon enough, besides using hyperlinks in an inline fashion, they would be grouped on pages so they would form a menu which would help people to navigate between pages that belonged to a certain group of pages. The web site was born.

![Illustration]({{ site.media }}/Ajax-suicide.png)

Today, complex layout methods have made it possible to borrow from interaction patterns of desktop applications, including drop down menu bars, expanding trees and tabs. It's this exact inevitable shift of desktop application design patterns to the page metaphor that has more than often led to confusion amongst both web designers and end users. In this era of AJAX and RIAs, the possibilities for user interface designers have become infinite. Hence the question arises: Have all of these developments actually led to an improved user experience?

By means of a small number of examples will I try to give some convenient rules of thumb to all of the disciplines mentioned above and challenge you to join the community in standardising new patterns for some of the open ends.

## Example: Hands and arrows

From the early days on, graphical web browsers have borrowed the appearance rules of mouse cursors from the desktop application environment. One new cursor was introduced however: the hand cursor with an index finger pointing up. As we all know, this cursor is always displayed when the end user hovers over a hyperlink. As mentioned before, HTML hyperlinks are used for a lot more things nowadays than merely plain, inline underlined text links. Menu items and even buttons are sometimes just HTML hyperlinks in disguise. Which cursor should web designers choose in those situations where hyperlinks are used for something that doesn't look like a hyperlink. Hand cursor or arrow?

The key to the answer to this problem lays in the fact that one shouldn't look at what the interface element looks like, nor to which HTML element is used in the code to create the interface element, but instead to what the element does. From the early days of graphical browsers on, a hand cursor have indicated to the user that on clicking, they would jump to another piece of information or even a whole new page, so this is also what the end user expects. It's recommended to make sure that interface elements that function as menu items always feature a hand roll over.

An exception to this rule of thumb is the submit button. Forms generally feature a submit button. Hitting the submit button usually makes the server return another web page, for instance with a confirmation message saying that the form was sent successfully. Even though this interface element seemingly 'links' to another page, the actual intention of the end user was in this case never to call for another page, but rather to issue the form that he filled out. Hence a hand cursor would only cause confusion in cases like this. Even in a case where a submit button doesn't look exactly like an average button.

## The trouble with drop down menus

Drop down navigation menu bars usually display their children elements on a mouse over event on the parent element. As the `<a>` (link) element is often used — and should be used — for navigation, the hand cursor on mouse over events is automatically inherited. In many cases, the items in such menus are neither blue, nor underlined. In other words, they don't even remotely look like anything that would obviously link to another page. Nevertheless, few end users seem to have any kind of trouble with the result of being linked to another page after clicking on one of the menu items, as the hand cursor doubles as a sort of warning to the end user that a bigger change is going to happen.

In desktop applications, the parent items of a menu never initiate any kind of action themselves when the user clicks on them. It's always the children elements of them that have that kind of power. However doubtful it is that you would want to put a menu bar on a web page or RIA that behaves exactly the same as their desktop brothers would, it's not unthinkable that in certain cases one would need to build a navigation tree or a navigation menu bar (or a functions menu bar for that matter) in which the items are grouped. If these groups don't represent a specific page or piece of information themselves, then it's probably less desirable to put a hand cursor on the roll over states of the parent/group items, as the user might expect this item to link to a complete new page itself. The closer your metaphor is to the metaphors we use for desktop applications, the more likely it is that hand roll overs won't add anything positive to the user experience, nor would action on roll over. Use clickable items instead.

### It's all in the clicking

Certain elements that expand on a single click do not necessarily lead to another page. Examples of this are accordions or collapsible widgets. Even though clicking on one of these items might not result in a hopping to a totally different screen, still a fair amount of information is collected or revealed to the end user. Hand cursors are not absolutely necessary here, but may sometimes be useful to indicate to the end user that an object is clickable. Especially if roll overs states of the element itself are not available.

### Rule of thumb for cursors

As I mentioned before, neither the markup, nor the visual design should be leading for the choice of cursor. User interface designers will have to determine the pattern of the user interface model and decide whether a hand cursor is in place or not. By consequence,  the user interface design should be the leading subject for cursor choices during the designing process and not the visual design or any markup choices. Though ideally, the markup should follow this decision and where possible, the link element should only be used for jumping to another piece of information. Regardless whether this takes place on the same page, by means of an AJAX call or more traditionally by linking to a new document. Using link elements for headers of expandable widgets and accordions is therefor forgivable. But for initiating a function, such as for instance a button which says 'add another item to this list', an input of the type 'button' will usually be more appropriate. In these cases, it's hardly ever recommendable to apply a hand cursor on roll over.

Bear in mind that end users do expect a button also to look like a button. A slight bevel and/or rounded corners have proved to be solutions which end users understand. For user interface patterns that are very well embedded in the end user's mind, a visual designer may want to take a higher risk. E.G.: The end user will generally already expect anything next to a box that is labelled 'search', that just remotely looks like a button, to be a button which will initiate the search call.

Perhaps it is needless to say that in case of a possible doubt if the end user will understand that a certain object is clickable; a (subtle) roll over state will always encourage him to click on the item.

The given rule of thumb of 'don't base your choice of cursor on what the user interface element looks like, but rather on what it does', should also be applied to other cursors, such as resize cursors or drag and drop cursors. Do bear in mind that these cursor types are newer to the page metaphor than all of the other cursors mentioned before and lean much heavier on the metaphors that we know from the desktop application world.

## Example: A step back

One of the new big challenges the web 2.0 has to overcome is something as trivial as accommodating a browser's page back function. The single page interface is a fact and since browsers don't really 'know' what goes on on a page, a single hit on the page back button might mean that the end user hasn't gone one step back in the process of what ever he was doing, but he might unwillingly be thrown out of the application, sales process and so on all together.

Site designers have acknowledged this problem and have overtime come up with several solutions.

### Blocking page back

On of these solution is blocking the browser back function by means of a fairly simple Javascript. My verdict: pure evil. Just don't.

### Page embedded back and forward navigation

Some designers of RIAs have opted for including back and forward navigational items on the page itself. In this way, one gains full control over the back and forward history. The trouble is that many end users — even when they're already used to the RIA's interface — manage to click on the browser back button before they realise — or understand — that they should have used the back button RIA itself instead. Who would blame them, as they've been clicking on that button for years. It seems just too confusing for the average end user to work with two sets of back and forward buttons.

### Brad Neuberg

Merely blocking — and therefor controlling — the end users navigational buttons doesn't really help. Yet, there's no harm in helping the web browser a little in maintaining it's browser history path. Brad Neuberg created a nifty script to take care of this and it's called: [the Brad Neuberg Framework](http://web.archive.org/web/20080401133554/http://codinginparadise.org/weblog/2005/10/really-simple-history.html).

## Example: Bookmarks

### Bookmarking RIAs

In old style web applications, the bookmark already wouldn't do much for you. With today's RIAs that use AJAX designers are facing even bigger challenges.

Picture an end user — called Jack — who is half way an online sales process for buying a ski outfit. Just as he clicked through a number of pages on which he decided on the right colour and style for his outfit and which shoes to go with it, the phone rings. It's mum. Jack is well aware that a phone call with mum seldom takes less than thirty minutes. As Jack wishes to continue later, he bookmarks the screen he is currently on and closes his browser.

No less then one and a half hour later Jack knows all about mums health, how well her magnolias are doing and that she can feel in her bones that winter is arriving. Which reminds him of the fact that the process of purchasing a ski outfit was still left unfinished. Hence, he turns back to his computer and opens the bookmark in order to find out that he hasn't bookmarked a near to end stage of his purchasing process, but just the main address of the application itself. All the labour that went into carefully assembling his ideal ski outfit turned out to be in vain and bad memories of late 90's frames websites come back to him.

Whereas traditional commerce engines generate urls that would at least roughly point at a certain section of the commerce path where the end user ended up upon, modern AJAX applications often won't leave the end user — nor the web browser — with a single hint where he's at, let alone what he has put in his shopping bag (although luckily this is usually solved with cookies).

This problem won't only occur with the use of AJAX for commerce engines, but also with other types of AJAX enabled products.

The core to this problem is not the technology that is used itself, but rather the way in which people design these applications. For designers, it might be helpful to consider the following:

**Manage to determine for every change on the screen that was caused by user intervention, whether this change is radical enough, to be considered a new page/screen by the concerned end user himself.**

If the latter is the case then a designer should communicate to developers which screens are there to be distinguished rather than leave this to the judgement of a programmer.

The same rule of thumb also helps to write a navigation flow for your AJAX application or site and even story boarding may become easier this way.

## Conclusion

We live in a time where the traditional disciplines of visual design/user interface design and front end engineering are blending with each other. More and more are logic and behaviour moving from server side to client side. This means that designers can no longer do with basic wire-framing and slick looking Photoshop composites alone if they want to keep enough control over not only what a user interface looks like, but also over what it does in order to guarantee the best user experience. My suspicion is that IF visual designers, engineers and most of all user experience specialists are aware of all the technical possibilities, the history of each design pattern and their intended use then more fabulous products than ever will appear on the horizon.

### Prototyping

Now is the time that designers and front end engineers should work closer together and learn from each other's disciplines. If designers stay behind, then they won't be able to specify what they have in mind exactly. Add this to the fact that software is nowadays often built in another place from where it was designed and it becomes clear that building advanced and realistic looking prototypes has become a crucial factor in specifying one's wishes in detail.

To be able to create realistic looking prototypes which need no explanation to developers and ultimately hardly any specification documents. The market will more and more desire a fair amount of knowledge of every aspect of user interface building from all disciplines to guarantee consistent, compliant and accessible user interfaces.

Web standards have brought us great things. For most types of content such as paragraphs, headers, tables, etc., it is clear to most disciplines which tag to use, how to style CSS and which visual style features may be applied. If the industry would have adopted web standards early enough, then there would have been room for W3C to develop updates for standards more rapidly. These new versions of standards of — mainly XHTML — might even have offered tags and application rules such as `<navigation><item>Menu item</item></navigation>`, `<input type="search" />`, `<input type="combobox" />`, `<input type="slider" />`, and so forth. And with tags that follow user interface design patterns as closely as this, browsers would have grown to respond to these tags in a equal fashion. Looking back, it's clear that (the acceptance of) standards have always been behind on trends in user interface engineering. User interface designers/engineers maintain an ongoing search for other methods to reach their goals, which is where the inconsistencies in patterns derive from.

### Patterns

This only shows that the application of CSS, Javascript and especially HTML in the way they were intended is more important than ever. But what to do when they don't fulfil our needs directly? The answer is patterns. What the world needs right now is more clear patterns in user interface engineering for — in particular AJAX — user interfaces. The solutions to problems with patterns offered earlier in this article would only be a taster of the latter. How desirable it would be if end users would find it just as obvious when to use the back button, when the application is collecting data or just stuck, how to navigate, etc., as the fact that hyperlinks are underlined. This may be reached sooner when designers keep a close eye on each other's ideas, but more importantly: on what their end users like and understand.

