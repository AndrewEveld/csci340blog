---
layout: post
title:  "Streaks and Thanks"
date:   2021-11-03 22:10:38 -0500
categories: disco tray studios update good vibes
---
These past few weeks, we have made many improvements to Good Vibes. We have been working on methods to increase the circulation of Good Vibes in the app. Currently, users only generate one Good Vibe a day as soon as they log their mood. Many users are not sharing their Good Vibes like we expected, so very few users receive Good Vibes from other users. We need an improved method of increasing the volume of Good Vibes out in the world. 

One idea we have began to implement is for users to be able to generate multiple Good Vibes a day based on a few different factors. We decided that users should receive more Good Vibes the longer their daily streak for using the app is, and they should receive more Good Vibes for receiving more "Thanks" from other users. We added a new field to users' documents in Firebase that keeps track of their mood logging streak, the number of consecutive days they have logged their mood. We also created a new field called "Thanks", which keeps track of the number of Good Vibes sent by the user and then shared again by another user. Basically, if user A sends a Good Vibe to user B, then user B sends that same Good Vibe to user C, then user A will receive one "Thanks" from user B. 

Taking these two new numbers into consideration, we now have to come up with a way to use them to calculate the number of Good Vibes a user should be able collect a day from logging their mood. We currently have the new system set up so that there are specific milestones for a user to reach with their Streaks and Thanks Received. At each milestone we increment the number of Good Vibes a user can receive daily. 

These improvements to the Good Vibe system will hopefully increase the Good Vibe flow in our Firestore database. Andrei is currently working on a new system for favoriting and sharing Good Vibes that will allow users to share and keep Good Vibes simultaneously. We learned from feedback from Dr. Goadrich's TEC class that users are reluctant to share Good Vibes that they like or find helpful, which is the opposite of what we wanted or expected. We want to encourage users to share Good Vibes that they like, which we plan to do by allowing them to keep Good Vibes they have shared. This new system of sharing will need to be merged with the new system of generating Good Vibes. I believe that we plan to only have "Thanks" sent whenever a user favorites and shares a Good Vibe.

The number of moving pieces in this app are ever increasing and I have been enjoying watching new improvements be made each week. Soon we will have a new version of Good Vibes to send out to Dr. Goadrich's class and maybe even a larger pool of testers. 
