#Getting Started

The HPE Cognitive Computing Toolkit (CCT) is a GPU-accelerated platform for deep learning and other advanced analytics. The CCT-Tutorial contains a number of examples from each of the repositories that comprise the Cognitive Computing Toolkit. This guide can be used to get an introduction to the platform.

## Intro

The CCT platform is software platform for developing-massively parallel applications that execute on multi-core processors such as GPUs. CCT differs from most other parallel programming paradigms (such as MPI, actors, transactional memory) by exposing the parallelism implicitly in the programming model rather than through explicit mechanisms and data structures. The model contains no threads, locks, message queues, critical sections, or races. It is a deterministic, massively-parallel programming model. It is also a declarative dataflow programming model, meaning that a CCT application describes the structure of the computation, not sequential actions.

### Language

CCT is written in the Scala programming language which runs on the Java Virtual Machine (JVM).

### Libraries 

- look at readme for what Ben has put here.

**cct-core** - This is the core library and API. It contains the compiler and runtime system necessary to optimize and distribute a CCT application.

**cct-io** - This library provides a set of objects useful for getting data into and out of a running CCT application using the field initialization, *sensor*, and *actuator* primatives that are part of the core CCT API.

**cct-nn** - This library provides APIs for deep learning and neural networks.

**cct-sandbox** - This library contains unstable CCT libraries for applications including signal processing and computer vision.

**cogdebugger** - This is a UI Wrapper for debugging CCT applicatiosn. Allows developer to visualize the compute graph, viewing the fields, step through the inputs. The debugger is part of the cct-core repository.

## Abstractions

The CCT programming model has three core abstractions: *tensor fields*, *operators*, and *compute graphs*.

brief mention of abstractions - fields, sensors, actuators, operators

## First Example

`BackgroundSubtraction` 
 is a relatively simple example to start with. It can be used to introduced several of the concepts covered in this tutorial.  It can be found [here](https://github.com/hpe-cct/cct-tutorial/blob/master/src/main/scala/tutorial/cogio/BackgroundSubtraction.scala) and under this path in your IDE:
`./cct-tutorial/src/scala/tutorial/cogio/BackgroundSubtraction.scala`

run inside cogdebugger - allows developer to visualize the graph, the fields, and step
wrapped in a compute graph
- input is mp4 file, each image or frame is size is 270x480, 3 bytes per pixel
- ColorMovieAPI from cct-io opens file and creates a sensor for feeding each frame into the compute graph  
- synchronous = false ? (look up what this does)
- vectorField (converts from ColorMovie data type to vectorField - most operations are supporte  
- background - initialized vectorField (same shape as the movie and sample depth (dimmension)
- background <== 0.999f*background + 0.001f*movieVector   
- operations - 2 x multiply by constant, or adds background and movieVector frame)
- <== feedback operator
- convert fromm vecotr field to color field
- caclulate suspicious 
- operations - subtract, absolute value, reduce sum
- intuition
- probe (part of cog debugger)
- run/stop/step/reset
- inspect - graph, fields, values





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

what can we plut here

## Neural Network Toolkit

* in each section point to good examples to look at 



