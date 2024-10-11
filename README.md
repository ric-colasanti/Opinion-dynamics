# Opinion-dynamics
NetLogo Opinion dynamics 

## Overview:

Purpose: The model simulates the opinion dynamics of a group of persons with different levels of extremism and uncertainty.

Entities/Individuals: The individuals in the model are called "persons", and they have two attributes: opinion and uncertainty.

Process/Mechanisms: The persons interact with each other through one of two opinion update rules: Deffuant or Edmonds. The opinion update rules consider the distance between the persons' opinions and their uncertainty levels.
Environment: The environment is a two-dimensional space with a fixed size and scale.
Simulation time: The simulation runs for a specified number of iterations.

## Design concepts:

Interaction: The persons interact with each other through the opinion update rules, which consider the distance between their opinions and their uncertainty levels.
Stochasticity: The model includes randomness in the initial opinions and uncertainties of the persons, as well as in the choice of interaction partner.
Collectives: The collective behavior of the persons emerges from their individual interactions and opinions.
Observation: The model tracks the opinions and uncertainties of the persons over time.

## Details:

Initialization: At the beginning of the simulation, the model creates a number of persons with initial opinions and uncertainties. The persons are distributed in the environment according to their opinions.

Input: The user can specify the number of persons, the number of iterations, the initial moderate and extremist uncertainties, and the opinion update rule (Deffuant or Edmonds).

##    Submodels:

The setup procedure initializes the environment and the persons.
The scale-opinion reporter calculates the y-coordinate of a person based on its opinion.
The go procedure runs the simulation for a specified number of iterations.
The update procedure updates the opinion and uncertainty of a person based on the chosen opinion update rule.
The average procedure calculates the average opinion of a person and its interaction partner.
The g and f reporters calculate the interaction strength between two persons based on their uncertainty levels and the opinion distance.

The deffuant and edmonds procedures implement the Deffuant and Edmonds opinion update rules, respectively.

## Output: 
The model outputs the opinions and uncertainties of the persons over time. The user can visualize the simulation and observe the emergent behavior of the collective.


## References   

Rainer, Hegselmann, and Ulrich Krause. "Opinion dynamics and bounded confidence: models, analysis and simulation." (2002)  
Deffuant, Guillaume, Frédéric Amblard, and Gérard Weisbuch. "Modelling group opinion shift to extreme: the smooth bounded confidence model." arXiv preprint cond-mat/0410199 (2004)   
Edmonds, Bruce. "Assessing the safety of (numerical) representation in social simulation." 3rd European Social Simulation Association conference (ESSA). 2005.

