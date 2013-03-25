---
layout: post
title: Dealing with labels
summary: As suggested in the article Form Follows Function and Achieving Thereof, every input element on a form should ideally have a label. Labels give more meaning to input elements and makes them accessible. This article dives into dealing with labels and input fields for postal addresses on forms.
avatar: avatar-label.png
---

A great example of a pattern that really requires the application of visible labels is the postal address entry. Postal address entries may easily contain four, five, or more fields to fill out. The many fields often lead to forms that are lengthier than necessary if all the labels are kept on the left. Another disadvantage of the left-label-layout is that it's far off of the layout of postal addresses on envelopes and letters in the real world.



If you make the layout of the address group more compact by mimicking a traditional postal address layout, then it will make the form more compact. More importantly: People will be able to fill you an address information in the same fashion they are used to on a postcard. Almost without looking at the labels.

This doesn't make visible labels completely obsolete though. In the example below, a Dutch address layout is applied. Imagine that you would like to send a nice bouquet of flower to your favourite blogger in The Netherlands. But if you've never lived in The Netherlands, then you're not likely to be familiar to this layout. Hence the use of visible labels will be helpful.



Putting all the labels as superscripts in between the input fields and the term 'Address' as a legend on the left is a great improvement for the layout, but there is an alternative that's even more compact, which I like to call superimposed labels.



Some implementations of this interaction pattern do just pre-fill the values of the input fields with the terms Residence, Street, Postal Code, etc. This is semantically incorrect, because 'Residence' is not a valid value for the field that's called Residence unless there is a place on this planet that is called 'Residence'. A practical issue is that the backend would always receive this value back as a place name, rather than for instance 'Amsterdam'. The backend would have to check whether this field's value is not called "residence" rather than simply checking whether a field was filled out at all for validation purposes. Extra site languages could even further complicate this matter.

## The super imposed label solution

The terms street, postal code and son on are labels more than anything else. These labels are positioned in front of the labels by means of CSS and triggered to disappear by a little bit of JavaScript code. The particular feature of these labels is that they disappear upon the click of a mouse. The terms will remain invisible after the user entered text into the field. Would the user move the focus to another element without filling in anything would return the label. It's an elegant pattern that saves space on the screen while labels are properly applied for all the right reasons.

## HTML placeholders

The HTML 5 standard has a solution built in for this, but not with the use of labels, but a certain attribute called 'placeholder' instead. The markup looks like this and it works in most modern browsers:

<input type="text" placeholder="residence" />
If this pattern is picked up quickly by screen readers, then it will become an accessible solution. For now, of all major browsers, only Internet Explorer (9) does not support the pattern. The IE problem could be fixed with a bit of JavaScript that fills in the value of the input field based on the value of the placeholder attribute and to erase that just before submitting the form if it hasn't been altered by the user.

