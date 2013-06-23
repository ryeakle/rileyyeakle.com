---
layout: post
title: Learning Programming
category: posts
---

Friends often ask me, 
>I want to learn how to program, how can I learn how to program? What should I do to start? 

##What do you want to learn?
Is your goal to learn how computers work? We're not talking about webapps and all that so called 'high level' nonsense. 
We're talking about electricity pulses flowing through tiny channels of
semiconductor, shaped into a useful structure for computation. This is 
the level of computation that interacts with the real world, where physics 
isn't just a nebulous memory from high school.

Or perhaps you think the circuits people did a great job. In fact,
they did such a great job at building this foundational platform 
for abstraction that it would be a shame to put all that work to 
waste. You want to harness this power to quickly spin out solutions
to your problems with the power of abstraction. Computers are like 
cars. Building them is certainly a worthy endeavor, but that's just 
the start. Really, the goal of cars is to move people from place to
place. It's the same with computers. Making the computer hardware work
in the first place is a challenge, but the more interesting challenge
is using this power to solve problems. 

I think these are two good starting points for learning to program: low-level first 
and high-level first. 

##If I knew more about programming, I'd know how to answer that!
###Low Level Programming
'Low level' in computer science refers to programs that are closely tied to
the physical hardware of the computer. These programs are directly connected
to the computer's actual circuitry. You might tell the computer to read a 
voltage off of an input, or toggle the bits in a register. The low-ness means
the level of abstraction. The lower level the program, the more the code
you write will actually resemble the machine instructions.

###High Level Programming
'High level' means the level of abstraction is... high. The code you write 
looks nothing like the actual instructions the computer executes. This is because 
someone smarter than you figured out how to take more human-friendly
input and turn it into computer friendly instructions. 

For example, in a medium level of abstraction, to open a door, you might say

1. Approach door
2. Identify handle
3. Lift arm to door
4. Grab handle
5. Twist knob
6. Push door
7. Release handle
8. etc. etc.

At a high level of abstraction, you realize that the procedure for opening
a door is well defined and you would simply say:

1. Open door

At a very low level of abstraction, you would go through the process of actuating
the muscles required to carry out the motions needed to perform the sub-tasks
needed to open the door.

##Low Level: Where Do Computers Come From?
If you want to know how computers actually work, or are interested in robotics,
this is a good place to start. I think the best way to get started with this
is with the [Arduino microcontrollers][arduino]. Microcontrollers are like tiny computers
without operating systems. You give them a program to run, and then they
run that program forever.

The tricky part about microcontrollers is that the learning curve usually 
looks something like this:

![img][learning curve]

What makes Arduino cool though is that they've eased the learning curve
and lowered the barriers for entry into the world of microcontrollers.

The community for arduino is unbelievably strong. there's plenty of beginner 
level support for those getting started online.

If this is the kind of thing you want to do professionally, you should 
transition to AVR or PIC microcontrollers. For hobbyist purposes though, 
Arduino is great. 

Start here if you want to get into: Robotics, home automation, computers that
interact with the real world.

##High Level: Poetry in Motion
If instead you want to rapidly deploy programs and applications on computers,
then high level programming might be a good place for you to start. With the 
power of abstraction, you can quickly bootstrap off the work of those before
you to make massively complex programs. 

The best way I've found to get started with this is by using Zed Shaw's [Learn 
Ruby/Python the Hard Way][lthw] book series. It's one of the few programming 
books I've seen that DOESN'T do something like:

>Ch. 1: Introduction

>Ch. 2: Variables 

>Ch. 3: Logic

>Ch. 4: Functions

>Ch. 5: Recursive Polymorphism in Non-deterministic Data Structures

High level programming is beautiful. Once you start, it's hard to leave. 
Principles like DRY (don't repeat yourself) and those awesome built-in 
data structures make for some elegant solutions to fundamentally complex 
problems.

Start here if you want to get into: web apps, scientific computing, the art of programming.

## Great! What if I want to do both?
Both is an option too. In fact, both is arguably the best option. 

It's important to remember no matter where you start, this takes time. It's like learning a new language. 
You may be able to pick up the syntax 100% within a few weeks, but learning to construct
excellent compositions using this language takes years of diligent practice. 

As you get started, I highly recommend you read the essay [Teach Yourself Programming in 10 Years][pn]
by Peter Norvig who drops some serious wisdom on the subject. In fact, you should probably do
that right... now. 

(Last update 2013-06-23)
[pn]: http://norvig.com/21-days.html
[lthw]: http://learncodethehardway.org/
[arduino]: http://arduino.cc
[learning curve]: /images/learn-programming/microcontroller-difficulty.png
