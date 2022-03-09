---
layout: post
title:  "Good Vibes Open Testing"
date:   2021-11-03 22:10:38 -0500
categories: disco tray studios update good vibes
---

Good Vibes development has been fruitfully chugging along, and we have finally made it to the point where we are confident enough in the app to begin open testing. Open testing is where anybody in the US is able to test our app granted that they are provided with the link for it. We have open testing set up for both the Google Play Store and the Apple App Store. 

One of the major changes that I helped bring to Good Vibes recently was removing the local database that stored quotes on users' devices and adding the quotes to our current remote Firestore database. The reason for this change is because the database changes for the local database were very complicated and difficult to keep straight. Each time we made updates to the local database, we would have to write code that had the ability to merge a user's current local database with the changes that we made. This process became tedious and resulted in many unexpected errors and bugs. We now have the quotes setup in the Firestore database which makes the programming of the app and the updating of the quotes much simpler. 

I have made a number of smaller improvements to Good Vibes. One of these improvements is the addition of a button used to share quotes from Good Vibes externally. We already have the functionality to share Good Vibes within the app, but we wanted to give users the option to share their quotes via text, email, social media, etc... The addition of this button was simple thanks to an existing Flutter package. Another small visual improvement was the addition of a loading screen to the app on bootup. This screen simple with a blank black or white background and the Good Vibes and Disco Tray Studios logo in the center. The purpose of this screen is to allow the app to fetch a user's information from Firebase before displaying any of the screens on the main app. This keeps the user from seeing any of the screens before they are ready to display information. 

I am looking forward to the feedback that we receive during open testing, and I hope that plenty of people have the change to try out Good Vibes for us. I'm excited to publish the app to the App Store and Google Play Store. 


