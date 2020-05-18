---
layout: post
title:      "Building My Rails Project - LaunchPad Crowdfunding"
date:       2020-05-14 22:40:15 -0400
permalink:  building_my_rails_project_-_launchpad_crowdfunding
---

For my Rails project I built an app called LaunchPad. LaunchPad is my take on a KickStarter / IndieGoGo crowdfunding site. Users are are to create 'campaigns' that other users can donate to and comment on. Campaigns can be sorted by their newness, those with the most funding, and those that have hit their funding goal.

While the solution ended up being rather simple, by biggest hurdle was getting the associations correct. Afterall, the project hinged on having correct associations, so I wanted to make sure those were right from the start. Specifically though, a 'campaign belonging to a user' and 'having many users, through donations' made things complicated. When set up just as written above, the associations appeared to have somewhat worked at first glance. However, it became clear that something was off while I played around in the console.

With that setup, ActiveRecord had trouble indentifying what a user was in relation to the campaign. I could run '@campaign.user' and '@campaign.users' just fine, but was unable to use '@someuser.campaign.build'. It wanted to assign the user to the "has_many" part of the relationship, and not the "belongs_to" relationship, no matter how many different ways I tried.

My solution was to use an alias for the User that creates the campaign. I did this in the association part of the models, and this is what it looks like in code: 

```
class User
     has_many :created_campaigns, class_name: "Campaign", foreign_key: "creator_id"
end

class Campaign 
     belongs_to :creator, class_name: 'User', foreign_key: "creator_id"
end

```

User_id in the Campaign table of the database was also replaced with 'creator_id', which is what the above code references to in the foreign key attribute. 

Not only did this solve my association issue, but it also had the added benefit of making my code more readable. Calling on '@campaign.user' is a little ambiguous. Someone reading my code would not be sure if I was calling on a user who donated to the campaign or the one who created the campaign. Being able to use '@campaign.creator' and '@user.created_campaigns' is a much clearer and better approach. 

While, again, this seemed to be an easy fix, it did take quite a bit of effort me to get right. This was a little deeper than what the module's lessons went over and made me explore some new areas of how models can be associated. 



