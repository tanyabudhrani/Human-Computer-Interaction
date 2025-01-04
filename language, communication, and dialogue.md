# language, communication, and dialogue

Created: October 7, 2024 6:37 PM
Tags: LEC

# talking to machines

- the fundamental difference between a computer and an ordinary machine is that a **computer can be approached through language**

## interpretation vs. ahead of time

- (conventional) **interpreter** translates just **one statement of the program at a time**
- **ahead of time compilation** translates the **entire program into machine code at once**
- many modern programming languages blend the two approaches (e.g., Java)
- pros and cons of interpretation (just in time compilation) and (ahead of time) compilation
    1. **cross-platform**
    2. **compiling time**
    3. **execution efficiency**

## compiler architecture

- two phases to compilation:

- **analysis phase**: **breaks source program into pieces** to build up intermediate representation
    - lexical analysis
    - syntax analysis
    - semantic analysis

- **synthesis phase**: **generates target program** from intermediate representation
    - intermediate code generator
    - code optimizer
    - code generator

## line handler

- **low-level routines** that **handle input/output from the source file**
- input line treated as **array of characters**, **uses pointer to next character**
- skips over whitespace, ignores comments, handles continuation lines
- APIs used:
    - `getchar()`: gets next character from input line and **move the pointer**
    - `peekchar()`: gets next character from input line **without moving pointer**
    - `peek2char()`: gets second character from input line **without moving pointer**

## lexical analyzer

- the **source file** is simply a **unique sequence of characters**
- lexical analyzer **scans output from line handler from left to right**
- **converts sequences of characters into “words”, or tokens**
    - **token**: a categorized sequence of characters
        - example token values:
            - **identifiers**: string and symbol table pointer
            - **reserved words**: integer code
            - **numbers**: binary form
            - **operators**: integer code
- **sequence of characters that make up a token** is called a **lexeme**

### example

- program code: `position = initial + rate * 60;`
- result from lexical analyzer:
- symbol/token table
    - data structure used by compiler to **associate tokens with their attributes**
- attributes include:
    - **type of the identifier**
    - **storage allocated for the identifier**
    - **scope of the identifier**
    - **number and types of arguments** (for function identifiers)
- often implemented using a **hash table**

## syntax analyzer

- syntactic analysis is also called **parsing**
- **analyzes groups of related tokens** that form larger constructs such as **statements and expressions**
- converts **linear string of tokens** into **hierarchical structured representation** called a **parse tree**
- checks for **syntactic errors** at this point
- hierarchical structure expressed by **recursive rules called productions**

## semantic analysis

- concerned with the **meaning of the program**
- checks for semantic errors, such as type errors
- **type checking**:
    - checks types of operands (e.g., no real number as array index, % operator requires integer arguments)
- insertion of extra operations such as **type coercion**
    - in view of the surrounding context, **compiler implicitly and automatically changes a value of a certain type** into a value of another type

## intermediate code generation

- intermediate code is **generated as a program for an “abstract machine”**
- needs to be easy to translate into the target program
- uses **three-address code**, similar to assembly:
    - each instruction can be described as a **4-tuple**: ****(operator, operand1, operand2, result)
    - and a **general form**: result = operand1 op operand2
- makes the **operator precedence explicit**
- some statements have to be broken up into multiple statements— **temporary names** must be generated to cover intermediate results

## code optimization

- improves intermediate code so that **final machine code runs faster**; or, can also **optimize for program space** (memory space) rather than run-time speed
- different compilers do this differently; some are more efficient than others
- some easy tricks:
    - **constant** **folding** — perform operations on constants at compile time 2*3.14 → 6.28
    - **reduction in strength**: $x^2$ → x * x
    - **loop unrolling**:
        
        > for (i = 1; i <= 3; i++)
        {x[i] = y[i];} → x[1] = y[1]; x[2] = y[2]; x[3] = y[3];
        > 

### example

- position = initial + rate * 60;
    - temp1 = float(60);
    - temp2 = identifier3 * temp1;
    - temp3 = identifier2 + temp2;
    - identifier1 = temp3;

