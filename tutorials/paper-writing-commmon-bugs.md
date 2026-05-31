# Common Bugs in Writing



http://www.cs.columbia.edu/~hgs/etc/writing-bugs.html

Last updated 01/12/2021 11:52:17 by Henning Schulzrinne

Preface (suggested by Bob Briscoe)

 - Be clear what you're trying to say before you write it.
 - Don't get attached to words you have written; be prepared to scrap
   what you wrote while you were thrashing around trying to work out
   what you wanted to say, even if its a whole paper.

Like almost all rules, there are cases where breaking them is a good
idea and seasoned writers may well object with "but" responses for
some of these. Thus, consider the rules below as mental rumble
strips - you should probably slow down and think if you encounter
these cases.

 1. Avoid use of passive tense if at all possible. Example: "In each
    reservation request message, a refresh interval used by the sender
    is included." reads better and shorter as "Each ... message
    includes ..."

 2. Use strong verbs instead of lots of nouns and simple terms rather
    than fancy-sounding ones. Examples:

      | verbose, weak verbs, bad | 	short, strong, good |
      | make assumption          | 	assume              |
      | is a function of         | 	depends on          |
      | is an illustration       | 	illustrates, shows  |
      | is a requirement         | 	requires, need to   |
      | utilizes                 | 	uses                |
      | had difference           | 	differed            |

 3. If you find yourself saying "In other words," it means you didn't
    say it clearly enough the first time. Go back and rewrite the
    first attempt.

 4. Avoid filler words, e.g., by converting sentences into a simple
    actor-action-object phrasing.

 5. Check for missing articles, particularly if your native tongue
    doesn't have them. Roughly, concepts and classes of things don't,
    most everything else more specific does. ("Routers route packets.
    The router architecture we consider uses small rodents.") Don't
    use articles in front of proper nouns and names ("Internet
    Explorer is a popular web browser. The current version number is
    5.0. Bill Gates did not write Internet Explorer.")

 6. Each sentence in a paragraph must have some logical connection to
    the previous one. For example, it may describe an exception
    ("but," "however"), describe a causality ("thus," "therefore,"
    "because of this"), indicate two facets of an argument ("on the
    one hand," "on the other hand"), enumerate sub-cases ("first,"
    "secondly") or indicate a temporal relationship ("then,"
    "afterwards"). If there are no such hints, check if your sentences
    are indeed part of the same thought. A new thought should get its
    own paragraph, but still clearly needs some logical connection to
    the paragraphs that preceded it.

 7. Protocol abbreviations typically do not take an article, even if
    the expanded version does. For example, "The Transmission Control
    Protocol delivers a byte stream" but "TCP delivers a byte stream,"
    since it an abstract term. ("The TCP design has been successful."
    is correct since the article refers to the design, not TCP.)

    Note that abbreviations for organizations do take a definite
    article, as in "The IETF standardized TCP."

    Since the "P" in TCP, UDP and similar abbreviations already stands
    for "protocol," saying the "the TCP protocol" is redundant, albeit
    common.

 8. Use consistent tense - present, usually, unless reporting results
    achieved in earlier papers.

 9. None: None can take either singular or plural verbs, depending on
    the intended meaning (or taste). Both none of these mistakes are
    common and none of these mistakes is common are correct.

 10. Use hyphens for concatenated words: "end-to-end architecture,"
     "real-time operating system" (but "the computer may analyze the
     results in real time"), "per-flow queueing," "flow-enabled,"
     "back-to-back," ...

 11. Don't overuse dashes for separation, as they interrupt the flow
     of words. Dashes may be appropriate where you want to contrast
     thoughts very strongly or the dash part is a surprise of some
     sort. Think of it as a very long pause when speaking. In many
     cases, a comma-separated phrase works better. If you do use a
     dash, make sure it's not a hyphen (- in LaTeX), but an em-dash
     (--- in LaTeX).

 12. Avoid scare quotes, as they indicate that the writer is
     distancing himself from the term or the term is meant to be
     ironic.

 13. Numbers ten or less are spelled out: "It consists of three
     fields," not "3 fields".

 14. Use until instead of the colloquial till.

 15. Use. Eq. 7, not Equation (7), unless you need to fill empty
     pages.

 16. Optimal can't be improved - more optimally should be better or
     maybe more nearly optimal.

 17. Avoid in-line enumeration like: "Packets can be (a) lost, (b)
     stolen, (c) get wet." The enumeration only interrupts the flow of
     thought.

 18. Avoid itemization (bullets) in most cases, as they take up extra
     space and make the paper read like PowerPoint slides. Bullets
     can, however, be used effectively to emphasize key points, if
     used sparingly.

 19. Avoid bulleted lists of one-sentence paragraphs. They make your
     paper look like a slide presentation and interfere with smooth
     reading.

 20. Instead of "Reference [1] shows" or "[1] shows," use "Smith [1]
     showed" or "Smith and Jones [1] showed" or "Smith et al. [1]
     showed" (if more than two authors). "et al." is generally used
     for papers with more than two authors.

 21. Use normal capitalization in captions ("This is a caption," not
     "This is a Caption") unless your style guide requires
     heading-style capitalization.

 22. All headings must be capitalized consistently, either in heading
     style, capitalizing words, or sentence style, across all levels
     of headings.

 23. Parentheses or brackets are always surrounded by a space: "The
     experiment(Fig. 7)shows" is wrong; "The experiment (Fig. 7)
     shows" is right.

 24. Avoid excessive parenthesized remarks as they make the text hard
     to read; fold into the main sentence.

 25. The material should make just as much sense without the
     footnotes. If the reader constantly has to look at footnotes,
     they are likely to lose their original place in the text.

 26. There is no space between the text and the superscript for the
     footnote. I.e., in LaTeX, it's text\textsuperscript{} rather than text
     \textsuperscript{}.

 27. Check that abbreviations are always explained before use.
     Exceptions, when addressed to the appropriate networking
     audience: ATM, BGP, ftp, HTTP, IP, IPv6, RSVP, TCP, UDP, RTP,
     RIP, OSPF, BGP, SS7.

 28. Never start a sentence with "and". (There are exceptions to this
     rule, but these are best left to English majors.)

 29. Don't use colons (:) in mid-sentence. For example, "This is
     possible because: somebody said so" is wrong - the part before
     the colon must be a complete sentence.

 30. Don't start sentences with "That's because".

 31. In formal writing, contractions like don't, doesn't, won't or
     it's are generally avoided.

 32. Be careful not to confuse its with it's (it is).

 33. Vary expressions of comparison: "Flying is faster than driving"
     is much better than "Flying has the advantage of being faster" or
     "The advantage of flying is that it is faster.".

 34. Don't use slash-constructs such as "time/money". This is
     acceptable for slides, but in formal prose, such expressions
     should be expanded into "time or money" or "time and money,"
     depending on the meaning intended.

 35. Avoid cliches like "recent advances in ...," "exponential
     growth," and "paradigm".

 36. Don't use symbols like "+" (for "and"), "%" (for "fraction" or
     "percentage") or "->" (for "follows" or "implies") in prose,
     outside of equations. These are only acceptable in slides.

 37. Avoid capitalization of terms. Your paper is not the U.S.
     Constitution or Declaration of Independence. Technical terms are
     in lower-case, although some people use upper case when
     explaining an acronym, as in "Asynchronous Transfer Mode (ATM)".

 38. Expand all acronyms on first use, except acronyms that every
     reader is expected to know. (In a research paper on TCP,
     expanding TCP is probably not needed - somebody who doesn't know
     what TCP stands for isn't likely to appreciate the rest of the
     paper, either.)

 39. Each paragraph should have a lead sentence summarizing its
     content. If this doesn't work naturally, the paragraph is
     probably too short. Try reading just the first lines of each
     paragraph - the paper should still make sense.

 40. $i$th, not $i-th$.

 41. Units are always in roman font, never italics or LaTeX math mode.
     Units are set off by one (thin) space from the number. In LaTeX,
     use ~ to avoid splitting number and units across two lines.

 42. For readability, powers of a 1,000 are divided by commas.

 43. Use "kb/s" or "Mb/s," not "kbps" or "Mbps" - the latter are not
     scientific units. Be careful to distinguish "Mb" (Megabit) and
     "MB" (Megabytes), in particular "kb" (1,000 bits) and "KB" (1,024
     bytes).

 44. It's always kHz (lower-case k), not KHz or KHZ.

 45. It's Wi-Fi, not WiFi (or wifi), since this is a trademark.

 46. Operating systems such as Android, (Mac)OSX, Linux or Windows are
     typically capitalized.

 47. It is  not common to use  the trademark symbol (R)  (or its country
     cousins SM and TM) unless you are  the owner of the mark and then
     only on first use.

 48. Use "ms," not "msec," for milliseconds.

 49. Use "0.5" instead of ".5," i.e., do not omit the zero in front of
     the decimal point.

 50. Avoid "etc."; use "for example," "such as," "among others" or,
     better yet, try to give a complete list.

 51. If you say, "for example" or "like," do not follow this with
     "etc.". Thus, it's "fruit like apples, bananas and oranges".

 52. Avoid excessive use of "i.e.". Vary your expression: "such as,"
     "this means that," "because," ....

 53. Remember that "i.e." and "e.g." are always followed by a comma.

 54. Do not use ampersands (&) or slash-abbreviations (such as s/w or
     h/w) in formal writing; they are acceptable for slides.

 55. "respectively" is preceded by a comma, as in "The light bulbs
     lasted 10 and 100 days, respectively."

 56. Therefore, however, hence and thus are usually followed by a
     comma, as in "Therefore, our idea should not be implemented."

 57. Never use "related works" unless you are talking about works of
     art. It's "related work".

 58. Similarly, "codes" refer to encryption keys, not multiple
     programs. You would say "I modified multiple programs," not
     "multiple codes".

 59. Use "in Figure 1" instead of "following figure" since figures may
     get moved during the publication or typesetting process.

 60. Text columns in tables are left-aligned, numeric columns are
     aligned on the decimal or right-aligned.

 61. Section, Figure and Table are capitalized, as in "As discussed in
     Section 3". Figure can be abbreviated as Fig., but the others are
     not usually abbreviated.

 62. Section titles are not followed by a period.

 63. In LaTeX, tie the figure number to the reference, so that it
     doesn't get broken across two lines:

     Fig.~ref{fig:arch}

 64. Do not use GIF images for figures, as GIFs produce horrible print
     quality and are huge. Export into PostScript.

 65. Only use line graphs when you are trying to show a functional or
     causal relationship between variables. When showing different
     experiments, for example, use bar graphs or scatter plots.

 66. Figures show, depict, indicate, illustrate. Avoid "(refer to Fig.
     17)".

 67. If you quote something literally, enclose it in quotation marks
     or show it indented and in smaller type ("block quote").

 68. Do not refer to colors in graphs. Many people will print the
     paper on a monochrome (black and white) printer and will have no
     idea what you are talking about when referring to the red or blue
     line.

 69. Avoid numbers with artificial precision. Unless you have done
     enough experiments to be sure that the value measured is indeed
     meaningful to five digits after the decimal point, you're
     overstating your results.

 70. Do not forget to acknowledge your funding support.

 71. All references must use consistent capitalization for the paper
     titles, i.e., either all title-case or all sentence-case.

 72. Technical report citations must have the name of the organization
     such as the university or company. Conferences must cite the
     location.

 73. Check your references to make sure they are up to date.

 74. References should be consistent: all authors should either be
     given with their full name (John Doe) or abbreviated (J. Doe),
     but not combinations.

 75. Conference references should contain the location of the
     conference, the month and some indication such as "Proc. of" or
     "Conference". Journal references always contain the volume, issue
     number and pages.

 76. Only include the year of the publication once, rather than
     multiple times in different contexts.

See also University of Minnesota Style Manual.

Thanks to Christian Bettstetter for contributions.

Last updated 01/12/2021 11:52:17 by Henning Schulzrinne