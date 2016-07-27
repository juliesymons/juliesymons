#Getting Started

The HPE Cognitive Computing Toolkit (CCT) is a GPU-accelerated platform for deep learning and other advanced analytics. The CCT-Tutorial contains a number of examples from each of the repositories that comprise the Cognitive Computing Toolkit. This guide can be used to get an introduction to the platform.

## Intro

The CCT platform is software platform for developing-massively parallel applications that execute on multi-core processors such as GPUs. CCT differs from most other parallel programming paradigms (such as MPI, actors, transactional memory) by exposing the parallelism implicitly in the programming model rather than through explicit mechanisms and data structures. The model contains no threads, locks, message queues, critical sections, or races. It is a deterministic, massively-parallel programming model. It is also a declarative dataflow programming model, meaning that a CCT application describes the structure of the computation, not sequential actions.

### Language

CCT is written in the Scala programming language which runs on the Java Virtual Machine (JVM).

### Libraries

1.  CCT-Core - This is the core library and API. It contains the compiler and runtime system necessary to optimize and distribute a CCT application.
2.  CCT-IO - This library provides a set of objects useful for getting data into and out of a running CCT application using the field initialization, *sensor*, and *actuator* primatives that are part of the core CCT API.
3.  CCT-NN - 
4.  CCT-Sandbox

## Abstractions

brief mention of abstractions - fields, sensors, actuators, operators

## First Example

- add pointer to first one in tutorial to look at

- add some explanation

## Fields

what are the different types of fields

which tutorial examples are relevant here 

## Sensors

random, file sensor, user defined sensors

which tutorial examples are relevant here 


## Actuators

what can we say about actuators

which tutorial examples are relevant here 

## Operators

- built-in
- feedback operator
- user-defined GPU operators
- user-defined CPU operators

## The Debugger

go over its functionality

## Programming CCT Applications



