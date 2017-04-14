# Planetary Technology Standard RFCs
[PTS RFCs]: #pts-rfcs

Many changes, including bug fixes and documentation improvements can be
implemented and reviewed via the normal GitHub pull request workflow.

Some changes though are "substantial", and we ask that these be put
through a bit of a design process and produce a consensus among the Planetary Technology
community and the [sub-team]s.

The "RFC" (request for comments) process is intended to provide a
consistent and controlled path for changes to the Planetary Technology Standard (PTS).

## Table of Contents
[Table of Contents]: #table-of-contents
* [Opening](#pts-rfcs)
* [Table of Contents]
* [When you need to follow this process]
* [Before creating an RFC]
* [What the process is]
* [The role of the shepherd]
* [The RFC life-cycle]
* [Reviewing RFC's]
* [Implementing an RFC]
* [RFC Postponement]
* [Help this is all too informal!]


## When you need to follow this process
[When you need to follow this process]: #when-you-need-to-follow-this-process

You need to follow this process if you intend to make "substantial" changes to
the Planetary Technology Standard, or the RFC process itself. What constitutes a
"substantial" change is evolving based on community norms and varies depending
on what part of the standard you are proposing to change, but may include the
following.

   - ?.
   - ?

Some changes do not require an RFC:

   - ?.
   - ?.

If you submit a pull request to implement a change without going
through the RFC process, it may be closed with a polite request to
submit an RFC first.

For more details on when an RFC is required, please see the following specific
guideline:

* [PlanetaryTechnologyStandard changes](standard_changes.md)


## Before creating an RFC
[Before creating an RFC]: #before-creating-an-rfc

A hastily-proposed RFC can hurt its chances of acceptance. Low quality
proposals, proposals for previously-rejected features, or those that
don't fit into the near-term roadmap, may be quickly rejected, which
can be demotivating for the unprepared contributor. Laying some
groundwork ahead of the RFC can make the process smoother.

Although there is no single way to prepare for submitting an RFC, it
is generally a good idea to pursue feedback from other project
developers beforehand, to ascertain that the RFC may be desirable:
having a consistent impact on the project requires concerted effort
toward consensus-building.

The most common preparations for writing and submitting an RFC include
talking the idea over on [#pts-discuss][discuss], filing and discusssing ideas
on the [RFC issue tracker][issues], and occasionally posting
'pre-RFCs' on [the discussion forum][discuss] for early
review.

As a rule of thumb, receiving encouraging feedback from long-standing
project members, and particularly members of the relevant [sub-team]
is a good indication that the RFC is worth pursuing.

[issues]: https://github.com/planetarytechnology/rfcs/issues
[discuss]: https://discuss.planetary.technology


## What the process is
[What the process is]: #what-the-process-is

In short, to get a major change added to the Standard, one must first get the
RFC merged into the RFC repo as a markdown file. At that point the RFC
is 'active' and may be implemented with the goal of eventual inclusion
into the Standard.

* Fork the RFC repo http://github.com/planetarytechnology/rfcs
* Copy `0000-template.md` to `text/0000-my-feature.md` (where 'my-feature' is
descriptive. don't assign an RFC number yet).
* Fill in the RFC. Put care into the details: RFCs that do not present
convincing motivation, demonstrate understanding of the impact of the design, or
are disingenuous about the drawbacks or alternatives tend to be poorly-received.
* Submit a pull request. As a pull request the RFC will receive design feedback
from the larger community, and the author should be prepared to revise it in
response.
* Each pull request will be labeled with the most relevant [sub-team].
* Each sub-team triages its RFC pull requests. The sub-team will either close
the pull request (for RFCs that clearly will not be accepted) or assign it a
*shepherd*. The shepherd is a trusted member who is familiar with the RFC
process, who will help to move the RFC forward, and ensure that the right people
see and review it.
* Build consensus and integrate feedback. RFCs that have broad support are much
more likely to make progress than those that don't receive any comments. The
shepherd assigned to your RFC should help you get feedback from Planetary Technology members
as well.
* The shepherd may schedule meetings with the author and/or relevant
stakeholders to discuss the issues in greater detail.
* The sub-team will discuss the RFC pull request, as much as possible in the
comment thread of the pull request itself. Offline discussion will be summarized
on the pull request comment thread.
* RFCs rarely go through this process unchanged, especially as alternatives and
drawbacks are shown. You can make edits, big and small, to the RFC to
clarify or change the design, but make changes as new commits to the pull
request, and leave a comment on the pull request explaining your changes.
Specifically, do not squash or rebase commits after they are visible on the pull
request.
* Once both proponents and opponents have clarified and defended positions and
the conversation has settled, the RFC will enter its *final comment period*
(FCP). This is a final opportunity for the community to comment on the pull
request and is a reminder for all members of the sub-team to be aware of the
RFC.
* The FCP lasts one week. It may be extended if consensus between sub-team
members cannot be reached. At the end of the FCP,  the [sub-team] will either
accept the RFC by merging the pull request, assigning the RFC a number
(corresponding to the pull request number), at which point the RFC is 'active',
or reject it by closing the pull request. How exactly the sub-team decide on an
RFC is up to the sub-team.


## The role of the shepherd
[The role of the shepherd]: #the-role-of-the-shepherd

During triage, every RFC will either be closed or assigned a shepherd from the
relevant sub-team. The role of the shepherd is to move the RFC through the
process. This starts with simply reading the RFC in detail and providing initial
feedback. The shepherd should also solicit feedback from people who are likely
to have strong opinions about the RFC. When this feedback has been incorporated
and the RFC seems to be in a steady state, the shepherd and/or sub-team leader
will announce an FCP. In general, the idea here is to "front-load" as much of
the feedback as possible before the point where we actually reach a decision -
by the end of the FCP, the decision on whether or not to accept the RFC should
usually be obvious from the RFC discussion thread. On occasion, there may not be
consensus but discussion has stalled. In this case, the relevant team will make
a decision.


## The RFC life-cycle
[The RFC life-cycle]: #the-rfc-life-cycle

Once an RFC becomes active then authors of the affected repo may implement it and submit
the changes as a pull request. Being 'active' is not
a rubber stamp, and in particular still does not mean the changes will
ultimately be merged; it does mean that in principle all the major
stakeholders have agreed to the changs and are amenable to merging
it.

Furthermore, the fact that a given RFC has been accepted and is
'active' implies nothing about what priority is assigned to its
implementations, nor does it imply anything about whether a member
has been assigned the task of implementing the changes.

In general, once accepted, RFCs should not be substantially changed. Only very
minor changes should be submitted as amendments. More substantial changes should
be new RFCs, with a note added to the original RFC. Exactly what counts as a
"very minor change" is up to the sub-team to decide. There are some more
specific guidelines in the sub-team RFC guidelines for [PTS changes](standard_changes.md).


## Reviewing RFC's
[Reviewing RFC's]: #reviewing-rfcs

While the RFC pull request is up, the shepherd may schedule meetings with the
author and/or relevant stakeholders to discuss the issues in greater
detail, and in some cases the topic may be discussed at a sub-team
meeting. In either case a summary from the meeting will be
posted back to the RFC pull request.

A sub-team makes final decisions about RFCs after the benefits and drawbacks are
well understood. These decisions can be made at any time, but the sub-team will
regularly issue decisions. When a decision is made, the RFC pull request will
either be merged or closed. In either case, if the reasoning is not clear from
the discussion in thread, the sub-team will add a comment describing the
rationale for the decision.


## Implementing an RFC
[Implementing an RFC]: #implementing-an-rfc

Some accepted RFC's represent vital changes that need to be
implemented right away. Other accepted RFC's can represent changes
that can wait until some arbitrary member feels like doing the
work. Every accepted RFC has an associated issue tracking its
implementation in the relevant repository; thus that associated issue can
be assigned a priority via the triage process that the team uses for
all issues in the relevant repositories.

The author of an RFC is not obligated to implement it. Of course, the
RFC author (like any other member) is welcome to post an
implementation for review after the RFC has been accepted.

If you are interested in working on the implementation for an 'active'
RFC, but cannot determine if someone else is already working on it,
feel free to ask (e.g. by leaving a comment on the associated issue).


## RFC Postponement
[RFC Postponement]: #rfc-postponement

Some RFC pull requests are tagged with the 'postponed' label when they are
closed (as part of the rejection process). An RFC closed with “postponed” is
marked as such because we want neither to think about evaluating the proposal
nor about implementing the described change until some time in the future, and
we believe that we can afford to wait until then to do so. Postponed pull
requests may be re-opened when the time is right. We don't have any formal
process for that, you should ask members of the relevant sub-team.

Usually an RFC pull request marked as “postponed” has already passed
an informal first round of evaluation, namely the round of “do we
think we would ever possibly consider making this change, as outlined
in the RFC pull request, or some semi-obvious variation of it.”  (When
the answer to the latter question is “no”, then the appropriate
response is to close the RFC, not postpone it.)


### Help this is all too informal!
[Help this is all too informal!]: #help-this-is-all-too-informal

The process is intended to be as lightweight as reasonable for the
present circumstances. As usual, we are trying to let the process be
driven by consensus and community norms, not impose more structure than
necessary.

[sub-team]: http://planetary.technology/team.html
