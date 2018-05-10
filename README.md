# Analysis of single-cell RNA-seq data: Normalization, dimensionality reduction, clustering, and lineage inference

# Instructor(s) name(s) and contact information
Diya Das (@diyadas, diyadas@berkeley.edu), Davide Risso (@drisso), and Kelly Street (@kstreet13)

# Workshop Description

This workshop will be presented as a lab session (brief introduction followed by hands-on coding)
that instructs participants in a Bioconductor workflow for the analysis of single-cell RNA-sequencing data, in three parts:
1. dimensionality reduction that accounts for zero inflation and over-dispersion common in single-cell RNA-seq and allows for the incorporation of sample- and gene-level covariates
2. cell clustering that employs a resampling-based approach resulting in robust and stable clusters
3. lineage trajectory analysis that uncovers developmental processes and is flexible to the input

We will provide worked examples for lab sessions, and a set of stand-alone notes in this repository.

Note to organizers: A previous version of this workshop was well-attended at BioC 2017,
but the tools presented have been significantly updated for
interoperability, and we have been receiving many requests to provide an
updated workflow. We plan to incorporate feedback from this workshop into a published document.

## Pre-requisites

We expect basic knowledge of R syntax. Some familiarity with S4 objects may be helpful, but not required.
More importantly, participants should be familiar with the concept and design of single-cell RNA-sequencing experiments.

## Workshop Participation

Participants should bring a laptop on which they have administrative permissions, and have installed the Bioconductor packages listed below.

## _R_ / _Bioconductor_ packages used

1. _zinbwave_ : https://bioconductor.org/packages/release/bioc/html/zinbwave.html
2. _clusterExperiment_: https://bioconductor.org/packages/release/bioc/html/clusterExperiment.html
3. _slingshot_: https://github.com/kstreet13/slingshot (will be submitted to Bioconductor shortly)

## Time outline

2 hr workshop:

| Activity                                   | Time |
|--------------------------------------------|------|
| Intro to packages                          | 15m  |
| zinbwave (dimensionality reduction)        | 30m  |
| clusterExperiment (clustering)             | 30m  |
| slingshot (lineage trajectory analysis)    | 30m  |
| Questions / extensions                     | 15m  |

# Workshop goals and objectives

List "big picture" student-centered workshop goals and learning
objectives. Learning goals and objectives are related, but not the
same thing. These goals and objectives will help some people to decide
whether to attend the conference for training purposes, so please make
these as precise and accurate as possible.

*Learning goals* are high-level descriptions of what
participants will learn and be able to do after the workshop is
over. *Learning objectives*, on the other hand, describe in very
specific and measurable terms specific skills or knowledge
attained. The [Bloom's Taxonomy](#bloom) may be a useful framework
for defining and describing your goals and objectives, although there
are others.

## Learning goals

Some examples:

* describe how to...
* identify methods for...
* understand the difference between...

## Learning objectives

* analyze xyz data to produce...
* create xyz plots
* evaluate xyz data for artifacts

### A note about learning goals and objectives (#bloom)

While not a new or modern system for thinking about learning,
[Bloom's taxonomy][1] is one useful framework for understanding the
cognitive processes involved in learning. From lowest to highest
cognitive requirements:

1. Knowledge: Learners must be able to recall or remember the
   information.
2. Comprehension: Learners must be able to understand the information.
3. Application: Learners must be able to use the information they have
   learned at the same or different contexts.
4. Analysis: Learners must be able to analyze the information, by
   identifying its different components.
5. Synthesis: Learners must be able to create something new using
   different chunks of the information they have already mastered.
6. Evaluation: Learners must be able to present opinions, justify
   decisions, and make judgments about the information presented,
   based on previously acquired knowledge.

To use Bloom's taxonomy, consider the following sets of verbs and
descriptions for learning objectives:

1. Remember: Memorize, show, pick, spell, list, quote, recall, repeat,
   catalogue, cite, state, relate, record, name.
2. Understand: Explain, restate, alter, outline, discuss, expand,
   identify, locate, report, express, recognize, discuss, qualify,
   covert, review, infer.
3. Apply: Translate, interpret, explain, practice, illustrate,
   operate, demonstrate, dramatize, sketch, put into action, complete,
   model, utilize, experiment, schedule, use.
4. Analyze: Distinguish, differentiate, separate, take apart,
   appraise, calculate, criticize, compare, contrast, examine, test,
   relate, search, classify, experiment.
5. Evaluate: Decide, appraise, revise, score, recommend, select,
   measure, argue, value, estimate, choose, discuss, rate, assess,
   think.
6. Create: Compose, plan, propose, produce, predict, design, assemble,
   prepare, formulate, organize, manage, construct, generate, imagine,
   set-up.

[1]: https://cft.vanderbilt.edu/guides-sub-pages/blooms-taxonomy/ "Bloom's Taxonomy"
