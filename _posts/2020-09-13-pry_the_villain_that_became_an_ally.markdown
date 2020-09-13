---
layout: post
title:      "Pry: the villain that became an ally"
date:       2020-09-13 17:58:02 +0000
permalink:  pry_the_villain_that_became_an_ally
---




At the beginning of this course, my cohort lead raved on and on about this gem called Pry. At first, I wrote it off as a professional having an extensive technical understanding of Ruby promoting something that we’d eventually use later down the line. However, after working through my first CLI project I found that pry wasn't an application to be avoided, but a tool that can help in times of need.

My CLI (Command Line Interface) project was built around the topic of plants. The information I used was acquired by using trefle.io API.  While going through the data provided through the use of the API, I found myself using pry more often than I had at the beginning of the course curriculum.

Pry is a gem that needs to be required within your documentation (normally at the very beginning alongside a gem install in your terminal) in order to be used properly. Simply put, pry pauses your program wherever you have it placed and allows you to check the return value you may receive at the end of the method that you have it placed it in. Pry’s function can also be thought of in the way the “pause” button works within a video game, but instead of a video game, it’s a method. With such large amounts of data, you want to be certain about what you're receiving at the end of a method.  Using a properly placed 'binding.pry' within my enumerating method, I was able to see all of the values each plant listing provided, and select said value to show the user in my CLI as well. All in all, Pry became an ally during this project and I suspect that as I continue to use ruby, Pry and I will build a stronger connection as time goes on.

