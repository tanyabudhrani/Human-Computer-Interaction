# evaluation techniques

Created: November 4, 2024 1:12 PM
Tags: LEC

![Screenshot 2024-11-04 at 1.17.09 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-04_at_1.17.09_PM.png)

### abstract and obtrusive

- **generalizable**
- high on **precision**
- **focused** data
- **quantitative**
- **structured**

### concrete and unobtrusive

- **single** **cases**
- high on **realism**
- **rich** data
- **qualitative**
- **unstructured**

## research question

- no matter what, **all research starts with a research question** (RQ), which guides you through the whole research process— it is the thing you fall back on when you are stuck or are digressing; **it keeps you on topic**

- **science** = **know why:**
    - **knowledge for its own sake** (don’t ask about usefulness)

- **engineering** = **know how:**
    - **knowledge to make things work** (e.g., a program to understand humans)

## hypothesis

- **derived from the RQ**, a hypothesis is a **precise problem statement** about a topic (e.g., about a physical system, a computer system, human experience)
    - states the **expected statistical relationship between groups of data**
    - the statement has to be **precise and state what we will be measuring**

### null and alternative

- the hypotheses we formulate are commonly about **expected effects**— statements about effects are **statements about differences, about change**
- that means that **there must be at least two sets of data** (else, nothing to compare)
- it also means that there must be **at least two hypotheses**:
    - **H0 - there is no effect**: the null hypothesis (**no detectable differences**)
    - **HA - there is an effect**: the alternative hypothesis (also called **H1**)

- H0 predicts that differences between two sets of data are **statistically not significant**

- HA predicts that differences between two sets of data are **statistically significant**
- the null hypothesis states the **opposite of the expected statistical relationship that the alternative predicts**
- the null is **conservative**, favors current knowledge unless **overwhelming evidence systematically refutes current beliefs**

> if the observed data show that it is **significantly unlikely that there is no effect** (so there is difference into the expected direction), then the **null hypothesis is rejected**, and the alternative hypothesis is accepted
> 

## independent variables or fixed factors

- **the condition under which a task is performed is the independent variable** (e.g., game type, telephone brand, learning with or without VR support)
    - factors that are **systematically varied, manipulated, and controlled by the researcher**
    - determines a **modification to the conditions** that people or physical objects undergo
- may also arise from **demographic data** (e.g., education level, gender, or age)

## dependent variables or measures

- **measurements** (often quantitative)
    - the things that we set out to **measure/observe** (e.g., temperature, time, a rating)
    - **demonstrate the effect of the independent variables** (e.g., fun while gaming)
    - depends upon the independents as well as the **user’s behavior or performance**

- **properties**
    - **readily observable and readily related to some scale of measurement**
    - **stable and reliable** so they do not vary under constant (experimental) conditions
    - sensitive to the **effects of the independent variables**

> a dependent variable is the **variable that changes as a result of the independent variable manipulation**— it’s the outcome you’re interested in measuring, and it **“depends” on your independent variable**
> 

### dependent variable: qualitative

- written web reviews
- camera footage
- sound bites
- observation protocols

### dependent variable: quantitative

- **time**: easy to measure, **suitable for statistical analysis** (e.g. learning time, task completion time)
- **error rate (frequency of errors in a certain part of a system)**: **shows where problems exist within a system**, may indicate cause of difficulties
- **patterns of system use (frequency of use of a certain part of the system)**: study the **patterns of use, preference and avoidance of particular sections**
- **patterns of request for help (frequency of access to on-line help system)**: study what **users find confusing**

> **confusion is the top 1 undesired effect**
> 

## quantifiable performance data in HCI

- situations in which numbers are useful
    - **effectiveness**: successful task completion rate
    - **efficiency**: the trade-off between **speed and accuracy**
        - **time requirements for task completion**
        - compare two systems on **speed or number of errors**
    - **effort**: **difficulty, ease of use** but also **energy consumption**

![Screenshot 2024-11-04 at 1.37.15 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-04_at_1.37.15_PM.png)

