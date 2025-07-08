---
layout: cv
type: webpage
permalink: resume.html
show_title: false
---

# Anthony Avancena-Brigante

<div class="screen-only Grid Grid--gutters large-Grid--fit u-textCenter u-contactInfo">
  <div class="Grid-cell">
    <a href="mailto:anthonyprbrigante@gmail.com" >anthonypbrigante@gmail.com</a>
  </div>
  <div class="Grid-cell">
    <a class="screen-only" href="https://www.linkedin.com/in/apbrigante">LinkedIn</a>
  </div>
  <div class="Grid-cell">
    <a class="screen-only" href="https://www.github.com/abrigante1">GitHub</a>
  </div>
</div>
<div class="print-only Grid Grid--gutters large-Grid--fit u-textCenter u-contactInfo">
  <div class="Grid-cell">
    anthonypbrigante@gmail.com
  </div>
  <div class="Grid-cell">
    631-626-1405
  </div>
  <div class="Grid-cell">
    www.abrigante.com
  </div>
</div>

## EDUCATION

### Bachelor of Science in Computer Science
`July 2021` 
<span class="degree">DigiPen Institute of Technology</span>

## TECHNICAL SKILLS

<p class="tech-skills">
<strong>Programming Languages:</strong>
Modern C++, C, C#, Python<br> 

<strong>Libraries:</strong>
Wwise SDK, ImGui, Qt<br>

<strong>Game Engines:</strong>
Entity-Component-System (ECS) Architecture, Unreal Engine, Unity<br>
</p>

## PROFESSIONAL EXPERIENCE

### ZeniMax Online Studios
Senior Audio Engineer - Unannounced MMORPG
`Nov 2021 - July 2025`
- **Led** a three-person audio engineering team in building a State of the Art audio tech stack.
- **Mentored** associate audio engineers in best practices for our custom engine's ECS architecture and tool development in Qt.
- **Oversaw** comprehensive task planning and prioritization for the audio team in collaboration with audio and production leadership.
- **Nurtured** a culture of technical ownership, serving as the sole technical product owner for audio and championing our sonic vision.
- **Implemented** an ECS-centric Wwise integration creating a ergonomic event-based API for interacting with the Sound Engine
- **Developed** a full suite of in-house audio tools and pipelines from the ground up, with a focus on rapid Sound Designer iteration.
- **Engineered** a background service application that automatically synchronized Wwise Assets with our Engine Asset database
- **Invented** a robust data assignment pattern for Audio that was promoted to be a core engine feature adopted by multiple teams
- **Enabled** our Composer to create dynamic musical soundscapes by designing and implementing a highly flexible Music System.
- **Rearchitected** our Acoustics integration resulting in a more maintainable codebase alongside performance gains of over 100ms.
- **Authored** a projectile whizzby system with user facing design parameters to allow Sound Designers to  express their artistic vision
- **Prototyped** a dynamic game mix system driven by various pieces of game context such as combatant threat and player significance. 
- **Built** a robust suite of ImGui-based debugging tools for easily visualizing all relevant audio data for any given entity
- **Spearheaded** dynamic resource loading initiatives and enhanced resource dependency tracking methodologies.

### DPS Games
Audio Programmer - Tomorrow Falls
`Jan 2021 - July 2021`
- **Collaborated** with the Audio Design team to develop and implement foundational C++ Audio Systems in the Unreal Engine that
allowed for a more responsive soundscape
- **Architected** networked game utilties that consolidated widespread code into a single location for use by all development disciplines.
- **Documented** both technical design documents and user guides for all implemented audio systems.
- **Implemented** audio debugging tools to help quickly locate bugs and iterate on features.
- **Developed** a dynamic whoosh system that triggered sound effects as players passed geometry at high speeds, accurately simulating the Doppler Effect.

### Qualcomm
Audio R&D Intern, Multimedia R&D Team
`June 2020 - Sept 2020`
- **Researched** methods of minimizing audio motion latency in interactive experiences to provide a more enjoyable and responsive experience for the listener.
- **Prototyped** new spatial audio streaming technologies to bring high-quality immersive audio experiences to a wider consumer audience.
- **Developed** a custom end-to-end audio experience in C++ and JavaScript to demonstrate the viability of the prototyped technologies.