- optimization
    - temp1 = identifier3 * 60.0;
    - identifier1 = identifier2 + temp1;
    - temp1 = rate times 60
    - position = initial + rate times 60

## code generator

- **generates target code consisting of assembly code**
- does the following:
    - **selects memory locations for each variable**
    - **translates instructions** **into sequence of assembly instructions**
    - **assigns variables and intermediate results to memory registers**

# talking to humans

## dialog design

- **system presents an output observed by the user who performs a task**— **user articulates an input that makes the system perform**
- a **dialog** is a **conversation between two or more parties**, usually cooperative
- in user interfaces
    - refers to the **structure of the interaction**
    - syntactic level of human–computer ‘conversation’

| lexical | shape of icons, **actual keys pressed**, characters |
| --- | --- |
| syntactic | **order of inputs and outputs** (keystrokes, clicks) |
| semantic | **effect on internal application**/data, meaning of keystrokes, clicks |
- dialog notations help us to
    - **analyze systems**
    - separate **lexical from semantic aspects**
    - understand **proposed designs** (i.e. rapid prototyping)

## state transition networks

- **formal descriptions to analyze**
- state transition networks (STNs)
    - **circles**: states
    - **arcs**: actions/events

### hierarchical STN

- really just an **STN inside another STN**
- named **sub-dialogs**
- essential for managing complex dialogs
- several things happen simultaneously
    - example: simple dialog box for text formatting

### design of escapes

- ‘back’ in web, escape/cancel keys
- similar behavior everywhere
- end up with spaghetti of identical behaviors!

### design of help menus

- menu structure nearly the same everywhere, but return to same point in dialog could specify on STN
- but is very messy— usually best added at a ‘meta’ level

### dangerous states

- two-mode word processor:
    - F1: changes mode
    - F2: exit (and save)
    - esc: no mode changes
    - but — esc also resets autosave

- exit with/without save cause dangerous states
- duplicate states with semantic distinction:
    - F1-F2 - exit with save
    - F1-Esc-F2 - exit with no save

## state diagram

- used in UML
- **extension to STN** (hierarchy, concurrent sub-nets, escapes)
- **OFF always active** (history states)
- **link marked H goes back to last state** on re-entering sub-dialog

- behavioral diagram
- nested state machines (history states)
- concurrent states

## flowcharts

- boxes — process/event (not state)
- how can flow charts indicate dialog?
    - **boxes indicate output language**
    - **diamonds indicate input choices**
    - **ellipses indicate states**
    

## jackson structured design

- for **tree-structured dialogs**
- less expressive
- greater clarity
- **hierarchical task analysis meets dialog design**
- notation
    - **o - optional elements**
    - *** - iteration**
- assumed order

## petri nets

- one of the oldest notations in computing
    - **places**: comparable to ‘states’
    - **transitions**: switches to change states (‘arcs’)
    - **counters**: place where user is in state diagram
- several counters are allowed for **concurrent dialog states**
- used for **UI specification**

## textual - grammars

- regular expressions
    - `sel-line click click* dble-click`
- same computational cost as STNs
- grammars: **backus–naur form or backus normal form (BNF)** metasyntax notation for context-free grammars
    
    > expr ::= empty
             | atom expr
             | ‘(‘ expr ‘)’ sentence
    > 
- more powerful than regular expressions or STNs
- still **cannot handle concurrent dialogs**

### production rules

- **unordered list of rules**
    - `if *condition* then *action*`
- condition **based on state or pending events**
- **every rule always potentially active**
- good for concurrency, bad for sequence
    
    > sel-line → first
    C-point first → rest
    C-point rest → rest
    D-point rest → <draw line>
    > 
- **events are added to list of pending events**
- “first” and “rest” are **internally generated events**

### propositional production system

- state based
- **attributes**:
    
    > mouse: { mouse-off, select-line, click-point, double-click}
    line-state: { menu, first, rest }
    > 
- **rules**:
    
    > select-line → mouse-off first
    click-point first → mouse-off rest
    click-point rest → mouse-off rest
    double-click rest → mouse-off menu
    > 
    

### communicating sequential processes

