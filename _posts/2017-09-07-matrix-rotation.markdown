---
layout: post
title:  "First steps"
date:   2017-09-07 16:09:00 -0300
---
The project is now bootstrapped: the CMake scripts to build the library and executables and link them to the dependencies and the [Travis CI][lozti-travis] is setup. I started by coding the main class (named it just `logic`), created a `lozti` namespace to separate my things from the rest of the world and it should be ok for now. Aside from `logic` there is the `piece` and the `matrix` classes, but they are not ready yet to be commented.

I do something that many condemn: I always try to use STL, Boost and templates first, not worrying very much if the code will be unreadable for the newbies. I known people think it's not so nice but I don't have problems when I re-reading my code even a year later. I think the code should be readable but I don't think *everyone* should be able to read it, unless the readability doesn't condemn the elegance of your program. Most of the programmers I know doesn't remember what ``std::find_if`` exactly does but I prefer to use it in my code instead of a 4-line loop just because STL is not evil and everyone should know it by heart (and because it's easier to write sometimes). Oh, and of course: I do this *unless the owner of the code I write (a.k.a. my employer) asks me to do otherwise.*

Anyway, I like inheritance avoiding and the way STL and Boost uses templates and I intent to do that aswell. You might see very few virtual methods in my code and maybe many templates. Sometimes the `vtables` come in the way of the performance and, although I know it is very rare, I prefer to leave it behind. I'm saying this because I think I might need ``std::array`` AND ``std::vector`` matrices and I don't intent to use inheritance to make other classes support both. But I might be wrong. Or not.

:)

[lozti-travis]:   https://travis-ci.org/swrh/lozti
