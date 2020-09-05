---
layout: post
title: "Start of my new project! Ilum!"
author: Lockna
---

# Start of my new embedded project! Ilum!

Hey guys! In this post I want to share my new project ilum.


### What is Ilum?
Ilum is collection of rust crates, to bring support for the Rust programming language to the Teensy 4.0.
Another name for this kind of things is board-support-package.

Ilum will consist of three crates
- ilum-init
- ilum-hal
- ilum-bsp

#### ilum-init
ilum-init will set up and initialise the CPU for further usage.
This crate will have the bootdata needed by the cpu and the memory layout of the iMXRT1062.
I'm going to start with this, since I need it for my other crates.

#### ilum-hal
ilum-hal is gonna be a hardware-access-layer, so I can easily interact with the hardware with ilum-bsp.
I believe this will be the most time consuming of the three crates.

#### ilum-bsp
This will be the main crate of ilum. With this crate, you will be able to write Rust for Teensy 4.0.
It depends on the previously mentioned crates. 
I will try to write proper functions so that you can easily use the Teensy and it's features.


### Why do I write all things myself?
Yeah, you can call me stupid, but I do not want to follow the template that crates like [embedded-hal](https://github.com/rust-embedded/embedded-hal) or [cortex-m](https://github.com/rust-embedded/cortex-m) give me. 
I prefer to start from scratch, so that I really understand everything and not just skidding something from another project.
I don't expect it to be easy for me either, but I can live with that.
I also reckon that it will take me a few months to get anything to work at all.


### Conclusion so far
So far I'm quite happy with my decision. I have learned already a lot about the inner workings of a mcu and I'll continue my research about it.
My first goal is to get a working initialition process for the cpu :)


I will keep you up to date