| effectiveness | - number of tasks completed
- **percentage of task completion** |
| --- | --- |
| efficiency | - **time to complete specific tasks**
- accuracy (answer to question true or false)
- number of errors
- ratio of **successful interactions to errors**
- number of times user **sidetracked from intended task** |
| effort | - **number of deviations** (extra clicks) from optimal path
- **time spent recovering from errors**
- number of commands/features used
- number of features user can remember after test
- fatigue (physically, cognitively) |
| usability | - **how often help system is used**
- time spent using help
- ease of use |
| satisfaction | ratio of **positive to negative user comments** |

### dependent variables: quantitative, qualitative

- tests may generate **qualitative (i.e. strings) and quantitative data (i.e. integers)**

- **qualitative evaluation**
    - measurements are more **subjective and relative (anecdotal)**
    - gives us cases, data are less structured, more diverse, or ‘rich’

- **quantitative evaluation**
    - measurements are more **precise and less subjective**
    - gives us better **controllable results, usually more structured, more uniform**, but less ‘rich’
    - **more formal data**, allowing for statistical analyses

![Screenshot 2024-11-04 at 1.40.26 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-04_at_1.40.26_PM.png)

### design and engineering

- adding more **structure to data** is **adding more conceptual knowledge**, which is ‘theory’
- whether intuition, tentative knowledge, layman’s theory, common sense, or best practice; **all of that is based on implicit and thus theoretical assumptions**

### scientific research

- theory is always involved:
    - what are data?
    - what are relevant data?
    - sort into which classes?
    - why arranged like that?
    - what do you represent?
    - representation = reality?
    - **stories are biased framings** (security or violation of privacy, different perspectives on the data)
    - what is useful depends on culture and context
    - ‘use’ depends on goals you have or not (e.g., is spyware useful? I have no use for it)

## measures

| nominal  | **attributes are named**, weakest form of measurement | • categories, classes, labels, tags, names
• **classifies data points into named or numbered but unordered categories** (e.g., user groups, gender, religion, education, region)
• **allowable manipulations**: **number of data points in a category**
• **statistics**: number of cases in each category, **most frequent category** |
| --- | --- | --- |
| ordinal | **distances between steps bear no meaning** | • classifies data points into ordered categories, **but differences between each category are unknown**
    ◦ **ordered but unequal steps**
    ◦ distances between steps bear no meaning
• **allowable manipulations**: counting number of data points in a given category, **merging adjacent classes** (e.g., number of users who are satisfied with your design)
• **statistics**: **median, mode, percentiles** (30% of users were satisfied) |
| interval | **distances are meaningful** | • similar to ratio scale, **but the “zero” point is arbitrary**
• ordered but with **equal steps** (distances are meaningful)
• **allowable manipulations**: **add, subtract**
    ◦ sometimes, ratios (multiply, divide) may not be meaningful
• **allowable statistics**: **mean, range, variance, standard deviation** |
| ratio | **absolute 0**, strongest measurement | • **absolute non-arbitrary zero**, strongest measurement
• classifies data points into ordered categories
• **equal differences between categories / steps**
• **allowable manipulations**: **add, subtract, multiply, divide**
• **allowable statistics**: **mean, range, variance, standard deviation** |

> **variance**: how much **each score is different from the mean** and thus **from every other value in the data set**
> 
> 
> 
> **standard deviation**: tells the **distribution of a set of data points in relation to the mean value**, expressed as ‘the square root of the variance’
> 

### qualification of qualitative data

- use of coding schemes and calculating **inter-rater reliabilities**
- calculate inter-rater reliabilities
    - **percentage agreement** (but no control of coincidental agreement)
    - **cohen’s kappa**
    - **krippendorff’s alpha**
- when reliably consistent, **collect raters’ scores on the actual data** (not the test set)
- apply appropriate statistics
    - calculate averages
    - correlations
    - regression (multiple)
    - t-tests for comparing means (e.g., user experience with MacOS or PC)
    - analysis of variance, etc

## measures and issues

- **unnecessary downgrading of measurement quality**
    - **high resolution can be degraded to low resolution with certainty**
    - **low resolution can never be upgraded to higher resolution with certainty**
    - **missing data**, data you did not measure, can be estimated, **they cannot be known**
