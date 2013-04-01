---
layout: post
title: Multi-lingual websites — A different approach
summary: Once upon a time the world was a well defined, less complicated place than it is today. The Italians lived on a pasta diet, only Japanese people drank sake and the Frisians only spoke Frysk. But things have moved on from here.
avatar: avatar-multi-lingual.png
---

In modern societies, all of the above no longer applies and on the ever expanding world wide web, national borders will look even more trivial tomorrow than today.

Neither the web, nor languages seem to respect the comfort of spatial limitations that national borders used to dictate. Not only have your customers' diet and habits changed, but they may also come from a number of different places. As desirable as the effect of this on the size of your target market may be, there is a downside: you might not share the same customs, currency or even the same language as your customers anymore. The latter will most certainly have a significant effect on the extent of your external communication.

The obvious solution to all this would be to teach all of your customers to speak Mandarin. Yet easier — and much cheaper — solutions are available. One solution is to offer a complete or a concise version of your website in translation to your (potential) customer.

### The trouble with translation

As with teaching Mandarin, the creation and maintainence of multi-lingual sites doesn't happen by itself and *de dato*, websites still do not translate themselves effectively either.

Before you can launch a successful multi lingual website, certain issues need to be addressed, including how the webserver chooses what language to present to the specific end user and how to handle pages that need be launched but have not yet been (fully) translated.

In the year 1517 Martin Luther needed no less than ninety five statements to cause a reformation. I will do my best to address all of the issues mentioned before in the next **eight statements**.

