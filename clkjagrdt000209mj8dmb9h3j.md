---
title: "Complexity Notes from "The Art of Unix programming""
datePublished: Wed Jul 26 2023 05:32:08 GMT+0000 (Coordinated Universal Time)
cuid: clkjagrdt000209mj8dmb9h3j
slug: complexity-notes-from-the-art-of-unix-programming
tags: complexity

---

### [Complexity](http://www.catb.org/~esr/writings/taoup/html/ch13s01.html)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1690349627494/6fe75e27-8813-42ce-87e5-3cd4818b48c3.png align="center")

*Accidental complexity* happens because someone didn't find the simplest way to implement a specified set of features. *Accidental complexity* can be eliminated by good design, or good redesign.

*Optional complexity,* on the other hand, is tied to some desirable feature. *Optional complexity* can be eliminated only by changing the project's objectives.

When we fail to *distinguish between optional and accidental complexity*, design debates become seriously confused. Questions about what a project's objectives are get confused with questions about the aesthetics of simplicity, and whether people have been sufficiently clever.

*Accidental code complexity* (making code more complicated than it needs to be to get the job done) often results from *premature optimization.* *Accidental codebase* bloat often results from violating the *SPOT rule*, duplicating code or organizing it poorly so that opportunities for reuse aren't recognized.

<mark>Essential interface complexity</mark> usually can't be cut without trimming the basic functional requirements for the software

Sources of *optional complexity* are the most difficult to make useful generalizations about, because they so often depend on delicate judgments about which features it is worth paying the complexity cost for. Optional interface complexity often comes from adding convenience features that make life easier for users but aren't essential to the function of the program.

Optional increases in codebase size (supposing the user-visible features and the algorithms used are held constant) can often come from various sorts of practices intended to make it more maintainable — adding mode comments, using long variable names, and so forth. Optional implementation complexity tends to be driven by *everything* that touches a project.

The *sources of complexity have to be grappled* with in different ways.

Codebase size can be attacked with better tools.

Implementation complexity can be addressed with better choice of algorithms.

Interface complexity has to be addressed with better interaction design, a skill involving considerations of ergonomics and user psychology.

(This skill is less common (and possibly more difficult) than writing code)

Attacking the kinds of complexity, on the other hand, has to be done more with insight than with methods.

You *cut accidental complexity* by noticing that there is a simpler way to do things.

You *cut optional complexity* by making context-dependent judgments about what features are worthwhile.

You *can only cut essential complexity* by having an epiphany, fundamentally redefining the problem you are addressing.