- classifiers in neural networks **may reduce measurement quality**
    - **classifiers split a data set in two or more groups**
    - by splitting, **intermediate values are lost**

# usability testing

- all formal/informal types of tests can be used in a **formative or summative manner**
    - **formative** means ‘**during design**’— **information helps shape the next iteration**
    - **summative** means ‘**after design**’— **information is for final evaluation** after rollout

| observations | **heuristic testing** > **experts test rules of thumb**

**cognitive walkthrough** > **expert acts as typical user**

**thought listing** > **concurrent, retrospective, constructive** |
| --- | --- |
| focus groups | moderator-guided discussion |
| interviews | unstructured
structured (semi) |
| lab experiments | work if **there is a specific thing that we want to assess** (e.g., testing a hypothesis), answering specific questions about targeted parts of a theory or system |

## heuristic testing

- evaluators, often experts, **examine the interface and judge its compliance with recognized usability principles**
- **experts score a number of variables according to design guidelines**, for example:
    - understandable language, dialogs
    - suited for target group
    - consistency
    - clear manual and help function

| pros | cons |
| --- | --- |
| evaluators can focus **directly on specific issues**: good, bad points | evaluators can **mark “issues” that aren’t actually usability problems** |
| evaluators can **pinpoint faults with individual elements early on** and determine their impact on overall usability | you have to choose exactly the right heuristics to make sure evaluations find all usability issues— definition issues: **what is understandable language?** |
| compared with lab experiment, **you can get feedback without the ethical and practical dimensions and costs** – relatively cheap and fast | number and quality of experts: **it can be hard to find evaluators who are experts in a certain industry** (e.g., banking) as well as usability |
| you can **combine it with lab experiment** | **little structure**: as you **need** **several expert evaluators** anyway, you may yet want to do lab experiments |
| with the right heuristics, **evaluators can help flag detailed issues** and lead the way to optimal solutions | **it’s subjective**: **findings can lack proof and be biased**, and solutions don’t arise automatically |

### cognitive walkthrough

- evaluators are experts and **work through a series of tasks and ask a set of questions from the perspective of the user**
- expert pretends to be a typical user, solving a specific task— **offers first interaction description with overview of issues**

| pros | cons |
| --- | --- |
| **more structured** | finds **task-related issues only** |
| **provides answers** to specific questions | **time consuming** |
|  | task description is not easy |
|  | quality of expert (to simulate a user) |

### thought listing

- potential users (**non-experts**) **perform a task and speak their minds**
- analysis protocol by expert, identifying issues
- three types of thought listing:
    1. **concurrent thought listing**: **one user at a time**, verbalizing **while using the application**
    2. **retrospective thought listing**: **one user at a time**, verbalizing thoughts **after use**
    3. **constructive interaction**: **two users at the same time**, **conversing** about the application
        
        > constructive interaction - **provides the most natural thinking-aloud as test subjects collaborate in pairs to solve tasks**
        > 
- constructive interaction
    - how to conduct constructive interaction (i.e. thinking-aloud protocol)?
    - design a set of tasks (like cognitive walkthrough)
    - participants are asked to say whatever comes to mind as they complete the task
        - what they are looking at
        - what they are thinking about
        - what they are going to do
    - **record and observe** (without attempting to interpret their actions and words)
    - **sessions are often audio- and video-recorded** so that developers can go back and refer to what participants did and how they reacted

| pros | cons |
| --- | --- |
| **real users**, rich data | **selection of users**, choice of task |
| **good insights** into problems | **time consuming** |
|  | are all thoughts verbalized |

### focus groups

- complements **constructive interaction**
- **small groups, predefined demographic traits** (e.g., older adults, caretakers)
- **moderated, questions directed at particular topic** (e.g., ethical use, societal impact)

### interviews

