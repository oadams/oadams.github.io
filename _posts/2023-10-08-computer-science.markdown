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


## How computers work:

Assuming you use Python to do your work, but know little about what goes on underneath.
This stream is about understanding computing from low level of abstractions to higher, thereby
demistifying everthing under the Python layer.

This means:
- from transistors to processors
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

Bed time readings:
- Code by Charles Petzold.
- Encodings https://tonsky.me/blog/unicode/. But caveat from hacker news discussion about why
    codepoints for length actually does make sense.
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
