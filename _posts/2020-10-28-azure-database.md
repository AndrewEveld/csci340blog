---
layout: post
title:  "Azure Database"
date:   2020-10-28 22:10:38 -0500
categories: disco tray studios personal update
---

This week at Disco Tray Studios we worked on both the Hendrix Assessment project and our Twitch. Lucy has been working on getting our Twitch account put together. I have yet to contribute to the Twitch scene, but soon we will all be creating educational videos about video games.

In regard to the Hendrix Assessment project, we have all been putting in a lot of work to get it running. This week we focused on connecting the .NET Core project to a remote Azure Database. We were also able to get the Microsoft identity login verification to work. We demoed the project to the clients and they were very happy with everything we have been able to accomplish.

I was mainly focused on getting the project to work with the new database. I had to change the names of some of our models to correspond to the names in the database. I was also able to get the submitting of assessments to work as long as the class had only one topic and wasn't TEC.

Ivy is the only one with the direct ability to view the data of the Azure Database. For this reason I have implemented a page that renders all of the data from the database onto the page.

I am beginning to become much more familiar with the Razor framework. I am learning a lot about interacting with the database and querying with EF Core.
