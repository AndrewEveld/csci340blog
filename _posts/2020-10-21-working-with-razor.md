---
layout: post
title:  "Working With Razor"
date:   2020-10-21 22:10:38 -0500
categories: disco tray studios personal update
---

Razor pages are a powerful way to create web apps with ASP.NET. They allow you to contain the view of a page within one file, and the backend of the page within another C# file that is connected to the view. This week I was able to become more familiar with the methods of passing information between the
user interface and the backend.

Razor pages have a really cool way of passing data to the backend after a user posts data. Essentially what happens is that you designate a certain field contained within one of your models to input fields in the form in the html. Once you designate those model fields to the html fields, the program generates a model that contains the information passed when the data is posted.

This whole process took me a while to fully understand because I didn't know that the program instantiated the model on its own. With this process I could directly assign values to the AssessmentOptions with the data filled out in the survey instead of passing the numbers to the backend and creating the AssessmentOptions myself. 