- **oriented at the individual**, complement of focus groups
    
    
    | unstructured | **open format**, like a normal conversation, **no questions prepared**, but topic defined
    
    good for **sensitive topics** (e.g., robots against loneliness and depression) |
    | --- | --- |
    | semi-structured | has an **interview protocol, guided conversation**, has **structure as well as options built in** to go into specific details, aspects, issues that were unforeseen |
    | structured | almost like a **questionnaire but face-to-face**
    
    **strict interview protocol**
    
    may be felt as rigid but is **good if specific questions / hypotheses should be investigated**
    
    no options to **explore unforeseen topics** |

### lab and field experiments

- an experiment is designed to **test a hypothesis about the role of one variable** (the independent variable) **on another** (the dependent variable)
- works if **there is a specific thing that we want to assess**, answering specific questions about targeted parts of a theory or system
    - does my new approach lead to faster completion of tasks?
    - is a text interface easier to remember than a GUI?
- for example, to test the validity of fitts’ law: relates the distance to the target, the size of the target and the pointing system to the time it takes to point to the target
    - the distance and size of the target are known
    - users perform a series of pointing tasks (trials) with different distances and sizes
    - different pointing systems are timed (sec) and measured for accuracy (hits vs misses)

as said, any formal or informal test type can be **used for formative or summative testing of your application**

## formative

- formative (during system development, **usually based on a prototype**)
    - **understandability** of application
    - **completeness** of application
    - **quality** of the application
    - **ethical** review
    - **liability** and law
    

## summative

- **process evaluation**
    - is the application well implemented? - **code review**
    - user statistics - **click behavior**, website traffic, peaks
    - **accessibility of website / contact info**
    - safety, security
- **impact evaluation** (effect on users, other stakeholders)
    - **environmental and behavioral factors** (cf. physical and cognitive ergonomics)
    - **final effect of the app on someone’s** **financial situation, health, work performance**

---

# laboratory experiments

- definition of an experiment:
    - an experiment is designed to **test a hypothesis about the role of one variable (the independent variable) on another (the dependent variable)**
- in confirmatory data analysis, or statistical hypothesis testing, we have:
    - **a hypothesis that we wish to “confirm” or “reject”**
    - **two sets of measurements of the dependent variable**, each corresponding to **one configuration of the independent variables**
    - a process that **we will repeat with multiple subjects**
    - a **statistical method** that we will use to **compare multiple sets of data**

## experimental design

- **between-subjects**
    - **split participants** into two or more groups
    - **each group receives a different treatment**/works under a different condition
    - makes it easier to **keep manipulations ‘clean’** (fewer order effects)
    - **variance is larger** (different people, not just different conditions)

- **within-subjects**
    - **all participants receive all treatments** / work under all condition
    - good when it is **hard to recruit enough participants**
    - **inevitable if you measure more dimensions** (e.g., feeling happy or sad; level of usability and user satisfaction)
    - **variance is better comparable** (same people under different conditions)

- **mixed designs**
    - **between-subjects for the independent variable**
    - **within-subjects for dependent measures**: feeling involved, feeling distant
    

### between subjects

- participants (users) **split into two or more groups**
    - make sure the groups are **demographically similar**
    - **have equal amounts of training, experience**, etc

### within subjects

- same participants in all conditions: **all participants perform the same task**

### things to watch out for in experiment design

- the experimenter must systematically **manipulate one or more independent variables in the domain** under investigation
- the manipulation must be made under **controlled conditions**, such that **all variables that could affect the outcome of the experiment are controlled**
    - **demographics**: male – female balanced, similar age, education, cultural background
    - **experience**: novice – expert
    - **habits**: how much sleep, stress levels, how much coffee

## confounds

- happen when variables that were **thought to be independent actually vary according to some other factor in the experiment** (e.g., attitude, profession, or a novelty effect)
    
    
    | experience factors | people have **more/less relevant experience with one condition than the other**
    
    **people in one group have more/less experience than the other group**— usually happens when group division is not done properly in between-subject tests |
    | --- | --- |
    | experimenter/subject bias | **experimenter subconsciously treats subjects differently, or when subjects have different motivation levels**  |
    | uncontrolled factors | **time of day, system load**, but most notoriously: **convenience sampling online** |

## order effects

- a particular type of confounding, which involves the **order in which the experiment tasks are carried out**