### Tsugi Studio
Audio Programming Intern
`May 2019 - Aug 2019`
- **Built** an application in C# to dynamically generate and compile C++ software for 3 different platforms.
- **Optimized** C++ DSP Code to achieve a performance increase of ~4900% via Data Oriented Design and SIMD assembly intrinsics.
- **Ported** C# DSP objects into C++.
- **Wrote** a C/C++ Fast Fourier Transform capable of using a 4096-byte window in real-time.

<div class="disabled-print" markdown="1"> 

## AUDIO PROGRAMMING PROJECTS

### [Granular Synthesizer](portfolio/granular_synth.html){: .u-project }
`March 2019 - May 2019`
- Learned the fundementals of the JUCE Audio C++ API
- Implemented an effecient system capable of running 10 large grain clouds simultaniously in real-time.
- Architected a randomization system for a grain's start/stop positions to create unique sound textures.

### [HRTF Wwise Plugin](portfolio/HRTF.html){: .u-project }
`September 2018 - December 2018` 
- Researched HRTF filter design and architecture to gain experience with spatialization DSP. 
- Developed a custom time-domain HRTF plugin in C++ capable of spatializing ~100 concurrent audio sources to allow for creation of more immersive player experiences
- Learned the inner workings of the Wwise Plugin API to expand my understanding of Wwise and it's API ecosystem.

### MIDI Synthesizer
`Jan 2017 - May 2017`
Course: Introduction to Audio Programming (ECE101L)
- Prograbundlmmed an ARM Microcontroller to be an Additive MIDI Synthesizer.
- Designed  a system to parse and understand MIDI Commands in real-time.
- Gained Experienced with Q-Format Integer Math
</div>

<div class="disabled-print" markdown="1"> 

## ACADEMIC GAME PROJECTS

### Gameplay Programmer
`September 2020 - December 2021`
Aster - Team Size: 6
- Developed a Spell Crafting and Combat Game built in Unreal Engine 4 focused on making players feel like a powerful Mage.
- Prototyped a basic Spell interface that helps the team quickly create new and interesting spells.
- Designed a Spell Crafting System implementation that lets players combine spell components to create a variety of unique spells.

### Gameplay Programmer | Technical Director
`September 2018 - April 2019`
[Higher Power](portfolio/HigherPower.html){: .u-project } - Team Size: 7

- Built a VR God Game for the Oculus Rift using Unreal Engine 4.
- Designed and Programmed a C++ Temperature System to provide new and exciting emergent gameplay experiences for our players
- Implemented a Blueprint Wrapper around the Temperature System to help designers quickly tweek and modify the underlying logic.
- Ensured that code quality adhered to style and performance standards by using an Unreal Style Guide.

### Core Engine Programmer | Tools Programmer
`Sept 2017 - April 2018`
[Contingency](portfolio/ember_editor.html){: .u-project } - Team Size: 7

- Created a Custom 2D Game Engine in C++ and OpenGL with a user-friendly API.
- Architected and Implemented a component system for dynamic Game Object Creation to allow for robost and rapid prototyping.
- Designed and Built a scene and game object editor using ImGUI to allow our Game Designers to work in-engine with no programming required.

## TEACHING & LEADERSHIP EXPERIENCE

### DigiPen Institute of Technology
Teacher's Assistant - Introduction to Audio Programming
`Jan 2018 - May 2020`
- Mentored over 40 students on the fundementals of audio programming.
- Taught students how to build an Additive MIDI Synthesizer on an ARM microcontroller.
- Graded programming assignments based on high-quality code via style and performance metrics.

### ProjectFUN 
Lead Instructor - Video Game Programming (AP Computer Science A)
`May 2018 - August 2018`
- Co-instructed a class of 30 students the foundations of Java through video game programming 
- Refined the existing course curriculum to be bought up to date with modern Comp. Sci. content
- Engaged students in hand-on learning of Java programming with well-defined benchmarks and game development milestones

### We Connect the Dots (Non-Profit)
Community Ambassador
`Jan 2016 - Jan 2017`
- Taught a weekly extracurricular TouchDevelop course a class of 20 5th graders to encourage the learning of
Computer Science at an early age
- Lectured an audience of 150+ students ranging from 13 - 18 on the basics of Computer Programming
- Presented We Connect the Dots to a panel of Harvard Business School Judges as a part of a venture captial competition

</div>