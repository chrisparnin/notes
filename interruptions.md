Notes on Interruption for Programmers
==========

# Interruption Factors

There are several factors such as the length of an interruption, the
brain’s ability to draw on background processes, the complexity of an
interrupted task and the brain’s ability to process concurrent goals
that influence how a developer recovers from an interruption.

### Length

The length of an interruption has several implications on recovery costs
and influences on cognitive processes. A common set of questions revolve
around short-term interruptions: If someone is interrupted for a minute,
what are the consequences? If someone stopped working for 15 minutes on
a programming task to check email, should it be considered an
interruption?

In answer to the first question, most psychology experiments study
interruptions on the orders of seconds and minutes and find clear
evidence of disruption to the primary task from short-term interruptions
as measured by increases of resumption lag.

In regards to the second question, previously during my exploratory
research, I measured activity that occurred within the IDE, and for the
purpose of the study, considered an interruption to occur when there was
no activity in the programming environment for 15 minutes or more. There
are two concerns here: First the length of the interruption and second
the nature of the work occurring outside of the IDE.

For the first concern, based on my definition of interruption, any break
in work is considered an interruption. Once a minute has passed without
any interaction in the IDE, the chances of no more work occurring in the
next few hours increases significantly. As observed in the study, most
events are clustered tightly in sessions: 98% of the events are within
one minute of another. Once a developer is interrupted, he or she may pursue
other activities before returning to work on the interrupted task,
increasing the length of the interruption. This behavior has been
observed in the workplace; [O’Conaill’s study][OConaill:1995] found 40% of
interrupted tasks are not immediately resumed after an interruption.

For the second concern, knowledge workers have been observed to perform
micro task-switching [[Bannon]][Bannon:1983]. That is, they often rotate between
several active tasks and windows every few minutes (programming,
checking email, adjusting a music player, etc.) [[Judd]][Judd:2011]. As these
types of task-switches often occur within a time span of a few minutes,
they were not measured in my study. Although tasks performed outside of
the IDE can be related to the programming task, they can often be
considered a different task, such as pursuing an information retrieval
task by doing a web search related to a programming task or in the case
of email, a communication or monitoring task.

Another way to characterize these types of questions is to consider what
are the differences in short-term and long-term effects due to an
interruption? Using my framework, it is possible to characterize some of
the effects of interruption on different types of memory based on length
of an interruption. In following table, I outline
some memory effects related to short-term and long-term interruptions.

--------------------------------------------------------------
| <span style="font-variant:small-caps;">Memory</span>      | <span style="font-variant:small-caps;">Short-term</span>                | <span style="font-variant:small-caps;">Long-term</span>                            |
|-------------|-------------------------------|--------------------------------------|
| Attentive   | Focus decays                  | Items need to be restored into focus |
| Prospective | Resilient                     | Monitoring processes discontinue     |
| Associative | Resilient                     | Weak associations have faded         |
| Episodic    | Source memory disruptions     | Consolidation reduces event fidelity |
| Conceptual  | Perceptions need to be primed | Abstractions need to be primed       |

-------------------

  : Table illustrating the effects of interruption length on different
  memory types.

For short-term interruptions, different kinds of memory are affected
differently. For attentive memory, the ability to maintain focus on
items decays immediately, especially if attention must be paid to
similar types of items. Prospective and associative memory can be
resilient to short-term interruption over the course of the day.
Episodic memory can be disrupted by short-term interruptions because the
interruption may disturb processes maintaining contextual information
about events that have occurred. Perceptions that have been primed in
conceptual memory fade with disuse.

With respect to effects on long-term memory, the different memory types
are affected in different ways. Attentive memory is devastated. For
prospective memory, monitoring processes discontinue the maintenance of
prospective actions. Weak associations held in associative memory are
irretrievably lost. For events held in episodic memory, details and
specifics are lost as the events are consolidated. Abstractions that
have been primed in conceptual memory fade with disuse.

### Background Processes

The nature of the brain supports background processing of information.
If a person stopped working to go on a walk, or solved a bug while
taking a shower, what implication does this have about interruptions?

Simply going for a walk increases creativity, even prior to starting the
creative task [[Oppezzo]][Oppezzo:2014]. So going for a walk in itself has positives
consequence as a direct result of the biochemistry of the brain. What if
the person was programming, then decided to go on a walk? The
*default-mode network* [[Broyd]][Broyd:2009], is a region of the brain that is
active during moments of rest or when a person is not engaged in an a
explicit task. Default-mode network processes involve reflection over
low priority tasks or unsolved problems. These tasks are often selected
from episodic memory [[Greicius]][Greicius:2004]. However, these processes are
interrupted and disengaged when a person must attend to a demanding or
externally cued task.

