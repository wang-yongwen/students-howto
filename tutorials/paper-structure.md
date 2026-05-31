# The structure of paper/report in Systems

http://www.cs.ucr.edu/~michalis/TECHWRITING/structure.html

Michalis Faloutsos

U.C. Riverside

## Some rules:

 - Recursiveness 1. In every section, the first paragraph should be a
   summary/overview of the section. You can actually start by saying:
   "In this section, we present..."

 - Recursiveness 2. In every paragraph, the first (or second line)
   should correspond to summary of the paragraph.

 - Top-Down: Start from high level and start increasing the details
   slowly.

 - Prepare the reader: Reports are not suspense thrillers. The reader
   should have an idea of where you are trying to get at.

 - Adapt: These rules are meant as guidelines. Paper requirements can
   differ. However, when you break one of these rules, be aware of it
   and have a good justification.

 - Personal pet-peeve: huge introductions: if you can not say it in 1.5
   page probably it is not very clear in your mind or you don't use the
   right level of abstraction.

Note: I have probably broken all these rules. I usually ended up paying
for it.

 - Total Paper length: ~15 pages.

Not all sections are compulsory from the list: [[#our][Our Idea]], [[#ana][Analysis]],
[[#exp][Experiments]], [[#dis][Discussion]]

---------

## Abstract

[1 paragraph 200-300 word. This is the ad and trailer for the paper:
it has to be an executive summary of your work in such a way as to
attract attention and get the reader to read more. Think of how you
would explain the work to your office mate]

 - 1-2 lines: goal of this paper

 - 1-2 lines: motivation and importance of work

 - 1-2 lines: per result or contribution of our work [it is good if you
  can quantify your claims with numbers that refer to intuitive or
  easily explainable metrics i.e. 50% faster]

[At paragraph level:

=*= indicates one or at most two paragraphs

=**= means as many paragraphs area needed, but don't do crazy]

## Introduction

[1-1.5 pages]

 - * What is the problem, motivation, importance, main contribution

 - * The problem: high level definition, significance

 - * Previous work [at most one line per relevant paper, leave details
    for next section]

 - * Our contribution: possibly list of results and contributions

 - * "The rest of this paper is structured as follows. In section 2,....."

## Background and Model

[1-1.5 pages]

 - * Definitions, scenario, model

 - * Previous work [provide details only if this will help show where
   your work is different or better. Make sure you reference all
   related work and especially that by people in the committee!]

 - * Weaknesses of previous work or the absence of the thing you are proposing

 - * Assumptions and limitations of your work. [Be honest, but don't
   condemn your work].

## Our Idea

[as required]

 - * The innovation in brief
 - * New definitions, if necessary
 - ** What it is and how it works
 - ** Explanation of fine points, clarifications

## Analysis

[as required]

 - * Overview of what we prove in this section

 - * Analysis-specific definitions [i.e. a graph structure that you will use in the proof]

 - ** Analysis  - proofs

 - * Comments  - Meaning of proofs at an intuitive or practical  level

## Experimental Results

[ as required]
 - * Overview of experiments: what we do measure, what we don't, why

 - * Simulation model or measuring infrastructure

 - ** Experimental Results

  1. use a heading (in bold) to distinguish experiments (i.e. The
     effect of size on performance or even better The size does not
     affect the performance..)

  2. each plot should have a clear reason for appearing (ie with more
     load we get worse throughput)

  3. explain each plot: the axis, what we see, what is the trend, why
     this is the trend

  4. statistical comments will strengthen your results: confidence
     interval, correlation coefficient etc.

  5. Each figure should be fairly stand alone and self explanatory:
     captions should be readable and understandable.

  6. Comments, discussion, explanations

## Discussion

[1-2 pages. If you have space and ideas, you can strengthen the
importance of your work by showing: a) significance, b) relation to
other pieces of work, c) possible practical applications]

 - * Overview of section

 - ** Paragraphs according to needs

## Conclusions

[1-1.5]
[Conclusions are very important. Do not expect that the reader
remembers everything you told him/her. Having stated the definitions,
you can now be more specific that  in the introduction]

 - * Overview what this work was about.

 - * Main results and contributions

 - * Comments on importance or

 - * Tips for practical use [how your results or experience can help
    someone in practice or another researcher to use your simulator or
    avoid pitfalls]

 - * Future work. Reinforce the importance of work, but avoid giving out
    your ideas].

## References

[It has to be correct, complete, and accurate]

## Appendices

[as required]
Appendices are no man's land: you can write whatever you want:
reviewers are not obliged to read through them.  Suggested uses:

 1. provide additional results that strengthen your arguments but are
    not crucial
 2. maintain the flow of the paper by putting here a lengthy proof or
    discuss a detail
 3. address an issue that shows you have thought the issue in depth