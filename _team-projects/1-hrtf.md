---
title: HRTF (Fall 2019)
permalink: /portfolio/HRTF.html
lang: en
projectUrl: qhn-dYVmGnQ
cover: http://img.youtube.com/vi/qhn-dYVmGnQ/0.jpg
---

{% contentfor project-description %}

This is a Custom HRTF Plugin created for the Wwise Audio Middleware. 

I wrote this plugin from scratch over the course of 4 months, and was responsible for all design and implementation of the HRTF FIR Filter.

This project was a great introduction for me into the realm of real-time DSP and optimizations. Initially, I started this project with my Object-Oriented Programming mindset and went to work. However, I quickly discovered that when working on low-level audio subsystems, function calls, loops, and more can have a serious impact on performance. 

This required me to shift away from the design patterns I was used to and adopt a more data-oriented design focus. By taking a step back and writing code that focused on efficient memory layout, and easy vectorization, I was able to see a performance increase of 3 simultaneous HRTF objects, to 100.  

{% endcontentfor %}

{% contentfor dev-details %}

- __Language__: C++

- __Target Audio Middleware__: Wwise

- __Development Cycle__: September 2019 - December 2019 

(4 Months)

- __Team Role__: Audio and Systems Programmer

- __Team Size__: 7

{% endcontentfor %}
