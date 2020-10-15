---
layout: post
title:  "Giving Functionality to Hendrix Assessment"
date:   2020-10-07 22:10:38 -0500
categories: disco tray studios personal update
---

This week I worked on getting some working examples of ways we can update pages in ASP.NET. Innocent is working on getting the database functionality working in our ASP project, and he was wondering how we planned to get information updated on each page that the user was using. I was able to get a few different strategies to work.

The first strategy that I had success with was by using C# "if" statements embedded in the html. I was able to store booleans in the C# model of the cshtml page, and the embedded "ifs" were able to utilize the boolean to only generate code given certain circumstances. The downside to this strategy was that the page had to be refreshed if a boolean variable was changed. Refreshing the page is fast, but not as fast as directly modifying elements with jQuery.

This brings me to the second strategy I used to update pages. The second strategy is by using jQuery to update the elements on the page. The benefit of this strategy is that it is very fast and the page doesn't have to be reloaded. The downside is that I would either have to write all of the logic for our project in javascript or embed C# functions within the javascript that all ran as soon as the page was rendered. Honestly, I prefer to never have to work with javascript because it is difficult to bug, and I always run into problems with the javascript behaving unexpectedly. I find it much easier to code in C#.

Therefore, my preference over these two methods would to be embed C# logic within html elements. Razor Pages makes this functionality very straightforward, and I would be able to keep the bulk of the logic in the C# file.