### within subjects

- tasks that are done **earlier are slower and more prone to error**; tasks that are done **later are more prone to fatigue and boredom**
- **warming-up effects**: ****first condition trains for the second
- **payment terminals**: fixed layout vs shuffling input numbers for security reasons
- task demands on the user:
    - **cannot rely on routine** (= automated motor output)
    - has to **pay more attention selecting proper keys**
    - **more effort** goes into **memory retrieval**

### preventing confounding and order effects through randomization

- control the effects of independent variable X on dependent variable Y so that **effects are distributed randomly among conditions (groups)**
- **randomly assign people to different groups** (this addresses the **experience effect**, best would be equal distributions)
- all of this **does not remove effects due to unknown differences**, but ensures that any effect due to unknown differences among participants or conditions is **random** (and will be **tackled through statistics**)

![Screenshot 2024-11-09 at 10.40.21 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_10.40.21_PM.png)

### preventing confounding and order effects through counter-balancing

- **counter-balancing**: mitigates **order effects in within-subject experiments**
    - **independent variables are varied across subjects in different order**
    - if there is an order effect, **this distributes the effect across all groups**, but does not remove them
- this will fail, however, **if order effects are not equal between conditions**— therefore, four between-subjects groups with one within factor each: order

# statistical analysis

- calculations that tell us mathematical attributes about our data sets
- how data sets relate to one another
- **the probability that our claims are correct**

## exploratory and confirmatory

- **exploratory data analysis** enables you to **find out potential patterns from collected data**
- **confirmatory data analysis** allows you to **validate whether the collected pattern really holds** (normally)
- without any pattern discovered, **there is nothing for validation**
- nevertheless, **validation result can provide feedback for further exploratory study**

### exploratory data analysis

- **inductive approach**, “**descriptive statistics**”
- analyses data sets to **summarize main characteristics**, **looking for patterns**
- often uses **visual methods to aid analysis**
    - visualization-driven discovery of co-occurrences in gene-expression
    - red is high positive correlation, interpreted as higher similarity in gene expression
- good to come up with **hypotheses that then later can be / should be tested**
- **to find the relation between similarity and liking, plot the data points**
    - **do curve fitting, using SPSS**: analyze > regression > curve estimation
    - **excel**: X-Y scatter plot, right click curve, add trend line, polynomial, order 2 then, options > display equation on chart
    
    ![Screenshot 2024-11-09 at 10.45.35 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_10.45.35_PM.png)
    

### confirmatory data analysis

- **deductive approach — inferential statistics**
- looks for **definite answers** to specific questions
- often uses **probability models and numerical calculations**
- given a hypothesis determined at the outset, **do the data support our hypothesis**

- **confirmatory data analysis** uses **descriptives to summarize and describe a group of numbers** from a research study, but that’s just the start

- **inferential statistics** are used to **draw conclusions and to make inferences that go beyond the individual cases**
- allows researchers to **make inferences about a large group of individuals** (i.e. population) based on a research study **in which a much smaller number of individuals (i.e., sample) took part**
- **testing the H0 → can ‘no notable difference’ be refuted?**
    - statistically, we can never demonstrate that anything is ‘correct’ or ‘true,’ **only that it is very likely to be correct**: “most swans are white”
    - statistics can also underscore that **something is very likely to be false**, finding a number of swans that are not white
    - **the stronger the statement, the less sophisticated statistics needed**: “all cats are white” and “Anything white is a cat” are easily falsified by finding one counter-example
- the null is conservative and **only rejected if it is significantly unlikely that no-difference** / no-effect occurred

## central tendencies

- central tendencies of group of scores (distribution) refers to the **middle of the group of scores**
- **mean**, written as M, µ, or X(X-bar)
    - X stands for the **scores in the distribution of the variable X**
    - N or n stands for the **number of scores in a distribution**
    
    ![Screenshot 2024-11-09 at 10.53.12 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_10.53.12_PM.png)
    

- **mode**
    - the mode is the **most common single value** in a distribution

- **median**
    - if you line up all the scores from lowest to highest, **the middle score is the median**
    - if there are two middle scores, the median is the average of the two

