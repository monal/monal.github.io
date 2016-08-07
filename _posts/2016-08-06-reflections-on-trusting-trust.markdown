---
layout: post
title:  Reflections on Trusting Trust - Ken Thompson [Reading]
date:   2016-08-06
categories: ['reading']
---
<cite>
Ken Thompson. 1984. Reflections on trusting trust. Commun. ACM 27, 8 (August 1984), 761-763. DOI=http://dx.doi.org/10.1145/358198.358210
</cite>

The paper talks about how we cannot trust a piece of code to be free from Trojan horses and how it's more important to trust the person who wrote that piece of code. The author gives a talk about how 
you can edit the C compiler source code to add a piece of self-reproducing code in C (code that prints itself as output) which does pattern matching to redirect logins to a "bug" intentionally. The source code is then run against the standard, existing binary file of the compiler. This will produce a new binary that can be used as the C compiler from now on(with the Trojan horse in it). If the user then proceeds to erase the added lines from the source code, the probability of catching the Trojan horse becomes quite less.
