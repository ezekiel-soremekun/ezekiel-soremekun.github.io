---
title: "Directed Grammar-Based Test Generation"
collection: talks
type: "Conference Talk"
permalink: /talks/2026-07-07-FSE26-Montreal
venue: "FSE 2026,Conference Venue: Concordia SGW Campus @Downtown Montreal"
date: 2026-07-07
location: "Montreal, Canada"
---

[More information here](https://conf.researchr.org/profile/icse-2023/ezekielsoremekun#)

[Website](https://debugging-assumptions.github.io/)

**Abstract:** To effectively test complex software, it is important to generate goal-specific inputs, i.e., inputs that achieve a specific testing goal. For instance, developers may intend to target one or more testing goal(s) during testing ? generate complex inputs or trigger new or error-prone behaviors. However, most state-of-the-art test generators are not designed to target specific goals. Notably, grammar-based test generators, which (randomly) produce syntactically valid inputs via an input specification (i.e., grammar) have a low probability of achieving an arbitrary testing goal. This work addresses this challenge by proposing an automated test generation approach (called FdLoop) which iteratively learns relevant input properties from existing inputs to drive the generation of goal-specific inputs. The main idea of our approach is to leverage test feedback to generate goal-specific inputs via a combination of evolutionary testing and grammar learning. FdLoop automatically learns a mapping between input structures and a specific testing goal, such mappings allow to generate inputs that target the goal-at-hand. Given a testing goal, FdLoop iteratively selects, evolves and learn the input distribution of goal-specific test inputs via test feedback and a probabilistic grammar. We concretize FdLoop for four testing goals, namely unique code coverage, input-to-code complexity, program failures (exceptions) and long execution time. We evaluate FdLoop using three (3) well-known input formats (JSON, CSS and JavaScript) and 20 open-source software. In most (86\%) settings, FdLoop outperforms all five tested baselines namely the baseline grammar-based test generators (random, probabilistic and inverse-probabilistic methods), EvoGFuzz and DynaMOSA. FdLoop is (up to) twice (2X) as effective as the best baseline (EvoGFuzz) in inducing erroneous behaviors. In addition, we show that the main components of FdLoop (i.e., input mutator, grammar mutator and test feedbacks) contribute positively to its effectiveness. We also observed that FdLoop is effective across varying parameter settings ? the number of initial seed inputs, the number of generated inputs, the number of input generations and varying random seed values. Finally, our evaluation demonstrates that FdLoop effectively achieves single testing goals and scales to multiple testing goals.