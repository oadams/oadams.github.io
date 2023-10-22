---
layout: post
title:  "A computer science curriculum"
date:   2022-06-11 00:00:00 +1000
categories: computer-science
---

- Targeted at Data Scientists who don't have a CS background, want to learn more, don't know what
    they don't know, and don't have all the time in the world.
- Three streams: (1) How computers actually work; (2) Theoretical Computer Science and (3) Software
    Engineering
- Rather than writing a series of talks, which is very time consuming, I want to leverage the
    existing array of stunning resources on the web that can be used. I want to shine a realistic
    path for a reader.
- The activities may require information not given up front, which means Socratic questions should
    be posed.
- Supplemental readings for bedtime mode are also listed. But note, real learning happens in an
    active way.
- It may be hard to pinpoint exactly how some of this knowledge would help the data scientist, while
    other examples (such as understanding Unicode) will very obviously help. But there are patterns
    of thought that some of this stuff exercises that generalizes elsewhere. Moreover, there will
    come times where understanding how things work under the hood a bit more will actually help in
    unexpected ways. Given the time investment required, it's not so bad.
- Some of these exercises may require some mental wrestling. That's a sign that you're growing. It
    *should* be a bit challenging. I'll admit I actually took some time to do the very first
    nandgame exercise: make a NAND gate out of some relays (transistors). I had to leave the
    computer and come back. Visualizing it lying in bed led me to the intuition behind the solution.

    That said, much of the learning here is to build a robust intuition, and a lot of the stuff is
    not strictly required. This is especially the case for something like microcorruption, where it
    gets hard really quickly. Once you hit a big roadblock, as long as you feel you have an
    understanding of how assemblers work, you are ready to move on.

- I've made a deliberate effort to constrain this curriculum to resources I personally have worked
    through, rather than texts that appeal idealistically, but might not be practical to read or
    work through.
- Because I am a computer scientist, however, it's possible working through these resources was
    easier because of some prerequisite knowledge I was unaware of. This is why Socratic questions
    is important for filling the gaps. Also, feedback to oliver.adams@gmail.com
- This document is also intended to be useful for computer scientists. There's a lot of articles
    about what CS people 'should' know about this and that, but that they don't actually really need
    to know for their job. This list is meant to be fairly minimal, but in doing it I'm actually
    learning stuff in a real bang-for-buck way too.

Where does stuff like leetcode fit into all of this?

Other stuff to look at:
https://primer.picoctf.com
projecteuler
leetcode

## How computers work:

Assuming you use Python to do your work, but know little about what goes on underneath.
This stream is about understanding computing from low level of abstractions to higher, thereby
demistifying everthing under the Python layer.

This means:
- from transistors to processors using nandgame.com
    - Supplemental questions:
        - Why do we need NANDs to make an AND when a transistor itself is basically an AND gate?
- Assembly/disassembly
- C programming.
- Operating Systems and Unix
- Networking, a tiny bit.
- Encodings like unicode and floating point operations.
- The Python Programming Language:
    - It's implementation in C
    - It's ins and outs, as per Fluent Python


Activities
- https://www.nandgame.com/
- https://microcorruption.com

### Nandgame:

TODO: Discuss.

### MicroCorruption:

This is a hands-on gamified way to become intimately acquianted with assembly. It uses the Texas
Instruments MSP430 family of CPUs. These are a bit simpler to get your head around than a CPU with
an x86-64 instruction set, but they share the same core fundamentals.

These exercises are quite difficult. Certainly this curriculum doesn't suggest that you need to do
them all. The goal of this step in the learning is to get a sense for assembly, and how CPUs work
with instructions. Getting a sense of how program counters, stack pointers, registers, opcodes all
work is the goal. Realistically after the first few challenges you'll have a decent sense and can
move on. Unless you're really enjoying it of course, in which case continue.

Some things that will be useful to know
- Hex (base 16) number representations.
- Endianness
- How things are addressed with bytes.

General tips:
- Determine the objective and then work back from there, getting a sense of dependencies along the
  way.

Estimated time. Perhaps a few sessions.


### Bed time readings:
- Code by Charles Petzold.
- Encodings https://tonsky.me/blog/unicode/. But caveat from hacker news discussion about why
    codepoints for length actually does make sense.
- The C Programming Language
- Operating Systems 3 Easy pieces
- Fluent Python

## Theoretical Computer Science

Big-O notation and algorithmic complexity Some classic algorithms to get a feel for the above.
    - Complexity of nested loops
Some must-know algorithms that you'll actually use in work:
    - Edit distance
    - Searching through a list versus checking if something is in a set.
Computability, halting problem, etc:


Bed-time reading:
- Sipser's book


## Software Engineering

Skills:
- Using a debugger
- Using a line_profiler
- Refactoring

## Machine Learning

Basically build up to a large language model.

## Notable Omissions

It's worth noting what is missing from this curriculum. Aside from stuff missing within the stated
topics because we don't go that deep, some topics are completely omitted:
- Databases
