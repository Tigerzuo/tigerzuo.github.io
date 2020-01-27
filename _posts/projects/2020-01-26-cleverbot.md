---
title: Self talking clever bot
subheading: Using clever bot api
categories: [projects]
---

A few months ago I saw this video of two Google home's talk to each other on youtube. The two bots were named Vladimir and Estragon and their conversation ranged from convincing each other that they are a robot to monty python references. The conversation was super entertaining, although it didn't always make sense. So I wanted to build something similar in my free time. 

[![Chatbot](http://img.youtube.com/vi/mpw_FB2QrjQ/0.jpg)](http://www.youtube.com/watch?v=mpw_FB2QrjQ "Chatbot")

The first thing I did was to search for the project online. Long story short, the project is private and the best guess of its implementation is by using Cleverbot API. 

The Cleverbot API can be called through the broswer and it returns a JSON object. However the API now cost about $10 for every 10000 calls which is a bummer to me. After a long while of searching for a free alternative API I struck gold. Turns out someone made a project to fake calling Cleverbot 'API' though the demo website. So the clever bot home site has a text box to demo the clever bot. Users can enter words and clever bot will text back its reply. This isn't a API so developers can't use it, but the project involed using a headless firefox to enter and parse texts on the demo website, thereby creating an API for developers to use. This is brilliant and now we can get to work.

The exact details can be found on my github but basically we spin up two instances of the Cleverbot API, we connect the output of bot 1 to the input of bot 2 and vice versa so its like two humans talking with each other. An initilization text is all thats needed to start the conversation. 

![chatbot]({{site.baseurl}}/images/chatbot/chatbot.png)
