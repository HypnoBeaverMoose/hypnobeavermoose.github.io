---
layout: page
title: Resume
permalink: /resume/
---

---

## Work History 
---
### Lead Engineer 09/2022 - 09/2023
#### [Raraland Inc](https://www.rara.co/)

After acting as a de facto Lead Engineer for a period of time I was officially promoted to Lead Engineer at Raraland. During this period my duties slowly shifted to maintaining the software and working closely with the rest of the team to help them develop the features we needed. I also oversaw a major pivot in the business model and product strategy.

 - Performance improvements (of up to 50%) for visual scripting system and overall engine.
 - Reduced loading times and restructured backend to support local storage of games. Overall, this reduced the average loading time by around tenfold.
 - Implemented gameplay improvements, such as improved character controllers and navigation, which simplified and expanded the types of games, that could be created.
 - Oversaw implementation of major features and ensured code quality and stability.

My time was split 50/50 between programming and coordinating with the rest of the team. I also had important participation in product design for a lot the features and overall planning and direction of the company.

---

### Senior Engineer  09/2020 - 09/2022
#### [Raraland Inc](https://www.rara.co/).

Raraland Inc. is a US-based startup, that aims to revolutionize how people create and share games. The company's flagship product Rara was a mobile engine, that allowed users to create and share games entirely on their mobile devices. It was in a way similar to Roblox, however, the game creation was strictly mobile. The entire engine was built on top of Unity.

During this period I built a major part of the engine and was responsible for a lot of the architectural decisions. I also took up a large long running refactoring effort to improve stability and development velocity, while at the same time pumping out features. Basically, we were changing the tires while racing.
 - Core Architecture - How the engine was built. Entities, Instances, Components, Properties etc. Three different types of data models:
   - Backend - how the a game was represented on the server along with backwards compatibility.
   - Editmode - what the game creator sees, including different entities, components, and properties.
   - Runtime - what the player sees. The elements in edit mode instantiated, interacting and changing in realtime.
 - Game Editor - The main thing a user interacts with in the engine. Made up of a 3D view, UI elements for selecting and modifying gameplay elements. Instant transition between playtesting and building the game. Interactive UI feedback when different parameters are being edited.
 - Rule System - A scripting system based on text and autocomplete, rather than nodes and connections. A full fledged extensible programming language, that allowed the user to modify the behaviour of any part of the engine

Additionally, I participated in the design and implementation of other major features such as realtime multiplayer, a character creator and various social network features.

---

### Lead Game Developer 07/2019 - 06/2020
#### [Dreamteck](https://dreamteck.io/)