1.  [French isn't French][1] 
 
2.  [Internationalisation is not localisation][2] 
 
3.  [Don't push options, push content][3] 
 
4.  [Make the switch][4] 
 
5.  [Mark your markup][5] 
 
6.  [Dialects matter][6] 
 
7.  [Translation as presentation][7] 
 
8.  [Form follows direction][8] 
 

### The statements

#### French isn't French

Some multi lingual websites offer a language choice at their front page or elsewhere on the website. Certain webbuilders hold on to this awkward tradition of writing the names of all these languages in the main language of that website. E.g.: Suppose I'm a French speaking person who is visiting a website that presents me with English language content. Somewhere on the page I find a drop down menu containing the alternate languages… in English! So looking for Français, I overlook French. Now surely, one wouldn't have the need to look for other than English language content if he understands the English word 'French'. Some people might argue that the word French looks similar enough to Français to be recognised as such by most people. However I'm sure you're not one of these people as we all considered: Dutch vs. Nederlands, German vs. Deutsch or… Persian vs. فارسی, Hebrew vs. עברית or Greek vs. Ελληνικά.

#### Internationalisation is not localisation

Rob is a good friend of mine. He's American, lives in Amsterdam and English is his native tongue. All though he speaks adequate Dutch as well, it's understandable that he likes to read things in his own language. How annoying for him it must be to discover that every other time he visits a website of an international corporation with an .nl domain he is presented with Dutch language content. Even though his web browser is configured well, with English as his first language.

For some obscure reason, a number of web builders assume that one who visits, for instance, a .nl domain, has Dutch as a first language. At the time of writing, a clear example is the website of Sony Ericsson. Sony Ericsson is a company that makes great phones, but learning more about their products can be a real pain if you don't fit exactly into one of their boxes. If you visit [sonyericsson.nl][9], you will only find Dutch language content. Even though most of their content, is available in English as well, but exclusively via the .co.uk domain. Not only is the whole search for the preferred language annoying, if you're interested in finding the nearest dealer or you want to know the local prices, visiting a foreign domain is also hardly helpful either. Unfortunately, Sony Ericsson is in good company, as other big names including: Microsoft, Siemens, Apple, Samsung, Motorola… — well, the list is infinitely long —, make the same mistake, by linking the language content to the domain only.

Information on local dealers, pricing, tax or environmental regulations all have a tight connection to global location. Languages don't, otherwise countries like Switzerland (as you know, Switzerland has 4 official languages) would have multiple domains for their country, except they don't. Therefore, domain spaces could make fine instruments to determine someone's possible location at times, for determining one's language they are less useful.

#### Don't push options, push content

Fortunately many other websites do offer a language choice at some, or any of their domains. Quite often a .com portal or front page is used for this purpose and in that stage the visitor will have to make a choice in which language he would like read the website's content. In my opinion, this is much more elegant than linking the presented language to a domain name, but wouldn't it be even nicer if the right language was selected FOR the user, rather than BY the user? I think it would and the browsing experience would certainly be smoother experience this way than by bothering a potential customer with language– or location questions.

The issue is, how does the website 'know' the preferred language of the site's visitor? Software manufacturers have found an answer to this and so modern web browsers tell what language is preferred. In most cases, this setting is based on the language setting of the system or the software version of the client.

#### Make the switch

Utilising automatic system language detection may smoothen up the visitor's browsing experience to a great extend, yet certain problems may occur:

*   The website's content might not be available in the desired language. Alternatives must be offered somehow. 
 
*   For whatever reason, one may feel the urge to review an article in his second or third language as well. Offering a language choice only at the site's portal or front page would make live switching impossible. 
 
*   Your Lebanese friend — whom you probably communicate with in French — might have launched you a web browser on his Arabic system. It would be desirable to have a choice of switching to another language at any given moment. 
 

Select boxes are widely used for language- or location switchers. A simple list in the sideline of what other languages are available, the way [wikipedia](http://www.wikipedia.org)] does, also makes an elegant solution. The advantage of a simple list on each page is that people have direct visual access to the name of their language at all times. One common mistake to indicate the language choice or to indicate the chosen language is flags. Flags have just as little to do with languages as domain names do. Think about it, with multiple countries where languages such as English, French or Arabic is an official language, what flag to use? Or what to do with languages that have no nationality, such as Roma? There's only one answer to the flag problem: if you can get around them, don't use them.

I will address these and other issues in a [proposed model][11], further below.

#### Mark your markup

Language attributes (e.g. `lang="en-GB"`) are by far not used enough on the web. *Lang* attributes on tags, such as paragraphs and headers that indicate what language is used in the content of the tag, help search engines, such as [Google][12], to determine the language of the content you offer to the world. Applying the *lang* attributes on tags within the body allows you to mix different languages on a page and filter some languages out, or visually highlight others. In the near future, these tags might also help browsers to use the right thesaurus to wrap text and wrap words effectively, which will result in cleaner page layouts.

#### Dialects matter

Another great thing about using language attributes, is that it allows you to not only indicate the language that is used in the content, but also the specific dialect of that language. This way, different dialects of, for instance English, may be distinguised. Separation becomes of much higher importance when individual dialects of the same language differ from each other to a greater extend.

Example: An Englishman, who's client is configured British English, visits a website that offers content in US English and Japanese. Allthough you could make a wild guess and present the visitor with Japanese content, knowing his browser setting, it's more likely that this visitor better understands another dialect of his own language than a completely different language. I suggest to select on exact match first and next, search for alternative dialects.

#### Translation as presentation

We fit our content in the structure of X(HT)ML and manipulate it's presentation using stylesheets and scripts. If there's any desire for changing the graphic design of a page, one replaces the Stylesheet, not the content or the structure, because content is content and not presentation.

The relation between content, structure and presentation could be seen as a triangle, pointing up. On top, there's the content. At one other corner resides the structure and the third corner is host to the presentation as depicted below. The attributes that indicate the language, belong in the corner of the structure. Few would argue that the way the content looks, such as the colour of the words, is part of the presentation of the content.

![Content triangle]({{ site.media }}/magicTriangle.png)

Changing the graphic representation of words doesn't affect their meaning, nor does language. Therefor I propose to conceive language as just *an aspect of presentation* of content as well. So why put different language versions of the same content in different X(HT)ML documents or even in a different databases? Different language versions could just as well be put together in the same document. Each element, such as paragraphs and headers, may be labeled with the appropriate language tag. Either server side (E.g.: XML/XSL) or client side (E.g: XHTML/Javascript) technology may be applied to filter out tags labeled with languages that are not to be presented to the site's visitor.

#### Form follows direction

A switch from a language which is offered in a left to right script (such as Latin), to a right to left script (such as Hebrew), should generally not be done without a layout change as well. The reason for this is, that languages, not written from right to left, are not only aligned right by default, but also have an effect on the visual balance of the page layout. Not changing the page layout to the text direction will result in a page layout which feels unnatural to someone who reads a right to left script, even though it might feel natural to someone who is more used to reading left to right scripts. That's why it's usually not enough to mirror only the alignment of the text. If a website has a sidecolumn, it's often best to move it to the other side as well. Here's an example:

![Latin l2r]({{ site.media }}/latin-l2r.png)

Above, you see the old frontpage of cornae.org in English, using Latin script. Now, we switch to Persian, which uses the Arabic alphabet, without touching the layout. It would look something like this:

![http://www.cornae.com/arabicl2r.png]({{ site.media }}/arabic-l2r.png)

This would look as unnatural to a reader of Arabic script as the example below would to a Latin script reader.

![Latin r2l]({{ site.media }}/latin-r2l.png)

The solution is to mirror the complete page layout. It's recommended to also change the order of tabs and menu items if they're displayed in a horizontal fashion.

The example below shows a mirrored page layout, opposed to the layout that was used for Latin script languages. Mind the small details, such as the find button, which moved to the left of the search box. Also the minus- and plus signs of the sidebar widget headers moved to the other side and even the order of the fruit buttons to make it complete.

![Arabic r2l]({{ site.media }}/arabic-r2l.png)

Different stylesheets may be used to present the pages using the proper layout, without having to touch the structure of the pages.

### The proposed model

As I prefer to provide you with answers, — rather than leaving you with more questions than you had before reading this article — I will propose a concrete model on which all of the above is applied.

<p class="geekAlert"><strong>Nerd alert</strong><br/> <em>The now following information might be of a technical nature.</em></p>

The model, as proposed below, is based on XHTML pages of which each page contains all of the available languages for that document. Tags containing text or other language sensitive content are labeled with language tags, such as applied on a the paragraph in English, Italian and French, shown in the example below:

	<p lang="en-GB">
	  This is a multi lingual website. Despite all efforts it might occur that a certain page is not (completely) available in your preferred language. My apologies for the inconvenience.
	</p>
	<p lang="it-IT">
	  Questo è un sito multilinguistico. Malgrado tutti i miei sforzi potrebbe accadere che una determinata pagina non sia completamente disponibile nella vostra lingua. Mi scuso per il disagio.
	</p>
	<p lang="fr-FR">
	  Ceci est un site multi-lingue. Malgré les efforts il est bien possible que certains pages ne sont pas dans leurs totalités disponibles dans votre langue préférée. Veuillez nous excuser.
	</p>    

By means of a javascript, all non desired languages are filtered out of the visible part of the DOM-tree. This is what enables any visitor to perform live language switching without generating any extra line traffic. One might argue that sending all non needed languages over the line results in unnesecary line traffic anyway. We're talking however, merely plain text in most cases. There's is a curve where a new ip-request a document in another language would result in larger waiting time than would be the case with downloading one, slightly larger file. There's also room to play with the order in which languages are taken up in the structure. On way of building the structure is by adding all the content for all languages first and next all the content for the next language, etcetera, showing here:

    
	<h2 lang="en-GB">
	  Multi lingual websites:<br/>
	  a different approach
	</h2>
	<p lang="en-GB">
	  Once upon a time the world was a well defined, less complicated place than it is today. The Italians lived on a pasta diet, only Japanese people drank sake and the Frysians only spoke Frysk. But things have moved on from here.
	</p>
	<p lang="en-GB">
	  In modern societies, all of the above no longer applies and on the ever expanding world wide web, national borders will look even more trivial tomorrow than today.
	</p>
	<h2 lang="nl-NL">
	  Meertalige websites:<br/>
	  een frisse blik
	</h2>
	<p lang="nl-NL">
	  Ooit was de wereld wonderbaarlijk overzichtelijke planeet. De Italianen aten pasta, alleen de Japanners dronken sake, Amsterdammers spraken Nederlands en de meeste Amerikanen hadden geen paspoort. De tijden zijn echter radicaal verander
	</p>
	<p lang="nl-NL">
	  In de hedendaagse samenleving is al het bovengenoemde niet meer van toepassing en op het immer uitdijende internet zullen nationale grenzen morgen van nog kleinere betekenis lijken dan vandaag.
	</p>
    

One may as well choose to group all language versions of the first element together in succession all the languages for the next element, etcetera, like demonstrated the example below:

    
	<h2 lang="en-GB">
	  Multi lingual websites: <br/>a different approach
	</h2>
	<h2 lang="nl-NL">
	  Meertalige websites: <br/>een frisse blik
	</h2>
	<p lang="en-GB">
	  Once upon a time the world was a well defined, less complicated place than it is today. The Italians lived on a pasta diet, only Japanese people drank sake and the Frysians only spoke Frysk. But things have moved on from here.
	</p>
	<p lang="nl-NL">
	  Ooit was de wereld wonderbaarlijk overzichtelijke planeet. De Italianen aten pasta, alleen de Japanners dronken sake, Amsterdammers spraken Nederlands en de meeste Amerikanen hadden geen paspoort. De tijden zijn echter radicaal veranderd.
	</p>
	<p lang="en-GB">
	  In modern societies, all of the above no longer applies and on the ever expanding world wide web, national borders will look even more trivial tomorrow than today.
	</p>
	<p lang="nl-NL">
	  In de hedendaagse samenleving is al het bovengenoemde niet meer van toepassing en op het immer uitdijende internet zullen nationale grenzen morgen van nog kleinere betekenis lijken dan vandaag.
	</p>  

The latter method has the advantage that the first paragraphs of each language will be drawn at more or less the same time. The visitor can already start reading the first lines while the rest of the content is still loading, regardless of his preferred language. The drawback is, that users of less advanced mobile readers, will have to scroll after reading each paragraph. Still, all content is availble to them.

### The flow

In a few easy steps, your customer will be presented with the intended content, without even noticing that some magic has occurred in the client or on the server.

#### STEP 1: Get the languages of the page

Every time a page is loaded the script will detect what languages are used on the page by recursively detecting all the elements within the DOM-tree that are equipped with a *lang* attribute and build a list of all the different lang values that are used on the page. Next, all the different options will be added to a select box using real names of the languages. The script will locate and identify the select box by it's unique ID. A cross reference table is embedded in the script to link the real language names to the iso codes.

#### STEP 2: Get information from cookie

Each time the select box is set to a another value, this value will be stored in a cookie on the visitor's system. If a cookie is available, the script will look whether this preferred language is available on the page. If so, the select box will be set to that language and all other languages will be filtered out of the DOM-tree. All other steps are now skipped. In case the cookie language is not available on the page, it will check the client language.

#### STEP 3: Sniffing the client's preferred language

Browsers declare the user's language first and second the preferred local dialect using [iso 639](http://www.sil.org/) codes of 2 or 3 digits each. E.g.: American English = en-US. 'Some systems' are less correct in announcing the language code as they could be and they will only state the language itself, not the preferred dialect of that language.

If you don't know your client language, find out about it with this [language check][19].

An extra function may be added to the script which looks for alternate dialects of the desired language, before looking for another language.

Next the script will check if the browser language is available on the page. If it is, then the select box will be set to that language and all other languages will be filtered out of the DOM-tree. All following steps are now skipped.

#### STEP 4: Get first language used on page.

If the browser language is not available on the page, then the script will make a decision of it's own, based on the value of the very first *lang* attribute that's found on the page. To this language the select box will be set and all other languages are filtered out of the DOM-tree.

This whole process as described above, is illustrated below. The flow chart is also available as a [pdf-file]({{ site.media }}/language-switcher.pdf).

![Language]({{ site.media }}/Language-switcher.png)

### Addendum

In this model, all the actual filtering takes place within the client, with some great advantages to it, including live switching, search engine friendliness and no need for complex server side technology. The application of Unicode permits you to mix every possible character system in one page. But of course, nothing keeps you from using the same technology for a server side language filter. If your pages derive from XML files, the same *lang* attributes may be applied to the XML. Another mechanism can used to filter out the unwanted languages for a certain request while generating the page.

For websites that generate large amounts of traffic every day, the latter method would probably be a fair option. For somewhat smaller scale websites, or websites for which no multi lingual content management system is on for hand, the client side model could more than well fit your needs.