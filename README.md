# Advanced Process Mining Lectures - Assignment 2

> In this assignment, you are going to work as a process mining consultant. In particular, you are going to help a local police department, in analyzing their process, related to their fine management process. Assume that, the system administrator of the local police department has provided you with an event log. Based on this event data, they want you to analyze their fine management process and answer the questions below. 


## Q1. Preliminary Analysis 

The goal is get an overview of the data and gather information to direct and facilitate further analysis.

1.  Create two sublogs:
    - all cases without appeal
    - all cases with an appeal
1.  For the original log, as well as the two sublogs, compute the following statistics:
    - number of traces and trace variants
    - number of events and average trace length
    - covered timespan of the log
    - number of activities
    - Which fraction of traces contains an activity multiple times?
1.  For each activity, compute the following statistics:
    - How frequent is the activity in each log?
    - For which fraction of traces of each log is the activity the first/last activity?
1.  For cases without appeal, create two dotted charts: one showing the activities over time and one showing the activities over case duration. Which patterns can you discover? Discuss and explain your findings.
1.  Consider the statistics computed in question parts 1b) and 1c). Compare the three logs and discuss the results. Which results seem to be desirable? Where can you spot potential problems or open questions?

## Q2. Discovery and Conformance 

Discover models describing the process. Analyze conformance of the log based on your models.

1.  Based on the sublogs created in Q1 a), discover two models:
    - one model describing the process without appeals
    - one model describing the process with appeals
    - Which algorithm/method did you use for discovery and why? How do you position your models in terms of simplicity and generalization?
1.  Compute quality scores for fitness and precision for each sublog and its model.
1.  Describe the behavior of your models (that is, the process they represent).
1.  For both sublogs, find and describe any deviations of the log from that process.
1.  Discuss and explain the results obtained in the previous questions 2a)-d).

## Q3. Attribute Analysis and Compliance 

For this question, focus on the subprocess without appeals. Analyze the information derivable from the attributes. Discover the rules underlying the payment process and check compliance.
1.  Assume, that “Send for credit collection” always results in full payment by the offender.
    1. Which fraction of traces terminates with proper payment (exactly the amount of the fine and all expenses)?
    1. Which fraction of traces terminates with too much payment?
    1. Which fraction of traces terminates with some, but insufficient payment?
    1. Which fraction of traces terminates with no payment at all?
    1. Alltogether, how much money is lost to the police department because of incomplete payment?
1.  The amount of payment requested from the offender increases according to certain rules as the process advances. Based on the data, derive these rules. Describe your findings using textual description as well as a graphical overview.
1.  Discuss and explain the results obtained in the previous questions 3a) and 3b). Which are possible explanations for irregularities in payment? Are there any deviations from the discovered rules? What are possible causes for irregularities and deviations? Which advice would you give to the police department to improve their compliance? You may perform additional computations to improve your understanding.

## Q4. Performance 

Analyze the performance of the process to discover bottlenecks and inefficiencies.

1.  Consider the dotted charts created in ## Q1. Create two similar charts for the process with appeals. Interpret the discovered patterns with respect to time performance of the overall process. You may create additional charts or perform additional computations to achieve higher precision or verify your conjectures.
1.  Analyze time performance based on the process models created in Q2. Present and discuss your results.
1.  Taking into account your findings in 4a) and 4b), which advice would you give to the police department for improving their time performance?

## Q5. Summary and Conclusion 

Summarize your findings. Briefly describe problems and possible solution to the process owner. Which topics would you recommend for further investigation?

