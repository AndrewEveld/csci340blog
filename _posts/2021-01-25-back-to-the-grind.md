---
layout: post
title:  "Back to the Disco Grind"
date:   2021-02-01 22:10:38 -0500
categories: disco tray studios
---
We're finally back on campus at Hendrix for the 2020-21 Spring semester. I'm glad to finally be back and to be among my friends that I haven't seen in almost a year.

Here at Disco Tray Studios, we've hit the ground running this semester. We have multiple exciting projects in progress including the Hendrix Assessment website, and new idea for a "feel good" app, upcoming work with professors to develop educational video games, and some finishing touches on the City of Hope Outreach time-tracking website. It is exciting to see so many ideas come together to create this wide array of community oriented software.

My job right now is to give the Hendrix Assessment website some some restricted access pages that only admins can see. We already have the majority of the admin pages developed, but we have no reliable way to distinguish from admins and non-admins.

An idea that I looked at and tried to implement was to look to see if the user was a part of the Hendrix Assessment Team on Microsoft Teams. If they were a part of that team, then that means they are an admin. However, we were unable to get this to work because we believe we don't have the proper authority to access this kind of information.

I think that for now we will have to hardcode a line into the code that checks whether the email of the user is the same as a certain admin email. Hopefully we can find a way to solve this problem in the future.
