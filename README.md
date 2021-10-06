    Class for complete minimization of logical functions to large number of variables.
   Quick, simple method, providing all solutions in the form of reduced minterms.
   This method has nothing to do with the Quine-McClusKey method.
   Its principle is to reduce each minterm individually so that its coverage does not meet maxterms
   (I have done tests with more than 25 variables).
   The solution includes:
   -the essential reduced minterms
   -The additional reduced minternes for a complete coverage
   -the synthesis where we find all the choices in the reduced minterms for a complete coverage.
   The method is based on an algorithm I’ve been using since 1966 (Brunin Simplification Method).
   In 1970, I built on this algorithm, a relay machine that made it possible to simplify the terms of 5 variables
   (I still have his plans).
   In 1974, a first program in Fortan (about 300 cards) which allowed me to move to terms with 10 variables
   In 1980, a basic program on a PC heatkit H8 with a 16K RAM allowed to simplify always 10 variables.
   Finally, in 2021, I took exactly the same alogithme to make one
 
   In the future... 
   -Option to avoid the expension of the max term to decrease the memory occupation and increase the speed. 
   -Option for very large functions with minterms and Max terms not expanded. In this case we can control the solutions that would produce switching hazards (asynchronous logic) by pre-merging the minternes that would be the cause of these hazards. 
   These options will be introduced when the class is instantiated
