---
layout: post
title:  "Good Vibes Development and Deployment"
date:   2021-09-29 22:10:38 -0500
categories: disco tray studios update good vibes
---

For the past few weeks, the majority of my time has been dedicated to the development and beta deployment of Disco Tray Studio's mobile application Good Vibes. The functionality that I was tasked with to add to the app is notifications. Users should receive a notification whenever they update their mood for the first time of the day, and users should receive a notification to remind them to update their mood during the day. On the deployment side of things, we wanted to set up beta testing distribution for both iOS and Android user because we plan on testing Good Vibes with some students at Hendrix. 

To add notifications to Good Vibes, I used a Flutter package called `flutter_local_notifications`. This package allowed me to setup notifications for both Android and iOS apps with fairly little app setup. During the process of setting up these notifications, I became more familiar with Flutter's provider and consumer objects that are the backbone of our backend and allow the app state to persist. For the notifications to remind the user to update their mood, I used a package called `shared_preferences` which enabled us to store the interval that the user chose to receive notifications. This package is popular for storing settings and other small pieces of data that need to be stored on the user's device. Initially I was trying to use a sqlite database with one table, but that was overkill for storing one key-value pair. 

Setting up beta deployment for iOS and Android on Firebase was a very interesting process. I have learned a lot about the details of building and uploading initial versions of mobile applications. We had to make account on the Google Play Store and App Store for Disco Tray Studios, so our apps could get verified. Each account has its own method of doing different kinds of testing, but, after each account was properly set up, we were able to deploy both apps for testing in Firebase distribution. Building the iOS app was much more complicated than building and deploying the Android app, but we expected this to be the case. The Bundle ID that we initially setup for our iOS app in Firebase did not work whenever I registered it, so I had to create a new iOS app in Firebase with a Bundle ID that I was able to register with Apple. 

Looking to the future, it might be worth it to try and setup CI/CD for Good Vibes, but that might be overkill for now. We should focus more of our energy on the development of the critical functionality of the app. It's a simple app, but there is much to do before it's ready to be uploaded to any app store. 
