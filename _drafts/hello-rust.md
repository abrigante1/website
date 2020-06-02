---
title: Hello, Rust
show_edit_on_github: false
show_subscribe: false
license: false
permalink: /drafts/hello-rust.html
---
For about a year, I've been watching Rust from the sidelines with extreme curiousity - eager to find the time to get my hands dirty and learn the language. Now that -- thanks to a global pandemic -- I'm armed with way more free time then I know what to do with, I'll be making a devlog on my experience learning and making a game in Rust.

<!--more-->

To provide some context on my own background, I'm entering my fifth year at DigiPen Institute of Technology where I'm majoring in Computer Science with a focus on digital signal processing and audio programming. During the course of my college career at DigiPen, I've had the opportunity to work on all sorts of projects, ranging from creating a completely custom game engine to a granular synthesizer. I primarily work in C++ but have some experience with C and C#, and have been wanting to add Rust to the list of languages I know.  

With that in mind - I decided I was going to dive in head first and learn Rust by creating *Boundless*, a 2D Survival Sandbox Game heavily inspiried by one of my all time favorites - Terraria, and thus this devlog was born! I plan on trying to write posts at least every other week, documenting the systems I implemented, what I'm enjoying and not enjoying about Rust, as well as just my over all experience with using the language for game development. Before we begin, I wanted to note that in an attempt to save your eyes from the horror that is my programmer art, my close friend and outstanding artist, Kyle Erickson, will be providing me with most of the assets that will be used for the game. If you want to see more of his awesome work, please give him a follow on Instagram at [@samurai.sunrise](https://www.instagram.com/sunrise.samurai/).

# Source Code and Git Workflow

All the code being used for the project can be found on Boundless's GitHub repository [here](https://github.com/abrigante1/boundless). Real quick, to explain the repository's layout - I like to organize my work into three core branches: 

 - Master
 - Production
 - Sandbox

Master is used for a "completed" version of the project. This will contain no work-in-progress features, and is intended to host the most recent version of the project that can be downloaded, compiled, and run with zero issues. Production, will be where I am actively working on polishing and re-architecting a features that have already been prototyped. This branch will include partially implemented features, but will be as close to complete as possible. Lastly, sandbox is where I will be doing all my testing work and experiementation. It's here where I will be trying out a potential implementation, and discovering what does and doesn't work. This branch will essentially always be unstable and it's explicit purpose is to act as a playground where I can try out new ideas, without risking the pollution of production. However, after this branch will usually be updated to include the most up-to-date version of production at a given moment. I heavily enjoy this workflow as it allows me to gain a better understanding of how a system needs to work with other systems *before* I try to architect the feature. As a result, I am able to see the bigger picture much more clearly. 

So with that our of the way...

# The Tech Stack

For this project, I was pretty conflicted with how much raw custom engine work I wanted to do. While I heavily enjoy core engine development, I really wanted to get right into making a game so I initially decided to create this project using the Amethyst game engine framework. [Amethyst](https://amethyst.rs/) is a huge Rust game engine framework that provides you with a lot of the tools needed to get starting making a game. It can take care of audio, graphics, entity management via an entity-component system, and many other things. 

However, if you have already taken a look Boundless's GitHub repository, you may have noticed that it says "...making a 2D Sandbox Game with the GGEZ framework" and *not* the Amethyst framework. Why's that? Well - while Amethyst does offer a lot of very powerful tools, it also isn't very well documented and felt extremely constraining. With every system I wanted to implement, it felt like I was fighting against Amethyst to get it to do what I wanted it to do, and I spent more time trying to figure out how Amyethest was support to work then I was spending time actually doing game development. As a result of this, I ended up framework-hopping a few times between Amethyst and the aforementioned GGEZ. 

[GGEZ](https://ggez.rs/) is another game engine framework, but has a completely different design philosophy. Rather then being an all-in-one toolbox providing everything you need to make a game, GGEZ gives you the basics and then lets you decide how to build on top of it. While this directly clashed with my initial desire to avoid doing too much core engine work, I eventually got tired of fighting Amethyst and decided that it was better to spend more time working on core engine features, then it was to dig through Amethyst's source code trying to figure out how it wanted me to do a thing. As a result, I feel that for this project GGEZ is the better route to go. 

I also really wanted to learn how a proper Entity-Component System (ECS), so on top of GGEZ, I also decided to use [specs](https://specs.amethyst.rs/) as the ECS for the game. For those that are unfamiliar with what an ECS is, specs has a great briefer that can be found [here](https://specs.amethyst.rs/docs/tutorials/01_intro.html). An additional secret hidden motive for using an ECS in this project, was also to get comfortable with what's currently the standard, so that I could hopefully one day try writing my own. So who knows -- maybe after this series I'll make one about writing a custom ECS :)

# Getting up to Speed

Since this initial post is already getting quite long, I'll briefly wrap up showing off what I currently have implemented in my sandbox, the source code of which can be seen [here](https://github.com/abrigante1/boundless/tree/v0.1), as well as some quick notes on where I'll be going next.

![Image](/assets/boundless/gifs/sandbox_v0.1_bp-1.gif)
Note: The background sprite for game in this gif is by MadFireOn and can be found [here](https://swapnilrane24.itch.io/nature-background?download) 


The above gif shows off the following features: 

- Rendering System
    - Sprite Sheets
      - Sprite Culling
     
- God Camera Controls 
     - Zoom
     - Pan

- World Generation
     - Basic Perlin-Noise Height Map

- Tile Interaction
     - Tiles stored in a TileMap 
     - Can click on a tile to see it's data, or delete it.

# First Impressions

In the next blog post, I'll be moving to more of a technical deep dive on each of the above systems, but rather then discussing the implementation currently seen in sandbox - I'll be detailing my process of taking the prototype and converting it into a proper feature implementation. I'm quite excited to being this process, as now that I've begun to get more comfortable with Rust, I can really sit down and architect implementations that use the language to its advantage. On that note, my first impressions of Rust have been extremely positive. Coming from C++, there were a few things that took a bit of getting my head wrapped around, but after spending the last few weeks with it nearly all of those complaints have gone away. With so many powerful features built write into the language, such as tuples and destructing, on top of an extremely expressive syntax - I couldn't help but fall in love with writing Rust code. That being said, while I wouldn't say I've had to "fight the borrow checker" yet, I still don't completely understand why or how it wants me to do certain things -- though I expect that to go away as I gain more experience. The only "real" flaw I've found with the language thus far, is that the compiler feels a bit slower compared to what I'm used too, and thats on top of C++'s already slower compile times. 

All-in-all, it's been an absolute blast to work in this language and can't wait to learn more about it's feature set. See you in the next post!