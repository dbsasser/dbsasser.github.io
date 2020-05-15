---
layout: post
title:      "Building My Rails Project - LaunchPad Crowdfunding"
date:       2020-05-15 02:40:14 +0000
permalink:  building_my_rails_project_-_launchpad_crowdfunding
---

For my Rails project I built an app called LaunchPad. LaunchPad is my take on a KickStarter / IndieGoGo crowdfunding site. Users are are to create 'campaigns' that other users can donate to and comment on. Campaigns can be sorted by their newness, those with the most funding, and those with the most comments.

While the solution ended up being rather simple, by biggest hurdle was getting the associations correct. Specifically, a campaign belonging to a user and having many users through donations made things complicated. When set up as just
