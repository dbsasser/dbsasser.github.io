---
layout: post
title:      "Channels - My Flatiron Capstone Project"
date:       2020-07-10 21:48:25 +0000
permalink:  channels_-_my_flatiron_capstone_project
---


After exactly five months into my journey at Flatiron, I have submitted my final project for review. Not too long ago, I had no idea what an array or hash was. Now, I'm building fully functional web applications, from the backend to the frontend. I am both proud and amazed at times on how much my knowledge has grown during this period.

For my final project, I created a lite version of Slack. The website is built with React and Redux on the frontend, and Rails API on the backend. Members of the website can sign up and join different channels/chat rooms that allow them to message with other members. Members also have the option to leave a channel if they wish.

Going into the project, I was more confident than usual. I felt like I had a solid grasp on how React and Redux works thanks to my cohort lectures and the video series on Learn Instruct. Of course, there were a few challenges during the actual coding. A large majority of them were purely simple mistakes, like not initiating parts of the state in my reducers. The rest we're overlooking on how components are rendered/re-rendered, and in what order. However, my skills at knowing when and where to put a debugger or pry have greatly improved, and I was able to sort out most things quickly.

That being said, I've come to realize that, just like in all my other projects, there is usually one major hurdle. Without a doubt, ActionCable was the biggest headache of this project. While I could have set an interval to keep checking for new messages ( 'polling' ), I felt that would be a lazy and inefficient approach. Plus, I also wanted to gain experience with ActionCable. 

ActionCable, is actually not that hard once you get an idea of how it works. You create a stream for (in this case) a model, broadcast to that particular stream when there is an update, and then connect to that stream on the frontend to receive the updates. Why did I spend a good ~15 hours on getting it to work then? Because during that time, I thought I knew how ActionCable worked and didn't understand how it actually worked. Once I understood what the 'broadcast_to' portion expected for arguments and how they should be formatted, it turned out to be easy.  So, lesson learned. If you can't get something to work, go back through the documentation and make sure you know the basics of what is going on. 
