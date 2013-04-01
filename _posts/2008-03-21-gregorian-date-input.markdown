---
layout: post
category: articles
title: Gregorian date input diversity
summary: One of the most common interaction patterns one can find on forms is the date input group. They appear in all shapes and sizes in various applications and sign up forms on websites. Certain forms of appearance seem to be more popular in certain geographical areas than other. But other than that it is hard to find any pattern or rationale why one website has chosen for model X while the other has chosen model Y. The suspicion would rise that the date input method is often dictated by the way the backend would 'like' it. This is a situation which neither we, as interaction designers and consultants, nor the end user should settle for.
avatar: avatar-date-notation.png
---

## International Formats

A part of the problem is that designers are often faced with international visitors to their websites. Different geographical regions  have their own popular format. Please find an incomplete list of popular formats below.

#### ISO 8601 International Date Format

- 2008-12-31(ccyy-mm-dd)

The international date format is adopted by several countries. Many people around the globe have never used this notation however.

#### United States of America

- 12/31/2008 (mm/dd/yyyy)
- December 31, 2008
- 31 December 2008
- 31-Dec-2008

The month/day/year order is **unique** to the USA, Canada and the Phillipines.

#### United Kingdom

- 31/12/2008 (dd-mm-yyyy)
- December 31st, 2008
- 31st of December 2008
- 31 December 2008

#### Kingdom of the Netherlands

- 31-12-2008 (dd-mm-yyyy)
- 31-12-'08 (dd-mm-yy)
- 31 december 2008

#### Greater China

- 2006年01月29日

The international date notation is popular in China. Chinese characters are often used for the words for year, month and day.

#### Norway

- 31&#46;12&#46;2008 (dd&#46;mm&#46;yyyy)  
- 31/12-2008 (dd/mm-yyyy) (used in handwriting, usually without the year attached)  
- 31&#46; desember 2008  

Of all the different formats above, only one notation is used in nearly all of these countries: **31 December 2008**.

![Aztec Calendar]({{ site.media }}/Aztek-Calendar.png)

> The Aztec calendar was the calendar of the Aztec people of Pre-Columbian Mexico. It is one of the Mesoamerican calendars, sharing the basic structure of calendars from throughout ancient Mesoamerica. The Aztec calendar was the most precise calendar until the arrival of computers.

## Input methods

I'll summarise the three most common methods:

### The single field pattern

dd-mm-yyyy

Many interaction designers are an advocate of the single field form. The valid argument for this is that users don't have to click or tab more than necessary and that the backend could filter out zero based notation, dashes, dots and so forth, in order to save it the right format. A user instruction is often placed next to the input field in order to make sure that users will always enter the month as either a number, or as a name.

#### Disadvantages:

User has to read instruction
User will copy dashes or other separation characters, even if not necessary for processing
Date syntax doesn't read as natural language (as opposed to syntices that use a spelled out month name)
I18n limitation: Different separation marks are used internationally
I18n limitation: Different day vs month order is used internationally. User could easily overlook this in the instruction
Limited form validation possibilities
Advantages:

Few clicks or tabs
Semi natural input
Fast input for data entry
Conclusion

### The single field method is a useful form when it's known that:

All users will be from the same geographical region
Server is capable of intelligent post processing
Emphasis is on speed and ease of input, rather than on unambiguousness
The separate fields pattern

The separate fields method is probably one of the most common of date input methods that are out there. It gained popularity because maintainers of backend systems like the way the different values can go straight into the database as numbers their respective fields.

Day
Month
Year
Validation is also much easier using this method than with the singe field method, because the limit on the amount of characters can easily be set in the HTML code and the minimum of characters and their value could easily be checked by either a JavaScript, or by the backend. E.G.: A number as high as 30, could never be a month and a three digit value could never be a year, nor day. International users would also not easily mix up day and month, as it is easy to label all the input fields individually. (If not necessary for accessibility reasons)

#### Disadvantages:

User has to tab or click more, unless smart automated tabbing scripts are applied
User could still enter the name of a month, rather than a number or the other way around, so validation is necessary for that, which is annoying for the user in the case of a mistake
Advantages:

Less mistakes possible than with the single input method
Less ambiguous
Conclusion

The separate fields method is particularly useful if the backend cannot do any intelligent post processing and/or when accuracy of input is of the highest importance.

### The all drop down pattern

Another input method that I've seen users yell at during numerous user tests is the all drop down method. A dropdown is used for the day, the month as well as for the year. Selecting a day from a list of up to 31 items is simply tedious. Scrolling through the list is often required and year drop downs may be even longer.