- good for **sequential dialogs**
    
    > bold-toggle = select-bold? → bold-on → select-bold?
    → bold-off → bold-toggle
    italic-toggle = …
    under-toggle = …
    > 
- and **concurrent dialog**
    
    > dialog-box = bold-toggle || italic-toggle || under- toggle
    > 
- but causality unclear

---

## why communicate with a machine in NLP?

- natural language is the **most natural and inclusive interface for human interaction**
- **flexibility** of devices by **adaptation** through (abstract) language instructions ****
- non-experts:
    - can **use complex devices** such as agent systems
    - can **train and teach devices** using natural language
- many social functions rely on **natural language communication**, e.g. business transactions
- **systems can operate autonomously** (after briefing) and report back to you about experiences
- **language is the most efficient way of communication**: abstract, minimalistic, and exploiting common ground

# natural language processing

- a language that is **spoken, written or signed by humans for general communication purposes**
- contrasted with formal languages (programming, mathematical languages) and constructed languages

## semantic analysis

- **marks up text with semantic (meaning) information**, such as proper names, gender, number, cause, effect, etc
- uses **heuristics** combined with **statistics and probabilities**

## syntactic analysis

- **analyzes groups of related tokens (words) that form larger constructs (sentences)**
- converts **linear sentence** into hierarchical structured **parse tree**
    - **parsing is done with grammars**, a formal specification of the structures allowed in a sentence
    - a parsing algorithm is a method for determining the **structure of a sentence with respect to the grammar**
    - a **parser** is a program that **determines the structure of sentences**

## part-of-speech tagging

- part-of-speech tagging is the task of **labeling each word in a sentence with its appropriate part-of-speech tag**
- POS classes **group words into different classes** depending on their syntactic or grammatical behavior

### classes include:

1. nouns (people, animals, concepts and things)
2. verbs (actions)
3. adjectives (properties of nouns)
4. adverbs (properties of verbs)
5. and many other classes, such as pronouns, prepositions, determiners, etc

### probabilistic POS tagging

- a word can have **many tags**
    - e.g., “work” can be a noun, or a verb— usually this is done using probabilities:
    - simple probability: $t_i= argmax_tP(w_i,t)$
        
        > argmax is a mathematical operation, **looking for the argument that yields the highest value** (the max) from a target function— finds the candidate with the **largest expected probability**
        > 
- however, we would like to add in contextual information— given w, what is the most likely t?
    
    ![Screenshot 2024-10-14 at 2.11.49 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.11.49_PM.png)
    
    - now it searches for the highest P, the most likely tag sequence $(T = t_1, ..., t_n)$, given a certain word sequence $(W = w_1, ..., w_n)$
- yet, **ineffective if related words are separated in the text**
- looks back, does not predict context/words about to come

### NLP approach

- generally, NLP models try to **predict what word will follow in a sentence** (**next-token-prediction**)
    - tokenization is identifying words, numbers, operators, etc
- **predicting a missing word** like in the example is called ‘**masked language modeling**’
- the word with the highest probability is not always the best choice— therefore, **some randomness is added** (or ‘temperature’) to be able to vary the wording

![Screenshot 2024-10-14 at 2.14.02 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.14.02_PM.png)

## tokenization

- **converts strings of characters into words**
- **after taking a sample from a dataset, we tokenize and change it into a vector**
- this just means putting numbers to words, which fits computer processing better

# generative pre-trained transformers

- **generative**: it **generates output**
- **pre-trained**: uses **large corpora of text** with **human feedback**

![Screenshot 2024-10-14 at 2.15.38 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.15.38_PM.png)

## transformers

- **transformer**: a neural-network architecture, trying to **connect tokens to one another based on a similarity measure**
    
    ![Screenshot 2024-10-14 at 2.16.09 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.16.09_PM.png)
    

### positional encoding

- positional encoding defines the **location of a token in a sentence** or other sequence and **gives that position a unique value**
    
    ![Screenshot 2024-10-14 at 2.16.46 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.16.46_PM.png)
    
    - now different attention mechanisms can operate on that encoded piece of text

### attention modules

