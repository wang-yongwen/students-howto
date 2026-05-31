# Writing Technical Articles

http://www.cs.columbia.edu/~hgs/etc/writing-style.html

The notes below apply to technical papers in computer science and
electrical engineering, with emphasis on papers in systems and
networks.

Read Strunk and White, Elements of Style. Again.

Give the paper to somebody else to read. If you can, find two people:
one person familiar with the technical matter, another only generally
familiar with the area.

Papers can be divided roughly into two categories, namely *original
research papers* and *survey papers*. There are papers that combine the
two elements, but most publication venues either only accept one or
the other type or require the author to identify whether the paper
should be evaluated as a research contribution or a survey paper.
(Most research papers contain a "related work" section that can be
considered a survey, but it is usually brief compared to the rest of
the paper and only addresses a much narrower slice of the field.)

## Research Papers

A good research paper has a clear statement of the problem the paper
is addressing, the proposed solution(s), and results achieved. It
describes clearly what has been done before on the problem, and what
is new.

The goal of a paper is to describe novel technical results. There are
four types of technical results:

 1. An algorithm;

 2. A system construct: such as hardware design, software system,
   protocol, etc.;

   One goal of the paper is to ensure that the next person who designs
   a system like yours doesn't make the same mistakes and takes
   advantage of some of your best solutions. So make sure that the
   hard problems (and their solutions) are discussed and the
   non-obvious mistakes (and how to avoid them) are discussed. (Craig
   Partridge)

 3. A performance evaluation: obtained through analyses, simulation or
   measurements;

 4. A theory: consisting of a collection of theorems.

 A paper should focus on

 - describing the results in sufficient details to establish their
  validity;

 - identifying the novel aspects of the results, i.e., what new
  knowledge is reported and what makes it non-obvious;

 - identifying the significance of the results: what improvements and
  impact do they suggest.

## Paper Structure

### Typical outline of a paper is:

1. Abstract, typically not more than 100-150 words;

2. Introduction (brief!): introduce problem, outline solution; the
statement of the problem should include a clear statement why the
problem is important (or interesting).

3. Related Work (or before summary). Hint: In the case of a conference,
make sure to cite the work of the PC co-chairs and as many other PC
members as are remotely plausible, as well as from anything relevant
from the previous two proceedings. In the case of a journal or magazine,
cite anything relevant from last 2-3 years or so volumes.

4. Outline of the rest of the paper: "The remainder of the paper is
organized as follows. In Section 2, we introduce ..Section 3 describes
... Finally, we describe future work in Section 5." [Note that Section
is capitalized. Also, vary your expression between "section" being the
subject of the sentence, as in "Section 2 discusses ..." and "In
Section, we discuss ...".]

5. Body of paper

 - problem
 - approach, architecture
 - results

The body should contain sufficient motivation, with at least one
example scenario, preferably two, with illustrating figures, followed
by a crisp generic problem statement model, i.e., functionality,
particularly emphasizing "new" functionality. The paper may or may not
include formalisms. General evaluations of your algorithm or
architecture, e.g., material proving that the algorithm is O(log N),
go here, not in the evaluation section.

*Architecture* of proposed system(s) to achieve this model should be
 more generic than your own peculiar implementation. Always include at
 least one figure.

*Realization*: contains actual implementation details when
 implementing architecture isn't totally straightforward. Mention
 briefly implementation language, platform, location, dependencies on
 other packages and minimum resource usage if pertinent.

*Evaluation*: How does it really work in practice? Provide real or
 simulated performance metrics, end-user studies, mention external
 technology adoptors, if any, etc.

6. Related work, if not done at the beginning

7. Summary and Future Work

often repeats the main result

8. Acknowledgements

9. Bibliography

10.Appendix (to be cut first if forced to):

 - detailed protocol descriptions

 - proofs with more than two lines

 - other low-level but important details

It is recommended that you write the approach and results sections
first, which go together. Then problem section, if it is separate from
the introduction. Then the conclusions, then the intro. Write the
intro last since it glosses the conclusions in one of the last
paragraphs. Finally, write the abstract. Last, give your paper a
title.

## Title

 - Avoid all but the most readily understood abbreviations.

 - Avoid common phrases like "novel", "performance evaluation" and
  "architecture", since almost every paper does a performance
  evaluation of some architecture and it better be novel. Unless
  somebody wants to see 10,000 Google results, nobody searches for
  these types of words.


