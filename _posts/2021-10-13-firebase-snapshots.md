---
layout: post
title:  "Firebase Snapshots"
date:   2021-10-13 22:10:38 -0500
categories: disco tray studios update good vibes
---

This week I added notifications for receiving a good vibe to Good Vibes and added a badge that is displayed on the app icon that indicated the number of received and unread Good Vibes. To add both of these features, I modified the snapshot that queries the data from the Firestore database. 

Each time the user opens Good Vibes, we query Firestore for a list of their current Good Vibes. To query this data, we create the query, then open a subscription to the query. While this subscription is active, we get notified of all changes to the set of data that is included in the initial query that was written. The object that we receive is a snapshot, and this object contains all the documents including the ways in which each document has changed. A document can be marked as `modified`, `added`, or `removed`. In the first snapshot received, all documents are marked as `added`. 

The code that I put into the snapshot function ignores the added documents of the first snapshot, then, in future snapshots, any added documents trigger a notification on the device and increments the app icon badge. Whenever the user navigates to the Good Vibes page, the badge is removed. 

I ran into problems with my code because I had put the "document add" check within a loop that was already looping over all of the documents. This caused too many notifications to be sent, and incorrectly incremented the app icon badge. After I fixed this issue, the code worked as smoothly as I had hoped. 

I learned a lot about communication with our backend this week by adding these changes. Utilizing the subscriptions to our database simplifies a lot of things for us, and keeps us from making too many unnecessary calls. We don't want to access Firestore more than we need to because we are allocated a limited number of reads and writes as long as we are on the free Spark plan. 

This notification is the last notification addition we have on our plate for now. In the future (near or far) we plan to add push notifications, so a user can receive notifications whenever the app isn't running. This type of notification requires some kind of logic running in our Firebase backend that triggers a notification whenever the Firestore database is modified in some way. I believe this requires the use of Firebase Functions, which we don't currently have access to as free users of the Firebase tools. 

In our next meeting, I am looking forward to hearing some of the feedback from Dr. Goadrich's class of Beta testers. On Monday some Disco Tray members visited the class to hear the feedback, and I am looking forward to learning some of the ways we will be able to improve the app. 