Although background processes can alleviate some of the problems
associated with interruption, the tasks reflected on are processed in an
indeterminate manner and not always directed toward the goals we intend.
The background processes only engage when the programmer is not doing
explicit work on a task, which may not always be an option. Finally,
having an unsolved problem pop in and out of attention can be unpleasant
when a programmer has returned home for the day and wishes to focus on
true rest, friends, and family.

When considering interruption management strategies, background
processes can be used as another channel for preserving mental state.
Understanding when background processes are engaged, or not, can enable
researchers to predict which interrupted tasks can incur the most
resumption cost.

### Complexity and Concurrency

The complexity of an ongoing task or interrupted task has several
implications on recovery costs and influences on cognitive processes.
How can we understand resource conflicts between tasks, especially if
the goals are concurrent?

The right hemisphere of the brain can take on a secondary task if both
the primary task and secondary task are simple and do not require access
to the same types of information [[Charron]][Charron:2010]. In this way, it is
possible for the brain to process two concurrent tasks but no more.
However, both hemispheres are recruited in complex tasks [[Banich]][Banich:1998].
There is also a general overhead introduced with shifting attention
between tasks [[Jersild]][jersild1927mental].

Although the brain can support temporary shifts in attention and even
process two concurrent goals, it does so at the cost of disrupting
complex tasks which require the same resources that the secondary task
would consume. This helps explain why interruptions such as instant
messages related to a task are less disruptive [[Cutrell]][Cutrell:2000]. The brain
may be keeping the primary task in mind, while using the secondary
processes&mdash;already primed for handling secondary information
related to the primary task&mdash;to integrate and handle the
instant message. Unfortunately, not all interruptions are related to the
task at hand.

When considering interruption management strategies, complexity can be
used to understand the mental resources required to support a task.
Future research that improves the measure of task complexity can enable
researchers to predict which interrupted tasks can incur the most
resumption cost. Future interfaces can discourage developers from taking
on tasks that are too complex and suggest ways to refactoring the task
into more manageable units of work.

# Individual and Ecological Factors

There are several individual factors, such as the expertise of developer
and the user’s preferences in using memlets, and several ecological
factors such as developers that work with pair programming or in
open-office floor plans that may influence how a developer may recover
from an interruption.

### Expertise

A person’s expertise has several implications on recovery costs and
influences on cognitive processes. In general, experts are viewed as
being more resistant to interruptions than
novices [[Ericsson]][ericsson2006cambridge].

Experts have more experience in dealing with interruptions. For example,
experienced nurses devise more effective strategies for dealing with
interruptions than inexperienced nurses [[Burger]][Burger:2010]. The strategies are
more effective because experts constantly self-monitor, keep track of
what they are doing, and check for errors in their
reasoning [[Ericsson]][ericsson2006cambridge]. Finally, experts have access to more
abstract representation in their conceptual memory allowing them to
attend to more information [[Chase]][ChaseSimon1973]. Unfortunately, the path to
becoming an expert is not easily walked: For a novice, evidence suggests
this can be a 10 year journey [[Chi]][Chi:1982].

Studies examining the difference between an expert and novice find that
performance differences arise from differences in brain activity. Not
only do experts require less brain activity than novices, they also use
different parts of their brains as evidenced by EEG and fMRI
studies [[Milton]][2007:golfexperts],[[Hatfield]][EEG_Experts:2004]: Experts use conceptual
memory whereas novices use attentive memory. That is, experts are able
to exploit abstractions in conceptual memory, whereas novices must hold
primitive representations in attentive memory.

### Pair Programming

Pair programming is a software development practice where two developers
work side-by-side on a single computer during programming tasks.
Cognitively, it touches upon the idea of distributed
cognition [[Hutchins]][Hutchins:1995] and transactive
memory [[Wegner]][Wegner:transactive:memory:91]. *Distributed cognition* is a
theory that describes how cognition and knowledge can be distributed in
groups and pairs. In one study of transactive
memory [[Wegner]][Wegner:transactive:memory:91], it was found that couples
outperformed randomly assigned pairs in memory tasks, because the
couples were better than strangers at self-selecting what to remember
and anticipating what their partner would not remember.

Some developers have suggested that pair programming could assist
developers in recovering from interruption:

> Interesting article. I was surprised to discover when I first started
> pair programming 13 years ago, how one person in a pair can hold the
> context while the other person in the pair gets interrupted. We could
> get back to work in seconds.

> I would guess a pair gets interrupted less than an individual.
> Societal graces about interrupting people talking and all that. In
> addition, when a pair \*does\* get interrupted, their minds (with
> their different grasps of the context) will get back on task quicker
> through cooperation. Don’t knock it until you’ve tried it.

