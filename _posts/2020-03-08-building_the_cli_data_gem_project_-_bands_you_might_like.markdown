---
layout: post
title:      "Building the CLI Data Gem Project - Bands You Might Like"
date:       2020-03-09 00:30:27 +0000
permalink:  building_the_cli_data_gem_project_-_bands_you_might_like
---


For my CLI Data project, the first project of the Software Engineering program at Flatiron, I wanted to build an application that I myself would find useful. So, I started thinking of things that I enjoy doing and listening to music is somewhere near the top of that list. However, I often find myself listening to the same music that I was listening to ten years ago and rarely ever seek out new music to listen to. Thus, I decided my application would be a tool to discover new bands based on bands that I already liked. The application, which I named Bands You Might Like, would follow this basic framework:

* A user types in a band or artist that he/she likes
* The application scrapes a website that lists similar bands
* A list of similar bands would be displayed
* The user could select a band from the list to find out more about that band

Now that I had an idea of what I wanted to do, I had to face what was easily one of the most daunting aspects to this project-- the blank slate that was given. For all the labs and lessons leading up to this project, there was always at least a basic application structure given and tests to make sure the code was right. Now, there was none of that and not only did I have to figure out how to code the project, but how to set the project up to begin with. While setting up a Gem wasn’t something that was covered in the lessons before the project, a couple of videos were provided on how to get started on the project page, which I used to get my basic project structure up and on GitHub. (Note: this was probably a bad time to switch from the browser IDE, but I switched to the desktop IDE and VSCode at this point so I could adjust my terminal size.) 

Once I was set up, I found banging out a rough working code to be surprising easy and felt a little relief that I maybe did know what I was doing after all. Luckily, the website Last.fm has tons of information on bands/artists and made scraping the information I needed my project a simple process. I could go to a bands page, scrape a list of similar artists, and then go to those artist’s page to scrape more information. I also took the time to build a more detailed flow chart for my application:

* Puts Greeting 
* Asks user for a band
* Convert input to a URL
* Get a list of similar bands and other band URLS from first URL
* Store the bands and band URLs as instances of a class
* Scrape more information about bands from each of their URLs 
* Display list of bands with some info (name, genres, popularity)
* Ask user which band they would like to learn more about
* Display more detailed information (name, genres, popularity, bio, top songs, links to music) based on input
* Get user input to go back, start again, or exit
* Puts Goodbye message

At this point, I was patting myself on the back for having this whole Ruby thing figured out. Unfortunately, just as how surprisingly easy I found it to get the rough code working, I was even more surprised by how time-consuming and frustrating it would be to iron out all the small details of the project. I faced a laundry list of tasks that needed to be completed, such as: Figuring out how to rescue the application if the website I was scraping didn’t have any information on a band, needing to give the user the option to exit or go back, controlling the interaction loop, emptying the array that held all instances of the bands, and setting up ‘graceful fails.’

More often that not, solving one headache would lead to another (like when I implemented a way to start a new search, but getting the issue of having two ‘Goodbye’ methods executing). After some time and thought, however, I am left with an application that I am both happy with and proud of. The project was a huge learning experience and how much I’ve learned in the past four weeks is astonishing. 

