[![Build Status](https://travis-ci.org/elyasha/myVelib.svg?branch=develop)](https://travis-ci.org/elyasha/myVelib)

# myVelib-coverage
Final project coverage report of Oriented Object programming at CentraleSupélec

# Documentation
The documentation of this project is available [here](https://elyasha.github.io/myVelib/)

# Coverage report
The coverage report of this project is available [here](https://elyasha.github.io/myVelib-coverage/)


# Pre-requisites
- jdk 11
- [myVelib framework](https://github.com/elyasha/myVelib)

# 1 Overview
A bike sharing system (like, for example, Velib in Paris) allows inhabitants to rent bicycles
and cycle around a metropolitan area. Such a system consists of several interacting parts
including: the renting stations (displaced in key points of a metropolitan area), dierent
kind of bicycles (mechanical and electrically assisted), the users (which may posses a reg-
istration card), the maintenance crew (responsible for collecting/replacing broken down
bicycles), etc.

### Error messages and CLI: 

- [ ] The CLUI must handle all possible types of errors, i.e.
                              syntax errors while typing in a command, and misuse errors, like for example trying to
                              rent a bike from a station which is oine or that has no available bikes.

# 4 Project testing

In order to evaluate your implementations we (the Testers of your project) require you (the
Developers) to equip your projects with both standard Junit tests (for each class) and
a test scenario, described below. Both JUnit tests and the test scenario are mandatory
parts of your project realisations, as we (the Testers) will resort to both of them to test
your implementations.

## 4.1 JUnit tests

Each class in your project must contain JUnit tests for the most significant methods (i.e.
excluded getters and setters).
``Hint``: if you follow a ``Test Driven Development`` approach you will end up naturally having
all JUnit tests for all of your classes.

## 4.2 Test scenario

In order to test your solution you are required to include in the project
- [ ] one initial configuration file (called my velib.ini), automatically loaded at starting
of the system,
- [ ] at least one test-scenario file (called testScenario1.txt).

``Configuration file``: An initial configuration file must ensure that, at startup (after loading this file) the system contains at leas the \standard" setup corresponding to the default
version of the CLI command setup.

``Test-scenario file``: A test-scenario file contains a number of CLUI commands whose
execution allows for reproducing a given test scenario, typically setting up a given config-
uration of the myvelib system (i.e. creation of some velib network, adding of some users,
simulation of some rental/returning of bikes, simulation of planning of a ride, computation
of statistics for the stations and the users, etc.). You may include several test-scenario
files (e.g. testScenario1.txt, testScenario2.txt, ...). For each test-scenario file you
provide us with you MUST include a description of its content (what does it test?) in the
report. We are going to run each test-scenario file through the runtest command of the
CLUI (see CLUI commands above):

````shell
runtest testScenario1.txt
````
