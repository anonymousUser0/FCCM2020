# Grapefruit 

Grapefruit is an automata processing simulator, implemented in python. It supports many essential automata compiling features such as automata minimization, automata transformation, fan in/out constraint, connected components extraction, static and run-time analysis, etc.
Grapefruit uses NetworkX as its underlying data straucture to maintain the automataon as a graph and run automaton processing algorithms to reshape the underlying graph.

Requirements
------------
External dependencies: `g++, swig, python`
OS: Linux, mac OS

1. Clone a fresh copy of the git Grapefruit repository (`git clone -b ASPLOS_AE https://github.com/anonymousUser0/FCCM2020.git`).

2. Download and Install Anaconda (python 2.7)

3. Install the following python packages using all available in Anaconda repositories:

    `sortedcontainers, numpy, matplotlib, pathos, networkx, deap, tqdm, Jinja2, pygraphviz`
    
    `conda install -c conda-forge sortedcontainers matplotlib pathos deap tqdm`
    
    `conda install -c anaconda jinja2 pygraphviz networkx pygraphviz numpy`
    

Install
-------

4. Go to the CPP folder and run the compile script with python include directoy path. For example:

    `./compile ~/anaconda2/include/python2.7/`
    
5. Add Grapefruit to your PYTHONPATH

    `export PYTHONPATH=$PYTHONPATH:/home/foo/Grapefruit`

6. Clone a fresh copy of ANMLZoo

    `git clone https://github.com/gr-rahimi/ANMLZoo.git`

7. Update the variable ANMLZoo's address path in Grapefruit's module `automata/AnmalZoo/anml_zoo.py` variable `_base_address`


Usage
-------
There are some scripts available in the "Example" folder replicating main experiments in the paper. Run each of them using the following command
`python <script name>`



