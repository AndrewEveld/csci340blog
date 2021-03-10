---
layout: post
title:  "Unfortunate Hardcoding"
date:   2021-02-08 22:10:38 -0500
categories: disco tray studios update
---
This week at Disco Tray Studios, we have decided on a method to check if a user is an admin on the Hendrix Assessment website. Unfortunately, we decided to hardcode the admin usernames into the code to check if the user is an admin. This is not the most ideal or scalable method because only people who are familiar with the code will be able to add or remove admins. Another way we could possibly get this to work would to be to add a new table into the database that contains references to all of the admins. We are hesitant to modify the database because each time it is modified, the data that we are using is deleted.

Other members of Disco Tray Studios are making great progress on our other projects such as the "Good Vibes" app and the improvements to the City of Hope Outreach time-tracking website.

In terms of the Hendrix Assessment project, there are a few bugs I have caught relating to the way that the assessments are reloaded onto the screen. The Assessment Options for some of the Outcomes seem to be in the wrong order. My hunch is that it is simply a matter of ordering the data after it is pulled from the database.