Use adjectives that describe the distinctive features of your work,
e.g., reliable, scalable, high-performance, robust, low-complexity, or
low-cost. (There are obviously exceptions, e.g., when the performance
evaluation is the core of the paper. Even in that case, something more
specific is preferable, as in "Delay measurements of X" or "The
quality of service for FedEx deliveries".)

## Abstract

The abstract must not contain references, as it may be used without
the main article. It is acceptable, although not common, to identify
work by author, abbreviation or RFC number. (For example, "Our
algorithm is based upon the work by Smith and Wesson.")

Avoid use of "in this paper" in the abstract. What other paper would
you be talking about here?

Avoid general motivation in the abstract. You do not have to justify
the importance of the Internet or explain what QoS is.

Highlight not just the problem, but also the principal results. Many
people read abstracts and then decide whether to bother with the rest
of the paper.

Since the abstract will be used by search engines, be sure that terms
that identify your work are found there. In particular, the name of
any protocol or system developed and the general area ("quality of
service", "protocol verification", "service creation environment")
should be contained in the abstract.

Avoid equations and math. Exceptions: Your paper proposes E = m c 2.

## Introduction

Avoid stock and cliche phrases such as "recent advances in XYZ" or
anything alluding to the growth of the Internet.

Be sure that the introduction lets the reader know what this paper is
about, not just how important your general area of research is.
Readers won't stick with you for three pages to find out what you are
talking about.

The introduction must motivate your work by pinpointing the problem
you are addressing and then give an overview of your approach and/or
contributions (and perhaps even a general description of your
results). In this way, the intro sets up my expectations for the rest
of your paper -- it provides the context, and a preview.

Repeating the abstract in the introduction is a waste of space.

Example bad introduction:


## Body of Paper

Hints and common mistakes

## Bibliography

Avoid use of *et al*. in a bibliography unless list is very long (five
or more authors). The author subsumed into et al. may be your advisor
or the reviewer... Note punctuation of et al..

If writing about networks or multimedia, use the network bibliography.
All entries not found there should be sent to me. A listing of
frequently-used references for networks is available.

Internet drafts must be marked ``work in progress''.

Book citations include publication years, but no ISBN number.

It is now acceptable to include URLs to material, but it is probably
bad form to include a URL pointing to the author's web page for papers
published in IEEE and ACM publications, given the copyright situation.
Use it for software and other non-library material. Avoid long URLs;
it may be sufficient to point to the general page and let the reader
find the material. General URLs are also less likely to change.

Leave a space between first names and last name, i.e., "J. P. Doe",
not "J.P.Doe".

## Acknowledgements

Generally, anonymous reviewers don't get acknowledged, unless they
really provided an exceptional level of feedback or insight. Rather
than "We thank X for helping us with Y", you might vary this as "X
helped with Y.".

## Reporting Numerical Results and Simulations

In all but extended abstracts, numerical results and simulations
should be reported in enough detail that the reader can duplicate the
results. This should include all parameters used, indications of the
number of samples that contributed to the analysis and any initial
conditions, if relevant.

When presenting simulation results, provide insight into the
statistical confidence. If at all possible, provide confidence
intervals. If there's a "strange" behavior in the graph (e.g., a dip,
peak or change in slope), this behavior either needs to be explained
or reasons must be given why this is simply due to statistical
aberration. In the latter case, gathering more samples is probably
advised.

Figures should be chosen wisely. You can never lay out the whole
parameter space, so provide insight into which parameters are
significant over what range and which ones are less important. It's
not very entertaining to present lots of flat or linear lines.

The description of the graph should not just repeat the graphically
obvious such as "the delay rises with the load", but explain, for
example, how this increase relates to the load increase. Is it linear?
Does it follow some well-known other system behaviors such as standard
queueing systems?

## Things to Avoid

Too much motivational material: 3 reasons are enough -- and they
should be described very briefly.

Describing the obvious parts of the result: "Obvious" is defined as
any result that a graduate of our program would suggest as a solution
if you pose the problem that the result solves.

Describing unnecessary details: a detail is unnecessary, if its
omission will not harm the reader's ability to understand the
important novel aspects of the result.

Spelling errors: With the availability of spell checkers, there is no
reason to have spelling errors in a manuscript. If you as the author
didn't take the time to spell-check your paper, why should the editor
or reviewer take the time to read it or trust that your diligence in
technical matters is any higher than your diligence in presentation?
Note, however, that spell checkers don't catch all common errors, in
particular word duplication ("the the"). If in doubt, consult a
dictionary such as the (on line) Merriam Webster.

## Guidelines for Experimental Papers

"Guidelines for Experimental Papers" set forth for researchers
submitting articles to the journal, Machine Learning.

 1. Papers that introduce a new learning "setting" or type of
   application should justify the relevance and importance of this
   setting, for example, based on its utility in applications, its
   appropriateness as a model of human or animal learning, or its
   importance in addressing fundamental questions in machine learning.

 2. Papers describing a new algorithm should be clear, precise, and
   written in a way that allows the reader to compare the algorithm to
   other algorithms. For example, most learning algorithms can be
   viewed as optimizing (at least approximately) some measure of
   performance. A good way to describe a new algorithm is to make this
   performance measure explicit. Another useful way of describing an
   algorithm is to define the space of hypotheses that it searches
   when optimizing the performance measure.

 3. Papers introducing a new algorithm should conduct experiments
   comparing it to state-of-the-art algorithms for the same or similar
   problems. Where possible, performance should also be compared
   against an absolute standard of ideal performance. Performance
   should also be compared against a naive standard (e.g., random
   guessing, guessing the most common class, etc.) as well. Unusual
   performance criteria should be carefully defined and justified.

 4. All experiments must include measures of uncertainty of the
   conclusions. These typically take the form of confidence intervals,
   statistical tests, or estimates of standard error. Proper
   experimental methodology should be employed. For example, if "test
   sets" are used to measure generalization performance, no
   information from the test set should be available to the learning
   process.

 5. Descriptions of the software and data sufficient to replicate the
   experiments must be included in the paper. Once the paper has
   appeared in Machine Learning, authors are strongly urged to make
   the data used in experiments available to other scientists wishing
   to replicate the experiments. An excellent way to achieve this is
   to deposit the data sets at the Irvine Repository of Machine
   Learning Databases. Another good option is to add your data sets to
   the DELVE benchmark collection at the University of Toronto. For
   proprietary data sets, authors are encouraged to develop synthetic
   data sets having the same statistical properties. These synthetic
   data sets can then be made freely available.

 6. Conclusions drawn from a series of experimental runs should be
   clearly stated. Graphical display of experimental data can be very
   effective. Supporting tables of exact numerical results from
   experiments should be provided in an appendix.

 7. Limitations of the algorithm should be described in detail.
   Interesting cases where an algorithm fails are important in
   clarifying the range of applicability of an algorithm.

## The Conference Review Process

It is hard to generalize the review process for conferences, but most
reputable conferences operate according to these basic rules:

 1. The paper is submitted to the technical program chair(s). Many
   current conferences require electronic submission, in either
   PostScript or PDF formats, occasionally in Word.

 2. The technical program chair assigns the paper to one or more
   technical program committee members, hopefully experts in their
   field. The identity of this TPC member is kept secret.

 3. The TPC member usually provides a review, but may also be asked to
   find between one and three reviewers who are not members of the
   TPC. They may be colleagues of the reviewer at the same
   institution, his or her graduate students or somebody listed in the
   references. The graduate student reviews can be quite helpful,
   since these reviewers often provide more detailed criticism rather
   than blanket dismissal. Any good conference will strive to provide
   at least three reviews, however, since conferences operate under
   tight deadlines and not all reviewers deliver as promised, it is
   not uncommon that you receive only two reviews.

 4. The technical program chair then collects the reviews and sorts the
   papers according to their average review scores.

 5. The TPC (or, rather, the subset that can make the meeting), then
   meets in person or by phone conference. Usually, the bottom third
   and the top third are rejected and accepted without (much) further
   discussion. The papers discussed are those in the middle of the
   range, where a TPC member feels strongly that the paper ended up in
   the wrong bin, or where the review scores differ significantly, in
   particular if there are only two reviews.

## Other References

 - http://www.bartleby.com/ Bartleby has dictionaries, grammars, an
  encyclopedia, and Columbia Guide To Standard American English

 -  http://istpub.berkeley.edu:4201/style/ Berkeley Information Systems
   and Technology Publications style guide

 - http://www.uiowa.edu/~c030162/Common/Writing_Tips/tips.html Writing Tips

 - http://ucsub.colorado.edu/~robertme/paperkey.htm Key to common comments made on your papers

 - http://contentselect.pearsoned.com/unit10.html Drafting the Paper in an Academic Style

 - http://www-relg-studies.scu.edu/facstaff/murphy/courses/style-sheet.htm Religious Studies style sheet

 - http://www.wisdom.weizmann.ac.il/~oded/writing.html Cisco style guide

 - http://www.wisdom.weizmann.ac.il/~oded/writing.html Oded Goldreich wrote an essay entitled "How not to write a paper",
  with recommendations on style and organization.

 - http://www-cs-faculty.stanford.edu/~knuth/klr.html Don Knuth has online the TeX source of a book on "Mathematical
  Writing" (also useful for Computer Science).

 - http://www.cs.ucr.edu/~michalis/TECHWRITING/structure.html The structure of paper/report in Systems, by Michalis Faloutsos,
  U.C. Riverside

Talks

 - "The Short Talk" (Charles Van Loan)
 - "Pointers on giving a talk" (D. Messerschmitt)
 - Tips for Preparing Delivering Scientific Talks and Using Visual Aids (ONR)

Contributors

This page contains material provided by Gail Kaiser, Craig Partridge, Sumit Roy, Eric Siegel, Sal Stolfo, Luca Trevisan, Yechiam Yemini, Erez Zadok.