The first developer suggests that pair programming could provide a cognitive structure that enables one developer to handle an interruption, while allowing the other developer to continue working.  The second developer suggests that there would be minimal interruption between the pairs because a developer could use contextual and social cues to avoid interrupting the partner at moments of high mental load.  While there is no scientific confirmation of the first point, the second point is supported in the literature: In a lab study of 7 pairs of students, there was no qualitative indicators of interruptions imposed by pair programming partners [[Jones]][Jones+Fleming:2013].

Although there is some evidence that pair programming could help developers with interruption, it would not completely address the issue of interruption.  Pair programmers may still need memory aids to deal with long-term interruptions or partner swaps.  While studies have identified benefits to pair programming, those benefits are not uniformly beneficial when considering overall economic factors [[Hannay]][Hannay:2009].  In my professional experience, the prevalence of pair programming may be overstated, as many organizations may state they are practicing pair programming, while programmers selectively perform it.

### Open Offices

Some developers work in office environments that expose them to a
constant stream of interruptions. *Open-offices*, where people work in
close proximity without any rooms and sometimes no dividers, is popular
for reduced cost and increased opportunity for collaboration.

There are several sources of evidence that point out the negative
effects of interruptions in open-offices. Open-offices can lead to lower
productivity and increased stress in employees [[Brennan]][brennan2002traditional].
Workers are more like to experience both internal and external
interruptions in open-offices [[Dabbish]][dabbish2011keep].

As a result of working in open offices, workers may be forced to develop
alternative work strategies. Some might delay complex work until working
at night or at home. In experiments with frequent interruptions,
subjects naturally adapted more aggressive suspension
strategies [[Monk]][FrequentInterruptions04] &mdash;open-office workers will
likely have to do the same. During the summer of 2013, I had the
opportunity to visit several startup offices with open-office floor
plans. I observed that programmers had developed a set of cultural norms
to help deal with interruptions: For example, wearing headphones
signalling a request for no interruptions or self-segregation into quiet
areas and collaboration spaces.

The design of the office environment will have long-lasting consequences
on the productivity of the workers who work in them. Managers need to
consider more than the initial cost savings offered by a particular
office design, but also factor in long-term productivity costs. Finally,
many of the factors that need to be considered are not static, for
example, developer’s age, project maturity, and team-sizes. Which means
what works well for today’s office may not work well for tomorrow’s
office.

Related notes on [open-office experiences](https://mcwiggins.backpackit.com/pub/2940758-open-office-pathology).

[Hutchins:1995]: http://hci.ucsd.edu/hutchins/citw.html
[Wegner:transactive:memory:91]: http://scholar.harvard.edu/files/dwegner/files/wegnererberraymond1991.pdf
[Jones+Fleming:2013]: http://dx.doi.org/10.1109/VLHCC.2013.6645252
[Hannay:2009]: http://dx.doi.org/10.1016/j.infsof.2009.02.00
[dabbish2011keep]: https://www.ics.uci.edu/~gmark/Home_page/Research_files/CHI%202011%20Self-interruption.pdf
[brennan2002traditional]: http://eab.sagepub.com/content/34/3/279
[FrequentInterruptions04]: http://interruptions.net/literature/Monk-HFES04.pdf
[Judd:2011]: http://dx.doi.org/10.1016/j.compedu.2010.10.004
[OConaill:1995]: http://dl.acm.org/citation.cfm?id=223665
[Bannon:1983]: http://doi.acm.org/10.1145/800045.801580
[Oppezzo:2014]: http://view.ncbi.nlm.nih.gov/pubmed/24749966
[Broyd:2009]: http://dx.doi.org/10.1016/j.neubiorev.2008.09.002
[Greicius:2004]: http://dx.doi.org/10.1162/0898929042568532
[Charron:2010]: http://dx.doi.org/10.1126/science.1183614
[Banich:1998]: http://view.ncbi.nlm.nih.gov/pubmed/9520311
[jersild1927mental]: http://doi.apa.org/?uid=1928-00322-001
[Cutrell:2000]: http://citeseer.ist.psu.edu/cutrell01notification.html
[ericsson2006cambridge]: http://www.cambridge.org/us/academic/subjects/psychology/cognition/cambridge-handbook-expertise-and-expert-performance
[Burger:2010]: http://view.ncbi.nlm.nih.gov/pubmed/20685907
[ChaseSimon1973]: http://matt.colorado.edu/teaching/highcog/fall8/cs73.pdf
[Chi:1982]: http://www.public.asu.edu/~mtchi/papers/ChiGlaserRees.pdf
[2007:golfexperts]: http://dx.doi.org/10.1016/j.neuroimage.2007.01.003
[EEG_Experts:2004]: http://view.ncbi.nlm.nih.gov/pubmed/15375345