- **regular attention (early approach)**: **connects an input to an output sequence** (A co-occurs with B)
    - the **further away words are, the harder it becomes to link them together**— so proximity is not good to account for semantic association
        
        ![Screenshot 2024-10-14 at 2.17.54 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.17.54_PM.png)
        

- **self-attention (provides some context)**: focuses on a **single sequence / sentence**
    - **links different positions of that single sentence together** and calculates a representation about that sequence— the sentence learns about itself
    - **the system sees a word as a token**; every token has a word embedding, without context
    - to provide context to the word embedding, **weights are added based on similarity**
    

- **single-head attention**: looks at **one aspect of the sentence**, then at another

- **multi-head attention**: each analysis or ‘head’ **runs in parallel, paying attention to different aspects of the sentence**
    - multi-head attention is a parallel process, estimating similarity among tokens that are then concatenated (weighted sum) for the most probable output
    

![Screenshot 2024-10-14 at 2.19.55 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.19.55_PM.png)

![Screenshot 2024-10-14 at 2.20.28 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.20.28_PM.png)

## GELU activation function

- in its transformer network, GPT also uses a special activation function
- the GELU function is an **approximation of the ReLU** (rectified linear unit) activation function
    - **provides computational efficiency** in DL neural networks— at the end of its process (the output layer), **GPT applies the softmax function to simplify the results**

### activation functions in general

- in principle, **a NN is linear (ax + b)**
- **adding an activation function makes the NN non-linear** and that allows the neural network to **learn complex patterns and make predictions**
- non-linearity would better fit most data sets and improve accuracy
- an activation function **calculates the weighted sum while adding bias**
- when predictions are wrong, **backpropagations return the error to the hidden layers** so to **adjust the weights**

![Screenshot 2024-10-14 at 2.23.08 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.23.08_PM.png)

### vanishing gradient problem

- we have **weights connected to words (x)** and the weights tell the next layer of the network **how much the output (y) is affected by that words**
- those weights are also called **gradients**
    - gradients can be adjusted to **minimize error (= maximize model performance)**
- **backpropagation** calculates the **gradients of the error (loss) for each weight**
- **it does that one layer at a time**, going backward from the layer closest to the output (y) to the layer closest to the input (x)

![Screenshot 2024-10-14 at 2.24.13 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.24.13_PM.png)

- **gradients become smaller and smaller with each layer** we go back, and the **weights in the first layers (close to x) are hardly updated anymore**
- activation functions cause the **vanishing gradient**
    - **sigmoid or hyperbolic tangent (tanh)** **compress input into a small range** (sigmoid: 0 to 1; tanh: -1 to 1)— through the layers, gradients become smaller and sometimes disappear

> sigmoid and tanh suffer from vanishing gradients, which are solved by using ReLU or as GPT does by using the GELU activation function
> 
- **logistic regression (sigmoid function) pushes data either in or out of class**

![Screenshot 2024-10-14 at 2.26.26 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.26.26_PM.png)

- thus, **a large data set becomes a small data set with values between 0 and 1** (the ‘derivative of the activation function’)
- therefore, the sigmoid turns big **differences between input values** (e.g., 1 and 100) into small differences (e.g., .1 and .9)
    - this is called **the ‘derivative’ of the activation function** and sigmoid and tanh make the derivative small

### overcoming the vanishing gradient problem

- observe the derivative of the sigmoid: **with bigger amounts of input, x becomes larger, such that the derivative (that what the sigmoid function outputs) approaches 0**
    - ReLU does not render small derivatives

# rectified linear unit

- ReLU: **f(x) = max(0, x)**
- makes **NN non-linear** and **removes negative inputs** (x below 0)
- mainly in hidden layers
    - **softmax in last layer**
- does not activate all neurons at once
- **quick convergence**: if you make a NN larger (a very deep learning system), **computational cost may increase exponentially**— yet, putting in more ReLU algorithms increases computation only linearly (making it faster)
    - therefore, **NN may quickly overfit**

# gaussian error linear unit

