# Grid-honeycomb
Note that most of the grid changing actually occurs with the ``` nth-child+n ``` class where specifying the ```nth-child ``` with ```n```
makes it less code heavy when specifying a specific hexagon.
In this case, ```3n+2 ``` was chosen for:

**Cycle 1: (3 x 0) + 2 = 2** 

**Cycle 2: (3 x 1) + 2 = 5** 

**Cycle 3: (3 x 2) + 2 = 8** 

**Cycle 4: (3 x 3) + 2 = 11** 

Whereas for formatting the positions of the hexagons with ```translateX translateY ``` ```6n+4 6n+5 6n+6``` was used for:

**(6n+4)** 

**Cycle 1: (6 x 0) + 4 = 4** 

**Cycle 2: (6 x 1) + 4 = 10** 

**Cycle 3: (6 x 2) + 4 = 16** 

**Cycle 4: (6 x 3) + 4 = 22** 

**(6n+5)** 

**Cycle 1: (6 x 0) + 5 = 5** 

**Cycle 2: (6 x 1) + 5 = 11** 

**Cycle 3: (6 x 2) + 5 = 17** 

**Cycle 4: (6 x 3) + 5 = 23** 

**(6n+6)** 

**Cycle 1: (6 x 0) + 6 = 6** 

**Cycle 2: (6 x 1) + 6 = 12** 

**Cycle 3: (6 x 2) + 6 = 18** 

**Cycle 4: (6 x 3) + 6 = 24** 

Which pushed the every 4th, 5th and 6th based hexagons to the right in every second row.

Everything was taken and learnt through the courtesy of this site:

https://www.codesmite.com/article/how-to-create-pure-css-hexagonal-grids
