---
layout: post
title:  "More Assessment Progress"
date:   2021-03-01 22:10:38 -0500
categories: disco tray studios update
---
It is time to celebrate! I have finally located the issue with the admin CSV page. I finally decided that in order to replicate the issue on my local machine, I would have to add a lot more data to the local SQLite database. Fortunately, after I added a lot more data, I was able to replicate the machine and use Visual Studios' debugging tools to pinpoint the issue.

I was right in my previous post that it was a problem with our query into the database. Instead of pulling out the Assessment Options only for the certain class we were looking for, the query pulled the Assessment Options for every class with the same outcome and topic id.

Something valuable I learned from this experience is that it is very useful to have a lot of different data added to the test database, so that you can see the highest number of possible outcomes.

The other members of Disco Tray Studios are making progress on the "Good Vibes" app and on the City of Hope website. Dr. Goadrich gave us a detailed rundown of the meeting this week with the faculty. Our mission is to help them think through some of their ideas, so that they can give the Game Development class more interesting and full ideas. We are all looking forward to meeting with them.
