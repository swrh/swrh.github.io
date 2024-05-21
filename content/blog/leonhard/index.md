---
layout: post
title:  "Leonhard"
date:   2016-10-24 21:15:00 -0200
---
After doing some thinking I decided to name the [Project Euler][project-euler] solutions project after [Euler][leonhard-euler] himself: [Leonhard][leonhard]. For now it's just a couple of [CMake][cmake] scripts with some simple C++ codes in it to serve as a boilerplate to solve and test the [Project Euler][project-euler] problems.

While designing it I thought it should at least be able to do the following:

1. include and execute any developed solution (in C++, of course);
1. test the result of a solution against a pre-defined value;
1. measure the time spent while executing any solution;
1. do all the steps above in batch mode (in one command only);
1. implement classes to be used as libraries in one or more solutions.

I believe if all the items above are achieved I'll have a nice place to solve the problems. I'll try to code it in the next days and, at least for now, it'll have just a command line interface. Let's see how this thing flows.

[project-euler]:  https://projecteuler.net
[leonhard-euler]: https://en.wikipedia.org/wiki/Leonhard_Euler
[leonhard]:       https://github.com/swrh/leonhard
[cmake]:          https://cmake.org