At Dreamteck I led the development of [Lifeslide](https://lifeslide.io/) - a paper plane flight simulator game, that combined a zen aesthetic with challenging gameplay. The game was a chosen to be a launch title of the then upcoming subscription platform [Apple Arcade](https://www.apple.com/apple-arcade/). The game was built in Unity 3D, and as part of the contract with Apple required to run on a number of devices: 
 - IPhone (the lowest tier was 6s)
 - IPad
 - AppleTV (both versions, and a full support for the Apple Remote)
 - iMac
 - Mac

At the start, the game was a promising PC prototype with many stability issues, including problems with graphics performance and tremendous memory leaks. I joined a team of young professionals, some of which had very little experience and together we managed to bring Lifeslide to Arcade in less than 3 months. My duties included, but were not limited to:

 - Working closely with studio head / product owner and publishers on determining development priorities requirements, estimates and deliverables
 - Establishing and maintaining various development processes, taking part in optimizing
other parts of the development pipeline – level design, art, etc.
 - Implemented CI using TeamCity and various other dev-ops work.
 - Porting to iOS, tvOS and Mac.
 - Major refactoring work for improving the stability of the game.
 - Created a menu system.
 - Implemented various gameplay mechanics.
 - Respawn system, that automatically guided the player away for obstacles and danger.
 - Different game modes (Arcade, Zen, Challenges)

---

### Senior Game Developer 04/2018 - 07/2019
#### [Dapper Penguin Studios](https://dapperpenguinstudios.itch.io/)

Dapper Penguin Studios hired me to help them with the release of their hit game "Rise Of Industry". As a senior developer I was in a team with two other developers and a number of amazing artists and designers. I was responsible for implementing and owning entire game mechanics across all stages of software development.
Some of the larger mechanics, that I built were:

 - Innovative logistics system, that uses dynamic programming to continuously solve the [knapsack problem](https://en.wikipedia.org/wiki/Knapsack_problem).
 - Pollution mechanic implemented as a compute shader.
 - Traffic visualization system based on Unity's Job System.
 - Dynamic in-game events.
 - Budget system.

In terms of technologies, I mainly worked with Unity 3D. In addition, I handled various day-to-day tasks:

 - Performance optimization - profiling, multithreading.
 - Maintaining and implementing UI systems.
 - Various graphics tasks – writing and maintaining shaders.
 - Improving existing procedural world generation solution.
 - Cross-platform support (Linux, Mac, PC).

---

### Freelance Game Developer 02/2014 - 04/2018
During this period I focused on game development for various clients. Mostly through [Upwork](https://www.upwork.com/freelancers/~01492cfede161f1deb), but also other channels. There are several notable games and projects I worked on:

- [Terraria](https://play.google.com/store/apps/details?id=com.and.games505.TerrariaPaid&hl=en) - I was hired by dutch studio Codeglue to help out with porting Terraria to mobile devices. The mobile port was developed in C++ using the studio's custom engine.
- [The Universim](https://store.steampowered.com/app/352720/The_Universim/) - As well as many other developers I had a tenure at Crytivo,  working on the never ending fairytale, that was The Universim. The project was developed Unity3D. I was mostly responsible for new gameplay mechanics, and UI.
- [Rocket Riot](https://store.steampowered.com/app/460190/Rocket_Riot/) - Another project for Codeglue. This time they needed me to bring their game Rocket Riot to XBLA
- [Ivalalearn](https://www.ivalalearn.com/) - An online medical imaging platform design to help veterinary medicine students. Ivala had a plethora of repos (20 - 30) that shared a common base, which was separated in a git submodule. The work involved a lot of Python scripting and git plumbing work. Basically I built a tool in Python to make sure all the projects were up to date whenever the base was changed. Additionally I built a medical imaging viewer using a ray-marching algorithm. All of the projects were implemented in Unity3D.

There are also a number of less notable clients and projects. Most of the work was done in Unity, with the occasional C++ project.

---

### Senior Software Developer 07/2012 - 02/2015
#### [Scopic Software](https://scopicsoftware.com/)
Scopic Software is an outsourcing company, which at the time specialized in computer graphics and web development. 
While at Scopic I worked for a number of clients, primarily using C++, but also

- UI frameworks like Qt and WinForms,
- Graphics API - OpenGL, DirectX, and CUDA
- Computer Vision libraries such as OpenCV

The more notable clients I worked for during that period:
- [Sketchlist 3D](https://sketchlist.com/) - A woodworking and design application built using Qt and OpenGL. My responsibilities were primarily to maintain the software, implement some new features and refactor the code to improve development velocity and stability.
- [Tomographix Quantiva](https://scopicsoftware.com/portfolio/tomographix-quantiva-workstation/) - Medical imaging application, that employed cutting edge technology to render CT, MRI, etc. The visualization relied on Sparse Voxel Octtrees, which were implemented on the GPU using CUDA. Datasets were streamed directly from HDD to the GPU on demand, whenever the user needed to visualize a particular part of the dataset.
  - Maintained and improved an existing renderer based on [Sparse Voxel Octtrees](https://en.wikipedia.org/wiki/Sparse_voxel_octree)
  - Worked on image registration and supporting various aspects of the DICOM format.
  - Optimized streaming of data from HDD to GPU. 
  - Implemented image compression using the Wavelet Transform.

---

### Game Developer 11/2011 - 06/2012
#### [Bon Art Studio](https://1050.studio/redirect)

In 2011 Bon Art was a art outsourcing company that wanted to establish its own game development offshoot - [Ludus Studio](https://www.ludusstudio.com/). I was one of their first hires.

Worked on three games for the company:
- [Board Defenders](https://www.ludusstudio.com/board-defenders/)
- [Toon Clash Chess](https://www.ludusstudio.com/toon-clash-chess/)
- [Foosball Cup](https://www.ludusstudio.com/foosball-cup/)

"Board Defenders" and "Toon Class Chess" were both developed in Unity 3.5, I was responsible for most of the code and reported directly to the studio head.
"Foosball Cup" was built in an internal engine in C++ and I was responsible for some graphics improvements and gameplay.

---

## Education
---
### Masters Degree "Game And Media Technology"
#### [Universiteit Utrecht](https://www.uu.nl/en) 09-2012 - 12-2014 

Utrecht University is one of the leading institutions in Europe in the in the fields of natural sciences and technology. It routinely get's ranked as a top 5 university. 

The program [Game And Media Technology](https://www.uu.nl/en/masters/game-and-media-technology) focuses acquiring knowledge and abilities to do cutting edge research in the fields of computer games, graphics, and multimedia.
Basically, we learned about the stuff, that was going to explode in the next few years.

- Pattern Recognition and Neural Networks
- Computer Vision
- Computer Graphics
- Virtual Reality

My master thesis focused on computer graphics and in particular how to speed up convergence of photon maps using local symmetry in the underlying geometry. You can find it [here](https://studenttheses.uu.nl/handle/20.500.12932/18840) 

---

### Bachelors Degree Informatics
#### [Sofia University](https://www.fmi.uni-sofia.bg/en)  09-2007 - 07-2011 
A standard computer science course, that covers a wide range of disciplines related to the field. 

- Analytic Geometry
- Linear and Higher Algebra
- Calculus
- Computer Graphics
- Data Structures and Algorithms
- Discrete Mathematics
- Numerical Methods
- Object Oriented Programming
- Differential Equations

In general, the programs at Sofia University tend to be a little heavy on the mathematical side, but that's something I learned to appreciate later in life. Turns out its easier to learn Javascript than figure out Fourier transform on your own.

---