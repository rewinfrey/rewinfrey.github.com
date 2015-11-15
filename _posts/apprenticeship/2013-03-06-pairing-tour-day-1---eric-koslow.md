---
layout: writing
group: Apprenticeship
title: "Pairing Tour Day 1 - Eric Koslow"
description: ""
categories:
- apprenticeship
---

During the last four weeks of an apprenticeship at 8th Light, resident apprentices do a two week pairing tour, and two weeks working on super secret challenges. I started my pairing tour today with Eric Koslow, who is part of a team working on a large [JavaScript MVC](http://javascriptmvc.com/) application. I took a few things from today that I feel like will be good lessons to remember in the future. I'd also like to not make this post a rant, but I warn you dear reader in advance if I do digress into a rant about the pains of large-scale JavaScript applications.

But first, if you haven't read [Uncle Bob's latest blog post](http://blog.8thlight.com/uncle-bob/2013/03/05/TheStartUpTrap.html) on the [8th Light blog](http://blog.8thlight.com) - you're missing out. I had a brief but turid affair with a startup back in Wichita. While my experience was not to the same degree Uncle Bob describes in his post, there were things I experienced there that make working in the culture of 8th Light a very refreshing oasis of code quality and best practices. I learned a ton working at that startup, but I also learned that phrenetic pace and marching through massive code changes without tests is akin to insanity. We all learn somehow, though.

Back to the pair tour. I didn't know what to expect when going into today because I don't have alot of experience working with JavaScript heavy applications. I read up on [Jasmine](http://pivotal.github.com/jasmine/) - a popular JavaScript testing framework - and went in with no expectations and an eager mind wanting to learn. Working with Eric was a great experience - I learned how to get better feedback and how to debug JavaScript code. Another big take away was how to search through large code bases whose structure and model relationships are opaque using [Ctrl p](https://github.com/kien/ctrlp.vim). We also did some interesting things with Git that helped solidify rebasing and squashing commits and managing branches efficiently. It was also a good feeling to help contribute to finishing a story with Eric that helped polish parts of the user experience that held an important place in the functionality of the application. It taught me some interesting things about the quirks of the iPad's Mobile Safari browser and how to listen to touch events. Most of all, I really appreciated Eric's patience in explaining the application and strategies for exploring the application. The exposure to Jasmine was also nice to experience, and would like to explore it on my own time after the apprenticeship.

It was also a valuable learning experience participating in the standup meeting with the client today. It helped reiterated a few things I've learned about effective communication with the client. I'd summarize these as:

* Communicate problems and delays as soon as possible.
* Communicate problems and delays as soon as possible.
* Clarify expectations and requirements for stories so unspoken expectations don't sour a client/consultant relationship.
* Communicate problems and delays as soon as possible.

This is something that's been reiterated numerous times throughout my apprenticeship both by my mentor, Micah, and the reading we are required to do. At times as an apprentice it is hard to role-play that client/consultant relationship in a realistic way, but in seeing the client/consultant interaction today all of those lessons came back in sharp focus. One of the 8th Light craftsmen on Eric's team handled a potentially sticky situation with the client very well by maintaining clear communication that reflected the principles of 8th Light. It was great to see this in action, and it brought home all the things I've learned about communication over the past three months.

It also made me appreciate on a deeper level that the relationship between client/consultant is the corner stone of a company like 8th Light. Without trusting relationships and demonstration of the agile process by consistently adding value for the client in the stories for each iteration, a business like 8th Light would not flourish. However, it reaffirms even more that the values and principles of 8th Light are specifically designed to promote the best possible client/consultant relationships, and that is a wonderful thing to be part of in any way possible.

My roommate and I both have serious gripes about JavaScript, which have less to do with the actual language, and more to do with how the language is commonly used. JavaScript uses [prototypal inheritance](http://blog.vjeux.com/2011/javascript/how-prototypal-inheritance-really-works.html) which is an interesting way to structure the object model of a language. Because of this JavaScript provides a tremendous amount of flexibility in how the language is used - including storing annonymous functions as attributes on an object. It's not JavaScript's fault that many developers writing JavaScript don't structure the code well, but it does make working in a large scale JavaScript application at times a confusing mess of loose structure, objects knowing a lot about other objects, and the global namespace being heavily polluted with state about the application when the application first loads.

It's impossible to think of JavaScript without also considering jQuery. For what it is and does, jQuery is a great library. It provides a useful API that simplifies the code required to do a number of everyday JavaScript functions related to traversing the dom, finding specific elements and controlling relatively simple behavior of those elements. But things can get weird quickly in JavaScript due in part to its asychronous nature, the fact that everything is loaded and anything can talk to anything, and traditional object oriented programming structure tends to break down quickly.

With all that said, JavaScript does allow for amazing results. One of the highlights of the day came from looking at [D3](http://d3js.org/) with Eric at the end of the day. Eric is in the process of creating a stock-simulator for a contest he wants to have with other craftsmen. The stock-simulator runs on a server with a public API that allows a third party to buy and sell stocks. Eric wants to provide feedback about the status of the stocks using D3 to visualize the data. I'm really excited to see it in action.