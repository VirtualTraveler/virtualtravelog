---
layout: post
title: "The Misapplication of Occam’s Razor or the Principle of Inappropriate Parsimony"
description: "In practices solutions based on these simple, low fidelity, models fail to handle the problem completely and often causes a whole series of new problems."
tags: [system design, failure]
modified: 2016-12-22
redirect_from: 
  - /entries/000032.html
  - /entries/2002/12/the_misapplication_of_occams_razor_or_the_principle_of_inappropriate_parsimony.html
---
There is a class of design problem that can mislead the unwary systems designer, myself included, although I am getting better at identifying the warning signs. These design problems require the designer to base the solution on a conceptual model of a real world system or process. It often appears that a simple conceptual model that approximates to the real world system will suffice. In practices solutions based on these simple, low fidelity, models fail to handle the problem completely and often causes a whole series of new problems. Redesigning the solution to handle these exceptions only produces more problems that require more redesign and so on. If the hapless designer persists s/he will often go through several complete redesigns before getting to a solution that finally solves the problem by modeling the real world system with a high degree of fidelity. This iterative redesign process is typical of this class of design problem. Some might say that only poor designers are ever trapped in this way, others will say these solutions are anti patterns. But I think there is more too it.

The type of design problem under consideration here is particularly intractable because there exists a series of approximate conceptual models of increasing fidelity and complexity. Faced with situations like these many systems designers will claim to be applying Occam’s razor when they opt to base their solution on the simplest conceptual model. But, a solution based on an approximation is only as good as the approximation. The only way to improve such a solution, if it is insufficient, is to replace the low fidelity conceptual model with one of higher fidelity. The worst type of problem is one that has many plausible conceptual models each of slightly higher fidelity and complexity than the last. The slavish misapplication of the principle of parsimony will condemn our systems designer to step through each successively higher complexity model until they finally reach one with the required fidelity.

> Occams Razor – When faced with several explanations of a phenomenon One should always choose the simplest, the one that requires the fewest leaps of logic

This leads to a tentative conclusion: Occam’s Razor is no good for selecting between alternative models if the alternatives are approximations with differing fidelity. A simple low fidelity model cannot be compared with a complex high fidelity one.

An old joke comes to mind. An engineer, a physicist, a mathematician and a biologist were asked to define Pi: The engineer said About 3, the physicist said 3.14159 +- 0.00001, the mathematician said The circumference of a circle divided by its diameter and the biologist said What is Pi. Choosing the least complex, lowest fidelity model is not always the right answer! Too many systems designers think there is virtue in always assuming Pi should be about three.