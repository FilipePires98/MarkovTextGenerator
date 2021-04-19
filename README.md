# Markov Text Generator

![](https://img.shields.io/badge/Academical%20Project-Yes-success)
![](https://img.shields.io/badge/Made%20With-C++-blue)
![](https://img.shields.io/badge/License-Free%20To%20Use-green)
![](https://img.shields.io/badge/Maintained-No-red)
 
## Description

The programs implemented in C++ have the purpose of collecting statistical information about texts using Markov (finite-context) models, and of automatically producing texts that follow the models built.

Along with the description of the solution, we also discuss the effects of the variation of the programs' parameters and attempt to compare different types of texts by the amount of information they hold on average.

## Main Programs

 - **fcm:** Parses a list of files to train the model and presents the entropy of the texts on those files.
 
 - **generator:** Parses a list of files to train the model and generates text to a file based on the occurrences statistics of contexts and letters after a context.

## Instructions to Build and Run 

- **fcm**

  Compile: `make fcm`
  
  Run:     `./fcm 3 0.5 input/small_alice_oz.txt`
  
- **generator**

  Compile: `make generator`
  
  Run:     `./generator 4 0.5 "init" 100 outputFile.txt input/small_alice_oz.txt`
  
Both *fcm* and *generator* programs have mandatory arguments. To have information
about them use the `-h` option.

To generate the html documentation run `make docs`.

## Repository Structure

/input      - textual dataset used for model training

/output     - knowledge gathered from the output of the main programs (graphs, entropy values for different parameters, generated texts)

/report     - written report explaining our design choices, presenting results from parameter variation and conclusions of those results

/src        - source code, written in C/C++

## Authors

The authors of this repository are André Pedrosa, Filipe Pires and João Alegria, and the project was developed for the Algorithmic Theory of Information Course of the Master's degree in Informatics Engineering of the University of Aveiro.

For further information, please read our [report](https://github.com/FilipePires98/MarkovTextGenerator/blob/master/report/report.pdf).
