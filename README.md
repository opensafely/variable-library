# Variable Library

## What is a variable?
Variables are a complex entity in that they combine Python code used in the `study_definition.py`, 
creation of the codelist on [OpenCodelists](codelists.opensafely.org) and Python code to import
codelists into the study defintion, usually in a file called `codelists.py`. 

## Problem 
Many OpenSAFELY studies contain the same variables that are implemented within the study 
definition. Currently these are either manually written, with guidance from the 
[documentation](docs.opensafely.org) or more commonly copied and pasted across 
from other studies, and dates changed. When the `cohortextractor` API endpoints have changed
or updated, this can mean that sometimes variables are written in an out of date way. 

## Aim of variable library
A variable library would aim to address the above problem by having one place for
variables to be taken off the shelf from, and pasted into research projects. In the future,
we would aim for this to have an interactive GUI or user interface with 
dropdown menus, and the ability to save and tweak. For now, this repo is a MVP of what the implementation of a Variable Library would look like. 
It contains [issues](https://github.com/opensafely/long-covid/issues) for different 
variable options with codeblocks for easy copy and pasting across to your study definition. 
These have documentation and will act as an easily explainable _library_ of variables. 

We will iterate and roadtest the components of this library before implementing a more complicated
project with user interface.
Please see the [discussion](https://github.com/opensafely-core/roadmap/discussions/5)
for what this project may iterate into. 

## How to Contribute
Researchers can contribute in two ways:
1) Put useful variables into an in issue on this repo with good documentation. At a 
minimum, an issue should contain code for the `study_definition.py`, code for the 
   `codelists.py` and the relevant codelist link (usually as a `codelists.txt`). It will be easier 
   copy and paste if this is put into code blocks which format it correctly. 
   
2. Add your thoughts to the [Roadmap](https://github.com/opensafely-core/roadmap/discussions/5)
and help shape what the Variable Library will look like in the future. 
