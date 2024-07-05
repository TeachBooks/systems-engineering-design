# 1. Introduction to the Book

<div style="text-align: center;">
  <img src="./images/erasmus.png" alt="erasmus" width="70%">
</div>

**Systems engineering design** is about formalizing and managing the process that leads to the creation of engineering design artifacts. It focuses on the process that started with a set of vague societal needs that require addressing. At the end of this formalized process is the end result, the engineering artifact that serves as the solution to address the societal needs. Engineers are typically more interested in the engineering design object itself, without focusing too much on the societal needs to which the designed engineering artifact should be the solution for. In short, their focus is on the object, not the process.

Turning the focus to the engineering design object too quickly, paying little to no attention to the societal needs that are the base of the engineering design problem, is likely to end up in engineering design solutions to problems that do not exist, i.e. building that which no one wants. Take the design of the VPRO head office where key stakeholders were neglected in the design process resulting in a building that was not fit for its intended purpose.

Focusing on societal needs is in line with what is stated in TU Delft's mission statement: *"We develop technology-based innovations for some of our society’s biggest challenges."*

The problem is formally a discrepancy between the societal needs of stakeholders versus what the engineering artifact can provide. The societal needs relate to the objectives of stakeholders (which is the domain of the social sciences) and the configuration of the to be designed engineering artifact (which is the domain of the natural sciences). The goal is to find that design configuration that has the highest overall group preference and also does not violate constraints related to physics. Put simply, the design configuration that is most desirable but also feasible.

The societal needs relate to the interests of each stakeholder, the value they want maximized, i.e. their preferences. The configuration of the artifact relates to constraints, i.e. a design space with feasible design configurations. A classical approach is that the designer creates a number of design alternatives from which the stakeholders have to select one by negotiation.

Choosing from a set of design alternatives is **a posteriori** decision making (after the fact). This means that the decision makers are faced with a fixed and limited set of design alternatives to choose from. The question is whether the designer did a proper job in interpreting each stakeholder's preferences into each of the design variants. It is quite likely that the designer overlooked a design configuration that would better represent all stakeholders interests.

A more preferred approach would be to have a formal **a priori** design methodology where the most preferred design configuration is the output of integrating both the stakeholders interests and constraints that apply.

The purpose of this book is to provide the reader with such a methodology to solve multi-stakeholder engineering design problems. The design process is modeled using a mathematical optimization model because of the isomorphisms [^isomorphisms] between design and mathematical optimization problems. Although mathematical optimization is being used to solve such problems, classical approaches are problematic for two main reasons: 
1) the scales used for rating candidate design solutions on preference do not enable fundamental mathematical operations, and 
2) the commonly used weighted arithmetic mean algorithm for aggregating ratings and weights yields an infinite amount of outcomes.

<!--more-->

Engineering design is distinct from empirical research. In Chapter 2 we make this distinction to clearly define the differences but also how they relate and how empirical research and engineering design depend on each other.Engineering design commonly relies on modeling and simulation, the basics of both are described in Chapter 3. Because of the isomorphisms between (engineering design), mathematical optimization, systems thinking and decision making all of these are formally defined in Chapters 4 to 7 respectively. This then leads to the formal description of the preference-based engineering design methodology which is described in Chapter 8. A number of Preference-based Engineering Design applications are then used in Chapter 9 to illustrate how the methodology can be applied to real life (engineering) design problems. We end the book in Chapter 10 with a reflection on the methodology itself and its broader use and implications.


[^isomorphisms]: An isomorphism is a one-to-one correspondence between two structures, such that the relationships and operations defined on one structure are preserved in the other. In design and mathematical optimization, this means that a design problem can be mapped to an optimization problem in a way that preserves the problem's essential characteristics and constraints.
