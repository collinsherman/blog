+++
title = "Theory of Computation"
subtitle = ""
image = "/img/portfolio/polyTime.PNG"
id = "theory"
sourceCode = "https://github.com/collinsherman/polyTimeAlg/blob/master/polyTimeAlg.py"
+++

In my Theory of Computation class, we were tasked with finding out if a Context Free Language was decidable or not.  To do this, we were to use an algorithm from our textbook that wasn't the easiest to look at, to say the least.  I kept getting tripped up along the way for one reason or another, so out of frustration, I decided to write a program that would follow the algorithm and print out the answer for me.

The basis of the algorithm was to use dynamic programming in order to have it run in polynomial time.  It stored each of the subproblems in an n x n graph that would be used for the further iterations of the algorithm.  I wanted to be able to see each step of the algorithm, so decided to have it print out the graph as well (which is pictured above).  It took a string as input along with a list of rules that would determine the decidability of the language.  If the graph had the starting node in the top-right corner position, then it would return "Accept" and I would know that the language was decidable with the given set of rules.  Otherwise, it would return "Reject," and I would know that it was not decidable.

With all of this in mind, you can follow along with the code on Github by clicking the link to the right.