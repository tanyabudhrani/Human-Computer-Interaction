# human information processing

# the human information process

## input: perception

### visual

- **image**
    - physical reception
    - interpretation: **3D, color**
    - **images** in design
    

- **text**
    - physical reception
    - interpretation: **semantics, pragmatics**
    - **text** in design

### hearing

- **sound**
    - physical reception
    - interpretation: **semantics, pragmatics**
    - **sonification of the interface**

- **speech**
    - physical reception
    - interpretation: **semantics, pragmatics**
    - **spoken word** in design

## throughput: processing

### memory

- **sensory**
    - neuroanatomy

- **short and long term**
    - information in the cell body

### cognitive processing

- **problem solving**

### affective processing

- **affective processing**

## output: response

### motor

- **speed-accuracy trade-off**
    - fitts’ law
    - shannon

- **performance evaluation**
    - index of difficulty
    - index of performence

- **user evaluation**
    - like?
    - dislike?

## structure and inner workings of the brain

- nerve cells are filled with DNA, proteins, and other molecules — about 84% of all genes in our DNA become active in our adult brains
- every type of nerve cell uses a specific range of genes to build the molecular mechanism for its function
    - light receptors in the eyes make proteins that can catch photons
    - nerve cells in the **substantia nigra make dopamine, crucial to our reward system** (cf. affective processing)

## problem solving

| problem solving | strategies, means, and **procedures to achieve a goal** |
| --- | --- |
| problem | how do i get what i want? |
| goal state | the **desired end state** or solution of the problem solving activity  |
| sub goal | **middle-term goal** along the way to solving a problem  |
| problem space | **short, middle, and long term goal states** and the information needed at each step  |

- solving a problem: **X should change so to overlap Y**
    - often, goal satisfaction is incomplete — a good-enough solution

## the problem continuum

- **well-defined problem**: full specification of the provided data, actions, strategies, and goal states, which **can be represented in a problem space**

- **ill-defined problem**: partial or imprecise specification of the provided data, actions, strategies, and goal states, which **cannot be (entirely) represented in a problem space**

### problem solving strategies

| **concept**      | **description**                                                                                     |
|-------------------|-----------------------------------------------------------------------------------------------------|
| **intelligence**  | - rule following <br> - difference reduction <br> - means-end analysis <br> - forward and backward reasoning |
| **creativity**    | - analogy <br> - random trial and error <br> - creative problem solving                              |  

- **difference reduction**: each sub goal that is achieved **brings the current problem state closer to the state goal**

- **means-end analysis**: for each sub goal, **a different procedure decreases the difference between current problem state and goal state** even if this temporarily leads away from the goal state

- **forward and backward reasoning**: recursive inference principles **used to solve well-defined problems, which explicitly have formal limitations**

- **logic reasoning**: only allowed for **known problems** (must have 1 to 1 relationships)
    - e.g if cause, then effect or if effect, then cause

- **analogical reasoning**: looks for **relations between features and categories** that are similar to relations between other features and categories
    - e.g. “the clock signal is the heartbeat of your computer” — relation: pulse
- **case-based reasoning**: a type of analogical reasoning
    
    - **old solution: old problem::adapted solution: new problem**
- **random trial-and-error**: a low level problem solving strategy but commonly found with non-expert users
- **creative problem solving**: give a different function to the standard means that are available to solving the problem

### creativity and deep learning

- DL is a **type of computer program** (AI) from the family of neural networks
- it has 10 to 20 layers of ‘cells’ that process raw data (e.g., one pixel)
    - **cells integrate information from the bottom layers up into the next higher level** and so on until they reach criterion and **place an object in a category based on its features**
- DL is **signal detection** in an advanced configuration

- **bottom layers detect**, for instance, lines

- **second layers search combinations of lines** such as edges

- edges together **make up typical features** for faces, cars, elephants, chairs, etc
- all cells are connected but **connections have different weights**— tweaking weights is done by terabytes of training data

# problem representation

- how you represent a problem affects its solution
    
    
    | surface level | solutions become focused on **color changes, shapes, texture, deformation of solid, etc** |
    | --- | --- |
    | structural level | solutions directed to fixing **loss of structure and managing processes and mechanisms of atoms and ions**  |
    | symbolic level | solutions derived from **logistics, reasoning, and abstraction** |

- how you **represent a problem** to your client, begs its solution
    - each level of aggregating the data **requires its own form of representation**

## structure decisions

- usually relate to **well-defined problems**

## unstructured decisions

- usually relate to **ill-defined problems** and a more vague problem state

### logic rationalist

- sees themselves as a **point in space abstract from the real world**

### associative empiricist

- takes **first person perspective** to go into concretization

## output

### response time

- time taken to respond to stimulus (speed): **reaction time + movement time**
    - movement time is dependent on **physical characteristics of subject**
    - reaction time is **dependent on stimulus type**

### accuracy of response

- another measure of motor skills is **accuracy**
- there is a **trade-off between speed and accuracy**
    - faster is sloppier
    - slower is precise
- whether speed of reaction will result in reduced accuracy **depends on the task and the user**

### fitts’ law: speed vs. accuracy

- a model of human movement
- **derived from shannon’s theory of information systems**
- predicts the time required to **rapidly move from a starting position to a final target area**
- models the act of pointing
- in the real world (e.g. hand or finger, eye tracking)
- on computer (e.g. mouse or joystick)
- task has a certain difficulty (number of bits)
- channel has a certain bandwidth (second/bit)

### index of difficulty

- movement to target **requires more time when distance to target A increases**
- error tolerance of target B decreases— **when target is farther away or of smaller size**

- movement to target requires less time when distance to target A decreases
- **error tolerance of target B increases**— with a closer target or one of larger size


- time $Tpos$ needed to complete the task is linear with respect to ID
    - $Tpos = a + b*ID$
        - a and b are **empirically determined through experimental data**
        - **a = y-intercept**
        - **b = slope(secs/bit)**
        - **Tpos = time taken (second)**
- index of difficulty **depends on the task**, not the device
- **the regression constants a and b determines how fast the task is** (or how fast the device processes the task)
- the **index of performance IP** (or throughput TP) defines how **quickly the task can be finished**
    - $IP = 1/b$

> human information processing is different from computation because **perception, memory, problem solving, and motor responses are less stable but also more adaptive** 

all the visual, textural , sound, and touch input become an **integrated whole and recede in memory**, sometimes in a single cell 

**memory is not fixed but changes over time**, and is context-sensitive

problem solving skills may differ — **for deterministic problems, you need reasoning; for undetermined problems, you need creative solutions** 

when you design a device, you need to reckon with speed-accuracy trade-offs; that is, trained users can be highly efficient, combining high speeds with great accuracy, but it also means that untrained users may not be as advanced

user testing of speed and accuracy tells you how your system or device does in terms of user performance
> 

### example

- when can you consider a problem to be well-defined?
    - **with full specification of the provided data, actions, strategies, and goal states, which can be represented in a problem space**
