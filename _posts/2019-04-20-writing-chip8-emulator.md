---
layout: post
title: Writing a CHIP-8 emulator
tags: [emulation, chip8, chip-8, nes, emulator]
comments: true
---

__TL;DR__: This post is not a tutorial for writing a CHIP-8 emulator. It just tells you how to get started into emulator development.  

If you are one of those people who likes to know how computer works at a very low level then you'll enjoy writing an [emulator][emulator] from scratch. And if you are just starting in the emulation field, I would say start with [CHIP-8][chip8]. It's not that complex and can be completed in two weekends. There is no better feeling in the world than playing a game on your own emulator. Writing an emulator is a journey full of __Aha..__ moments of both kind, realization one and excitement one. Even if you know how computers work internally in theory, after writing an emulator you'll look at them from a brand new perspective.  

It always felt like a daunting task to write an emulator, especially when there aren't any _tutorials_ or _step by step guides_ available on the internet. You might find some post here and there which will tell you how to start writing an emulator like this one but you have to do the hard work i.e. reading all the documentations available for that hardware. Once you understand the architecture of that hardware, the rest of the task is just implementing the different parts one by one and integrating them. As soon as you'll start writing code you'll realize that it's not that complex as it looks on the surface, given that you've read all the documentation.   

Here are some things that I learned from my journey:  

1. Start collecting all the documentations and make a pictorial representation of the hardware architecture. If you are emulating a console then chances are you won't find the official docs. You have to search in the forums for any unofficial documentation.

2. Divide the task into multiple parts. Usually those parts are implemented in this order: CPU, Display, Input and Sound. You can write and test these components separately. Writing unit tests first is a good idea here and will save a lot time while debugging later.

3. Start testing with simple test roms. Internet is full of such roms. The best thing about this is that if there is something wrong in your implementation, you'll be able to narrow it down easily. Though I would say unit tests should capture those first.

4. Persevere. Believe me, once you'll see your first rom running, nothing can second that feeling. It can be tedious at sometimes but don't give up. Take a break then come again. If you are stuck at some place, try to search online if anyone has faced that issue already. If not, then try to debug by yourself and post in those forums with your own solution.

__Details of my implementation:__  
I've written a CHIP-8 emulator in python3 using [pyxel][pyxel] library for graphics, input and sound. The code is in one file. You can find it over [here][code]. I know it's bad but will refactor it once I'll fix some minor bugs here and there. There is also a test file for some instructions. I used [pytest][pytest] for that.



[pyxel]: https://github.com/kitao/pyxel
[pytest]: https://docs.pytest.org/en/latest/
[chip8]: https://en.wikipedia.org/wiki/CHIP-8
[emulator]: https://en.wikipedia.org/wiki/Emulator
[code]: https://github.com/shivanju/chip8-python3