### visual inspection of central tendencies is not reliable

- given any set of collected data, **there will almost always be some variation**
    - differences between data sets may be due to **just normal variation**
    - two sets of ten tosses with different but fair dice
        1. first dice gives 6, 2, 4, 4, 2, 6, 4, 2, 5, 6 (M = 4.1)
        2. second dice gives 6, 4, 4, 5, 4, 4, 2, 1, 4, 5 (M = 3.9)
- if they are both fair dice, shouldn’t their outputs have the same probability? does this mean that the dice are not fair? given any set of data (even dice throws), **there will always be some variation**
- the question is **whether this variation is explainable by normal variation**

## variance

- how spread out are the scores in a distribution?
    - X stands for the scores in the distribution of the variable X
    - M, µ, or X is the mean
    - N or n stands for the number of scores in a distribution
- standard deviation (σ, S, or SD)
    - the square root of variance
    
    ![Screenshot 2024-11-09 at 10.56.10 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_10.56.10_PM.png)
    

![Screenshot 2024-11-09 at 10.56.54 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_10.56.54_PM.png)

## mean and variance

- there are two separate issues here: **the mean, or the average, and the variability, or the standard deviation**
    
    ![Screenshot 2024-11-09 at 10.57.20 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_10.57.20_PM.png)
    
- the difference between the means of the two curves is the same in all three above situations— however, they certainly do not look alike

## signal versus noise

- given two datasets, **the difference between their means is the “signal”**
    - the change that we think that we introduced into the dataset by **manipulating the independent variables**

- **the** **variability is the “noise” that is introduced by random factors beyond our control**
    - given any dataset, there will always be some “noise,” **so we cannot trust that the “signal” tells the story 100%**
- the question is: **how much noise can we expect to encounter in a normal situation?**
    - meaning: **when can we trust that the difference that we’re seeing is a reliable difference, and not just because of noise?**

### signal = mean, noise = variance

- intuitively, we can trust that the difference we are seeing really is a difference **when we have more observations in our sample**

## t-test

- the t-test was originally used by gosset to compare differences in barley yields (for a beer brewery)
    - the idea is to **calculate the signal (mean difference) to noise (variability) ratio**
- a large part of western-based science is indebted to the t-test and related techniques such as (M)ANOVA

### t-test: independent samples

- a statistical test that **compares the difference between the means of two groups of data**, **taking the variability of the two groups into account**
- calculates a t-value which gives us the signal-noise ratio
- **if this ratio is high enough** (we have enough “signal” to compensate for the “noise”), then we can **be more confident that the signal is trustworthy**

![Screenshot 2024-11-09 at 11.02.48 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_11.02.48_PM.png)

### different types

- **independent samples t-test** (a.k.a., two-samples t-test)
    - compares the difference between the means of two groups of data, **taking the variability of the two groups into account**
- **one-sample t-test**
    - **tests the mean of a single group against a known value**
- **paired samples t-test**
    - **compares means from the same group at different times** (e.g., before-after treatment) **or different conditions in a within-subjects experiment** (e.g., working with an avatar vs a robot, order effects, or measuring happy versus sad)

### t-test: one sample

- tests the **mean of a single group** against a **known value**
    
    ![Screenshot 2024-11-09 at 11.04.40 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_11.04.40_PM.png)
    

### t-test: paired samples

- paired-samples t-test **compares means from the same group at different times** (e.g., one year apart) or different within-experiment conditions
- interestingly, **paired samples t-test and one sample t-test are mathematically equivalent**
    - **known mean is 0**
    - **single group is now the group of the differences**

![Screenshot 2024-11-09 at 11.05.24 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_11.05.24_PM.png)

## role of the normal distribution

- the normal distribution allows the t-test to say something **about how likely it is that the differences between the means of the two groups are systematic, or just happened by matter of chance**
    - **default is the null (H0) = observed differences are chance occurrences**
    - given enough data, or a small enough variability, we can reject the null in favor of the alternative (HA or H1) if:
