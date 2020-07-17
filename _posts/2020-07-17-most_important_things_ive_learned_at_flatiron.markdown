---
layout: post
title:      "Most Important Things I've Learned at Flatiron"
date:       2020-07-17 20:32:51 +0000
permalink:  most_important_things_ive_learned_at_flatiron
---

One of the graduation requirements for the Flatiron Online Software Engineering program is to write 7 blog posts and one more blog post is all that stands between me and being officially graduated. So, I've decided to use this opportunity to offer my completely unsolicited advice to anyone getting started in their software engineering journey. This post is specifically for the Flatiron bootcamp, but I think it will apply to almost any bootcamp or self learning as well. 

### 1. Learn to get yourself unstuck
Learning to get yourself unstuck is probably the most important piece of advice I can give to anyone just starting out. Whether it is learning to read the errors Learn Test gives you or an error in the terminal, the ability to understand what the problem is such a huge part of being a good developer. The best part? 90% of the time it will tell you exactly what went wrong, down to the line number --“Unexpected “,” on line 9, expected “;”. Yes, it sounds trivial, but learning to read and recognize errors speeds up the process tenfold.  

### 2. Get good at debugging
This is still in the same vein as getting yourself unstuck, but you should regularly be using pry, byebug, debugger and the console when writing code. If you can’t figure out why a function isn’t returning what you expect, drop a pry in the code and figure out what exactly is going on. You might not be passing in what you think you are as arguments into the function. Using the console is also a great way to quickly test things before moving on. Say you set up your database and model relationships to have a User who has many blog Posts. Save yourself a headache later on and take two minutes to use your console to make sure you can call @user.posts on an instance of a User.  I’ll admit that I probably wasn’t using pry enough leading into the Sinatra project, but I felt like my ability was on another level once I started utilizing those tools.

### 3. Keep your momentum going, but don’t get burned out
Let’s be honest, getting those Learn tests to light up green is addictive, and, if you’re like me, hours can fly by in the blink of an eye when you’re in your groove. But, this also a good way to burn out, even when you’re doing something you love. I highly recommend using a Pomodoro or some other style interval timer when coding. The Pomodoro technique is straightforward. Code for 25 minutes, then take a 5-minute break. Repeat this 4 times, but on the fourth break, take a longer 15 minute break. Then start all over. You can find timers like this online and in the app store, but it’s also easy enough to keep track of on a normal clock. These short bursts of work help keep you productive and focused, without the burnout. 

### 4. Relish in the projects
Projects are the biggest learning opportunity in the Flatiron curriculum. It’s one thing to solve a lab when you have strict guidelines, tests to let you know if you’re right, and have just went through a walkthrough in the lesson beforehand. Projects are a different beast. The training wheels are off and you’re not only responsible for if something is right, but what is right in the first place. For me, it’s when all those things I learned in the lessons prior start really coming together. I start making those connections in my brain and understanding things as a whole. 

Projects are also the time to learn even more things. After the CLI project, I tried to add at least one thing that is not gone over in the lessons. For the Sinatra project, I knew Bootstrap was a popular CSS framework, so I learned/used it for that and all subsequent projects. Then, in Rails, I integrated Active Storage so my site was capable of saving rich text with pictures. In the Javascript project, I had to teach myself Json Web Tokens (JWTs) so that I could have user authentication in a single page application. I would later incorporate JWT into my React/Redux project, and also dived into ActionCable so that I could set up a real time chat application. 

No, this isn’t required to graduate Flatiron, but don’t lose sight of why you’re at Flatiron to begin with. Eventually, these projects will help form your software engineering portfolio. If you’re sitting across a table from an interviewer who tells you that their company uses ActionCable, you’ll be able to point to that project and show that you’ve already been acquainted with it. The chances of that happening increase with every new thing you add to your skillset.

### 5. Get your MVP out
Here’s some advice that I, at times, have had trouble following myself. I’ve spent hours trying to get the perfect margins on a CSS element, trying to future proof my code for features I wanted to add later, and generally solving problems that I didn’t have –all while the basic functionality of my site wasn’t working. Trying to make a killer project is great, but you’re first priority should be getting a minimum viable product out. You can’t expect to code something that has as many features as a nearly two-decade old Facebook website in a week’s time, especially as someone new to software engineering. But what you can do is get a site with users and a newsfeed working, and then start building the like feature, image sharing, and fan pages as times goes on. This doesn’t and shouldn’t end with your project review either. Keep fleshing out your projects afterwards to make your portfolio even stronger.

### 6. Help other students
Why? Well, for one, it’s the nice thing to do. Someone has undoubtedly helped you in this journey and you can return the favor by helping someone with something you pick up on quicker than they do. But there is also a selfish reason to help other people. Being able to code something in a practical sense is very different than being able to explain it to someone else. It takes a much deeper level of understanding to effectively explain a concept. So, hop on AAQ when there’s no Technical Coaches around or on the Slack channel and try to help out. Not only will your understanding grow, but you’ll also get better at being able to talk about code, which is a vital skill to have. 


