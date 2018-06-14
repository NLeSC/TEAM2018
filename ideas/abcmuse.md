# Sprint Name 

from AMUSE to ABC-MUSE

# Team leader

Inti Pelupessy

# Target project 

Flagship eWatercycle 2/ eStep

# Expertise required

Python

Project organization

Testing/ Documentation

# Size of team

4 or 5

# Description

A long term goal is the split AMUSE in a general framework ("MUSE") and domain specific parts ("ABC"). This goal now becomes urgent
within the eWatercycle project (development of "HyMUSE"). We have an idea of what the base framework should be, it s a matter
of doing some grunt work to get this going. Since no specific expertise is required, and the work can be split up in discrete tasks
I think its ideal for a sprint...

# Goals

to be defined: 
 - what would be the ideal installation procedure, and how do we get there from the current situation (keeping everything functional
 for current users)

Tasks:

These may change on the basis of input from team members, since fresh eyes will probably mean fresh ideas!

- split framework:
  * move framework code to src/muse directory
  * copy back astro code to src/amuse
  * split mixed functionality classes (new framework datastructures vs astro specific)
  * fix corresponding interface imports
- move/ reogranize tests
- replace nostests (deprecated)
- fix examples
- fix documentation
- move or containerize buildbot (test framework) machines and installations
- fix install scripts:
  * join current 3 versions
  * add some safety checksum mechanism
  * make python 2/3 agnostic
  * cleanup prereq
 - python 2 vs 3: both are supported, but work slightly different, make works same way
 - add support mechanism to work with other unit frameworks 
 
 end product is a lean muse framework, base for AMUSE, OMUSE and HyMUSE 
 