- **if the t-test shows that the difference between the means (the signal) is more than what would be expected purely by chance**
    - **then we say that the difference is statistically significant**
    - certain researchers would then reject H0 and accept H1

## significance

- if the t-test shows that the difference between the means (the signal) is more than what would be expected purely by chance, then we say that the difference is statistically significant— how does the t-test “show” us this with a value?
    - **the numerator of the t-value is the difference between the means of the groups**
    - **the denominator is the variability of the groups**
- intuitively, **the larger the t-value is, the more significant the difference** (or the signal) is, compared to the noise
    - significance depends on the **size of the dataset (the degrees of freedom)**
    - and on the **risk level** (or alpha level or rejection area) that we set: a = .05
        - gives the level of confidence we want to have before making a judgement
        - usually set at 95% (or a 5% chance that we might be wrong): p < .05
        - but that is **pretty arbitrary and depends on the situation**
- **degrees of freedom are the maximum number of values that you can freely vary in a data sample while keeping the same mean**
    
    ![Screenshot 2024-11-09 at 11.08.54 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_11.08.54_PM.png)
    
    > N = 200
    male, n1 = 98
    female, n2 = 102
    independent samples t-test: df = n1 + n2 − 2
    > 
    > 
    > effect of males versus females, t(df) = t(198) = 5.49 
    > 
- put more formally, if you know X with the sample size n and if you know the scores X1, X2, ..., Xn – 1, then you can calculate the value of Xn
    
    ![Screenshot 2024-11-09 at 11.10.38 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_11.10.38_PM.png)
    
- level of significance, then, **is the t-statistics in relation to the degrees of freedom**
    - **more degrees of freedom and the t-value can be lower to establish a significant effect**
    - fewer degrees of freedom and the t-value has to be very high to establish a significant effect

## probability

- SPSS, R, or excel (and other spreadsheets and statistical packages) **calculate the probability = p-value for us**
- the p-value gives us the **confidence that the null hypothesis is valid**
    - for instance, a p-value of 0.30 means that we are **30% sure that there is no significant difference between the two datasets**
- therefore, **we reject the null hypothesis if the p-value is less than or equal to our required significance value**— i.e. the amount of error that we're willing to tolerate under the level of confidence that we require
    - for instance, if we are using a significance value of 0.05 (or we want a confidence of 95%), we reject the null hypothesis if the p-value is 0.05 or less

![Screenshot 2024-11-09 at 11.14.45 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_11.14.45_PM.png)

### some limitations

- **data points of each sample are normally distributed**
    - not always the case, **but t-test very robust in practice, due to central limit theorem** (CLT)
- population variances assumed equal
    - t-test reasonably robust for differing variance, however, does deserve consideration, **may use F-test to validate** (ANOVA / MANOVA)
- **individual observations of data points in sample should be independent**
- significance level
    - **decide upon the level before you do the test**
    - **typically stated at the .05 or .01 level**

> **CLT**: **a sample** **approximates normal distribution as the sample size gets larger** (i.e. aim for n ≥ 50 in each between-Ss condition to avoid trouble)
> 

## false alarms and missed signals

- the t-test gives us the probability that the difference that we’re seeing between the data sets is not due to pure chance
- there are two types of mistakes we might make
    - **type 1 error: null hypothesis is true, but we reject it by mistake (false alarm)**
    - **type 2 error: null hypothesis is false, but we accept it by mistake (missed signal)**
- effects of the level of significance
    - if we set our **confidence level too high** (e.g., p < 0.0001), **we run a greater chance of Type 2 errors**
    - if we set our **confidence level too low** (e.g., p > 0.1), **then we run a greater chance of Type 1 errors**

![Screenshot 2024-11-09 at 11.17.13 PM.png](evaluation%20techniques%20134b756f8122803090f3d2a9da5d5386/Screenshot_2024-11-09_at_11.17.13_PM.png)

- in most scientific studies, type 1 errors are generally considered to be worse because the hypothesis is the current state-of-the-art theory— therefore, **people expect a high confidence level if you’re going to overturn it**
    - for example, if it’s “presumed innocent till proven guilty,” you need an overwhelming vote in a jury to convict a serious crime