- GELU is what GPT uses so **error can be propagated back without vanishing gradients** (weights are updated also in the early layers of the deep network)
- most older activation functions, ReLU included, are not curvi-linear and handle complex data sets less well
- GELU is more stochastic, is more probabilistic, and therefore **can handle complexity better**
- **ReLU gives linear results, GELU produces non-linear results**

![Screenshot 2024-10-14 at 2.30.49 PM.png](language,%20communication,%20and%20dialogue%20118b756f81228075b090e6de3e4f22f4/Screenshot_2024-10-14_at_2.30.49_PM.png)

- activation function to approximate a Gaussian cumulative distribution function (CDF): **differentiable everywhere, enabling efficient gradient-based (= error) optimization**
    - **GELUs more easily approximate complicated functions** than can ReLUs or ELUs— **GELU has a probabilistic interpretation**

## softmax activation function

- the last station before producing an output and is to **simplify the complexity** of all those nodes firing (weights)(features) at it, **providing a probability distribution** which features are most telling to identify the input is a cat and not a chair
    - **maps a vector of logics or real numbers (the input) to a vector of probabilities** $z = [z1, z2, ..., zn$$]$— **each probability ranges between 0 and 1 but such that the total probability sums up to 1**, that way, the softmax function offers a probability distribution

- **exponents** are used to ensure that **all probabilities are positive**

- the denominator with the sum of the exponentiated input **normalizes the probabilities to add up to 1**
- **softmax is a generalization of the logistic function**— softmax gives you probabilities for each class:
    - **decisions for a class are based on the highest probability**; in contrast, sigmoid is binary – two classes only: in or out

## GPT is also pre-trained by humans

- GPT employed **reinforcement learning from human feedback (RLHF)**
    - trainers played the AI as well as the user, **conversations were fed to the network**
    - responses by the network were ranked by the trainers, which served as reward models, influencing the probability distributions towards more humanlike choices
    - today, users can upvote or downvote GPT’s replies and give feedback to **fine-tune results**

# hardware challenges for LLMs

- LLMs cost lots of time and consume lots of energy (not sustainable)
    - **massive data**
    - **GPU utilization (of many GPUs)**
    - **inference**
    - **large systems (computing, communication, storage)**
    - **algorithms may be slow**

- **infrastructure**:
    - storage slow
    - network slow
    - CPU slow
    - limited bandwidth
    - limited GPU memory

- **engineering**:
    - single threaded data load
    - suboptimal decoding
    - suboptimal augmentation
    - synchronous execution of loading and compute
    - lack of data queuing
    - insufficient parallelism

- **algorithms**:
    - too small batch size
    - computationally suboptimal
    network architecture
    - no tensorcore use to speed up processing without losing accuracy

- **error cascading**
    - processing natural language is a multi-step process
    - **errors at one stage lead to more errors further down**

- **ambiguity**

## speech recognition

- converts spoken words to **machine-readable input (text)**
- **identifies the speaker according to acoustic input** (voice verification)
- before, techniques mostly came from electrical engineering and mathematics:
    - digital signal processing
    - probabilities and statistics, modeling
- **measured in word error rate** (number of wrong words/length of sentence)
- problems:
    - **speaker dependence**
    - **acoustic sampling**
    - **environmental noise**

### situated context

- image recognition only gives the **type of object and not the instance**
- identifying object instances is difficult but needed:
    - **count multiple objects** (chairs), **identify object across contexts**, **assign properties to different instances of objects** (my chair is broken), object instances may move, disappear, appear, etc
- extreme solutions:
    1. **all objects of the same type** (e.g., chairs) **are the same instance** (chair)
    2. **every perception of an object results in a new instance** (as many chairs as there are perceptions)
- match places and objects within contexts
- location defines object instances and objects define the location:
    - **objects in known locations mapped to known object instances**
    - **objects in different locations mapped to different instances**
- differentiate objects when they do not match in properties (size, color, position, ownership):

- **permanence**: how much can change to still identify an object?

- **changeability of properties of things**: movable, transferable, size, color

> NLP has problems with interpreting a situation due to **ambiguity of meaning**
> 

# humans interpreting machines

- computers need literal instruction but humans get the gist
- computers need **prescriptive grammar** while humans need **descriptive grammar**