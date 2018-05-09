---
layout: post
title: Card Scanner Project v1.0.0
description: Powered by Raspberry Pi
image: assets/images/2018-05-09.jpg
date: 2018-05-09 13:33:25
lang: en
---

It's very surprising to see how more than a week has passed since my last blog post! Sorry to keep you guys waiting, but I was working on a new personal project... the card scanner!

As some of you may know, I am an active member of IEEE's student branch at my university. I will be the Vice President of Communications next semester, overlooking publicity and recruitment of new members for our organization. One of the most human labor-intensive tasks is keeping track of who attended our events, which is a crucial task since event attendance is the primary method for students to earn active status within the club. In the past, we've manually entered students' names for every single event or had students fill out online forms, but both of these proved insufficient because it was either time consuming, too much work, discouraged students from marking themselves present, or a combination of these. Whatever the case may be, we wanted a new and innovative way to sign in members with ease, and this was my solution:

![Card Scanner](/assets/images/2018-05-09.jpg){:class="image main"}

Yup, a card scanner connected to a [Raspberry Pi](https://www.raspberrypi.org/products/raspberry-pi-3-model-b/){:target="_blank"}. Why is it connected to a Raspberry Pi? Because it looks cool. There's not a functional reason, but I just wanted to get one and play around with it, so I decided to incorporate it in this project. By the way, I was astonished by the capabilities of this little computer! I loaded [Raspbian](https://www.raspberrypi.org/downloads/raspbian/){:target="_blank"} on my Pi, but the flexibility of this machine is amazing. It's literally a tiny Linux computer, and it performs quite well!

I'll give you guys a brief overview of how this works. First, I created a Google Sheets page which basically acts as my database. I initially thought of making an SQLite database, but I wanted to share the information on the database with other officers (and only these officers) who would need frequent access, so I thought a local database wouldn't be a good design choice. Our organization board uses Google Drive for EVERYTHING, so I thought it is best to keep all the info there anyways. Then, I created a command line Python program that loads the database via its [API](https://developers.google.com/sheets/api/){:target="_blank"}. As students swipe their student MCards, it keeps track of their attendence individually, adding new students to the database as necessary. At the end, the program will send the list of students who swiped their card via email, and the program terminates. Pretty neat, huh?

Hopefully, this new method would somewhat alleviate the manual labor our organization had to deal with in past semesters. I'm looking forward to creating new projects using Raspberry Pi!

You can access the project source code [here](https://github.com/shutas/IEEEUMich-Card-Reader){:target="_blank"}.