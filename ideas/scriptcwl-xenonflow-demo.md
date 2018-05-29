# Sprint Name 

Script-CWL-Flow

# Team leader

Berend Weel

# Target project 

eStep in both xenon-flow and scriptcwl cases

# Expertise required

Python
Java
Common Workflow Language
Workflow application

# Size of team

4

# Description

To showcase both scriptcwl and xenonflow and what they can do it would be good to have a demo and some documentation
on how to use them in conjunction. This requires some changes in both scriptcwl and xenonflow to make this combination
more smooth.

The idea is to create an ipython notebook that starts with importing the available steps from a xenonflow server.
Showcase the listing and inspection of these steps a little bit.
Then builds a workflow using the available steps.
Submits the resulting CWL workflow to the xenonflow server, which executes it (probably locally).
Finally the results are returned and visualized.

# Goals

 * Adapt the cerise python client so it works well with xenonflow
 * Add a CWL step api to xenonflow
 * Add support for step api to scriptcwl
 * Create an ipython notebook to showcase the use of scriptcwl with xenonflow
 * Add or plan documentation to be written for xenonflow
 * Create a plan for a xenonflow release
