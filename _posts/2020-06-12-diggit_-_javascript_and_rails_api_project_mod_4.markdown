---
layout: post
title:      "Diggit - Javascript and Rails API Project (Mod 4)"
date:       2020-06-12 04:16:58 +0000
permalink:  diggit_-_javascript_and_rails_api_project_mod_4
---


For this project I built a Reddit-lite (or 'Digg', if you remember that site) style single page application. Users can submit links to different categories on the site, and then those links can be upvoted by the community. 

At this point in the program, I'm very comfortable using Ruby and Ruby on Rails, so setting up the Rails API was a breeze. I generated the different models and controllers, leaving most of the controllers blank until I needed to use them later. 

However, as soon as I got to the front end of the project, I quickly ran into a bit of a problem. Having users and limiting upvotes to one per submission per user would mean I needed a way to sign up and log users in. We've done that in Rails, but it wasn't something gone over (yet) for JS and a single page application. Thus, after some Googling and some pointers from my cohort lead, I had a long weekend of learning about JSON Web Tokens. With the JWT gem, I was able to generate the tokens and pass them back in the JSON renders of my User and Auth controllers. From there, I stored the tokens in localStorage on the client side, and passed them back in a Authorization header when needed in my fetch requests. The JWT gem was then able to decode those tokens once passed back to make sure a user was authorized to perform certain actions. While that sounds easy enough in theory, it did take me a good amount of time to wrap my head around the process and figuring out how it worked. 

The rest of the front end work didn't really have any major obstacles. Instead though, there was a constant stream of minor things that proved to be frustrating. Most of those though were just due to me being new to the language and not remembering proper syntax. I also found it much easier in JS, compared to Ruby, to end up with a messy pile of code. In the index.js file, for instance, I found myself having a long file of functions that were in no particular order. I eliminated most of the mess by making creating classes for my API and Users, leaving my index.js with my const declarations and event listeners. 
