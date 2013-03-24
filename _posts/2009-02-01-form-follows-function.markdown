---
layout: post
title: Form follows function and achieving thereof
summary: Forms can be dreadfully tricky to style and structure properly. Several articles that are out there focus on best practises for building forms using HTML en CSS. This article focusses in a non technical fashion on the use of meaningful nomenclature and how form semantics relate to elements that current markup standards have to offer. It may help anyone to recognise structural patterns and to compose forms properly.
avatar: avatar-forms.png
---

## Form Building Blocks

All input elements on a form must be tagged with labels. Labels describe what type of information the form may contain.

![Illustration](Vioolsleutel-illustratie.png)

All input elements on a form should also be logically grouped in field sets. A field set is a group of form elements that are related towards each other. For instance a yes/no answer with radio buttons or an address input fields group.

The subject of the field set may be marked by means of a legend. A legend describes a group of form elements that are contained within a field set.

In retrospect it could be said that there is the following list of most important building blocks for forms:

- Input elements (Free-form input fields, text areas, radio buttons, etc.)
- Labels
- Legends
- Fieldsets

This article strives to elucidate which element has to be used when.

There are basically two types of forms. Vertical forms and horizontal layout forms.

Simple forms are the old fashioned type of forms that are popular for smaller patterns, such as a login dialogue.

Horizontal forms have a bit more layout to them. This often means that the form is divided into two imaginary columns. There's each time a question on one side and one or more answers, or input fields for the answers, on the other side.

### Horizontal forms

The following example displays a complex layout for where there's each time a short question on the left and room for an answer on the right. These questions are related towards each other and therefore grouped in a field set and tagged with a legend that says 'Personal Information'.



Question doesn't mean that it looks 100% like a question sentence that ends with a question mark, but that it semantically IS a question. The author of the form is simply asking the user for all this information in the most concise fashion. This makes the short questions on the left hardly anything more than labels of the input fields, which is the reason that most site editors would choose the following structure of form elements to push the baby out:



The chosen structure creates a nice little form. I like to call this type of field set the Concise Form Pattern. So far so good. But… now I dare challenge you to apply a similar structure to the following example.



If Name, E-mail and Phone Number are labels as established before, then the Gender question would be a label as well. But then the answers Male, Female and Not sure couldn't be labels any longer, because the XHTML specification reads: "Each label must not contain more than ONE field. Label elements shouldn't be nested."

The only form element that's left to use is legend. Since the current group of elements already has a legend, the radio buttons should be grouped in a field set inside the existing field set. The structure would look like this:



I like to call the pattern that has a legend on the left and the answers on the right the Comprehensive Form Pattern. The example above is a combination of the concise and the comprehensive pattern.

### Vertical forms

Simple forms don't differ from complex form by structure, only by layout. This is an example of a simple form:



The diagram below demonstrates how the universal structure of this form doesn't differ in any way from the complex form. I call this layout the Condensed Form Pattern.



## Judge the Things by What They Are

What becomes clear in this story is that visual layout of a form doesn't have to influence the structure of it. In a complex layout form, the things that are positioned as questions that are positioned on one side of the form may be labels, legends, or a mixture of both. The same principle applies to simple layout forms. The differences are merely cosmetic.

A clear and shared nomenclature of form elements based on what things are, rather than what they look like, helps multi disciplinary teams to work more efficiently and to build lean products using reusable and highly maintainable building blocks.