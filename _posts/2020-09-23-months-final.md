---
layout: post
title:  "Wrapping up MLIM"
date:   2020-09-23 22:10:38 -0500
categories: disco tray studios personal update
---
This week is the last week that we plan to be putting in a lot of work into [My Life in Months][my-life-in-months]. The only feature we have yet to release is the month picker feature. This feature allows users to select the starting and ending months of each of their life events. This setup allows users to create the charts much quicker using the number of months. Users no longer have to calculate the amount of months each of their events happened. This also reduces user error, which allows each user to create more accurate charts.

We decided to allow the users to choose whether they wish to use the month picker feature or continue using the number of months. I spent the bulk of this week and last weekend figuring out how we could seamlessly toggle between each option. Figuring this feature out was mostly straightforward, and I learned a lot about javascript's Date object. For some reason the Date objects would sometimes not behave like dates. It's almost like javascript forgot what kind of object they were. After much frustration with the misbehaving Date objects, I decided to implement all of the date calculations myself. This saved me a lot of headache and frustration. Implementing these functions turned out being much more simple than I expected since I didn't have to worry about the days and leap years and February and such. Working only with months and years makes months much much easier.

The main thing that I learned this week was that I need to be more open about implementing objects or methods that already exist. Just because a data structure is already implemented, it doesn't mean that it is implemented in exactly the way that I want. I could have saved a lot of confusion in the My Life in Months source code if I had decided not to the Date object at the very beginning, and, instead, had used some methods to manipulate a date string. 



[my-life-in-months]: https://discotraystudios.github.io/my-life-in-months/
