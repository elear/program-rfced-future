---
title: "RFC Editor Model (Version 3)"
abbrev: "RFC Editor Model"
docname: draft-iab-rfcefdp-rfced-model-latest
category: info
obsoletes: RFC8728
updates: RFC7841, RFC8729, RFC8730
ipr: trust200902
area: Internet
keyword: Internet-Draft
stand_alone: yes
pi: [toc, sortrefs, symrefs]

author:
 -
    role: editor
    ins: P. Saint-Andre
    name: Peter Saint-Andre
    organization: Mozilla
    email: stpeter@stpeter.im

normative:

informative:
  I-D.draft-carpenter-rfced-iab-charter:
  RFC2026:
  RFC2418:
  RFC2850:
  RFC5378:
  RFC5620:
  RFC6635:
  RFC7154:
  RFC7322:
  RFC7776:
  RFC7841:
  RFC7991:
  RFC8179:
  RFC8700:
  RFC8711:
  RFC8716:
  RFC8728:
  RFC8729:
  RFC8730:
  RFC8874:
  STYLEGUIDE:
    title: Style Guide
    date: 2021-10-26
    target: https://www.rfc-editor.org/styleguide/
    author:
    - organization: RFC Editor


--- abstract

This document specifies version 3 of the RFC Editor Model. The model defines
two high-level tasks related to the RFC Series. First, policy definition
is the joint responsibility of the RFC Series Working Group (RSWG),
which produces policy proposals, and the RFC Series Approval Board (RSAB),
which approves such proposals. Second, policy implementation
is primarily the responsibility of the RFC Production Center
(RPC) as contractually overseen by the IETF Administration
Limited Liability Company (IETF LLC).

This document obsoletes RFC 8728. This document updates RFC 7841,
RFC 8729, and RFC 8730.

--- middle

# Introduction

The Request for Comments (RFC) Series is the archival series
dedicated to documenting Internet technical specifications,
including general contributions from the Internet research and
engineering community as well as standards documents. RFCs are 
available free of charge to anyone via the Internet. As described
in [RFC8700], RFCs have been published continually since 1969.
The overall framework for the RFC Series and the RFC Editor
function is described in {{RFC8729}} and is updated
by this document.

The processes and organizational models for publication of RFCs
have changed significantly over the years. Most recently, in 2009
{{RFC5620}} defined the RFC Editor Model (Version 1) and in 2012
{{RFC6635}} defined the RFC Editor Model (Version 2), since
modified slightly in 2020 by {{RFC8728}}.

This document reflects experience gained with version 1 and
version 2 of the Model, and therefore describes version 3 of
the Model while remaining consistent with {{RFC8729}}.

In 2020, following meetings led by the RFC Series Editor
in 2019, the IAB formed an open program to conduct a community
discussion and consensus process for the further evolution of
the RFC Editor model. Under the auspices of this program, the
community considered changes that would increase transparency
and community input regarding the definition of policies for
the RFC Series as a whole, while at the same time ensuring the
continuity of the RFC Series, maintaining RFC quality,
maintaining timely processing, ensuring document accessibility,
and clarifying lines of authority and responsibility.

More specifically, in order to ensure sustainable maintenance
and support of the RFC Series based on the principles of expert
implementation, clear management and direction, and appropriate
community input {{RFC8729}}, this document divides the
responsibilities for the RFC Series into two high-level tasks:

1. Policy definition governing the Series as a whole. This is
the joint responsibility of the RFC Series Working Group (RSWG),
which produces policy proposals, and the RFC Series Approval Board (RSAB),
which approves such proposals for publication in the Editorial Stream.

2. Policy implementation through publication of RFCs in all of the streams that form the
Series. This is primarily the responsibility of the RFC Production
Center (RPC) as contractually overseen by the IETF
Administration Limited Liability Company (LLC) {{RFC8711}}.

In this model, RFCs are produced and approved by
multiple document streams. The stream approving body {{RFC8729}} for each stream
is responsible for the content of that stream. The RFC Editor
function is responsible for the packaging and distribution of
all RFCs; specifically, RFCs from all of the streams are
edited and published by the Production Center.

The four streams that now exist are described in {{RFC8729}}.
This document adds a fifth stream, the Editorial Stream.

This document obsoletes {{RFC8728}} by defining version 3 
of the RFC Editor Model. This document updates {{RFC7841}} 
by defining boilerplate text for the Editorial Stream. This 
document updates {{RFC8729}} by replacing the RFC Editor role
with the RSWG, RSAB, and RSCE. This document updates {{RFC8730}}
by removing the dependency on certain policies specified by the
IAB and RSE. More detailed information about changes from 
version 2 of the Model can be found under under {{changes}}.

# Overview of the Model

Version 2 of the RFC Editor Model {{RFC8728}} defined a structure
consisting of the RFC Series Editor, the RFC Production Center, and
the RFC Publisher, with oversight provided by the RFC Series Oversight
Committee (RSOC) on behalf of the Internet Architecture Board (IAB).

By contrast, version 3 of the RFC Editor Model, specified here,
provides a more consensus-oriented framework (similar in some
respects to the structure of technical work within the IETF)
that retains roles for specialized expertise in document
editing and publication.

Policy definition happens within the RFC Series Working Group (RSWG),
which produces policy proposals that are subject to approval by the
RFC Series Approval Board (RSAB), after which such policies are
formally established through publication in the Editorial Stream
within the RFC Series. The RSWG is an open working group (as described
in {{wg}}) that seeks input and participation through a public process
from a wide range of individuals who have an interest in the RFC Series.
The RSAB consists of appointed members who represent the various RFC
streams {{RFC8728}} as well as an expert in technical publishing, the
RFC Series Consulting Editor (RSCE).

Policy implementation is performed by the RFC Production Center (RPC),
as contractually overseen by the IETF Administration Limited Liability
Company (IETF LLC).

In short:

* The RSWG proposes policies that govern the RFC Series as a whole, with
  input from the community, the RSAB, and the RSCE.
* The RSAB considers those proposals and either approves them or returns 
  them to the RSWG, which may make further changes or remove them from
  further consideration.
* If approved, such proposals are published as RFCs in the Editorial
  Stream and thus define the policies to be followed by the RSWG, RSAB,
  RSCE, and RPC.
* The RSCE provides expert advice to the RPC and RSAB on how to implement
  established policies on an ongoing and operational basis, which can include
  raising issues or initiating proposed policy changes within the RSWG.
* The RPC implements the policies defined by the Editorial Stream in its
  day-to-day editing and publication of RFCs from other streams.
* If issues arise with the implementation of particular policies, the RPC
  brings those issues to the RSAB, which interprets the policies and provides
  interim guidance to the RPC, informing the RSWG of those interpretations.

This model is designed to ensure public processes and policy documents,
clear responsibilities and mechanisms for updates and changes to policies
governing the RFC Series as a whole, and effective operational implementation of the
RFC Series, thus meeting the requirements specified in Section 4 of {{RFC8729}}.

The remainder of this document describes the model in greater detail.

# Policy Definition

Policies governing the RFC Series as a whole are defined via open and public 
discussion through proposals that are adopted by and discussed within the RFC
Series Working Group (RSWG), that pass a last call for comments in the
working group and broader community, and that are then approved by the 
RFC Series Approval Board (RSAB).

Policies under the purview of the RSWG and RSAB might include, but are
not limited to, document formats, processes for publication and
dissemination of RFCs, and overall management of the RFC Series.

## Structure and Roles

### RFC Series Working Group (RSWG) {#wg}

#### Purpose

The RFC Series Working Group (RSWG) is the primary venue in which 
members of the community collaborate regarding the policies that 
govern the RFC Series. 

#### Participation

All interested individuals are welcome to participate in the RSWG
(subject to anti-harassment policies as described under {{coc}}). This
includes participants in the IETF and IRTF, IAB and IESG members,
individuals who use RFCs in procurement decisions, authors of RFCs
and Internet-Drafts, developers of tools used to author RFCs, scholarly researchers, and
so on. The IETF LLC Board members, staff, contractors, and the IETF Executive
Director are invited to participate as community members in the RSWG
to the extent permitted by any relevant IETF LLC policies. Members
of the RSAB are also expected to participate actively.

#### Chairs

The RSWG shall have two chairs, one appointed by the IESG and the
other appointed by the IAB. When the RSWG is formed, the chair
appointed by the IESG shall serve for a term of one (1) year and
the chair appointed by the IAB shall serve for a term of two (2)
years; thereafter, chairs shall serve for a term of two (2)
years, with no term limits on renewal. The IESG and IAB shall
determine their own processes for making these appointments.
Community members who have concerns about the performance of an
RSWG chair should direct their feedback to appointing body.
The IESG and IAB shall have the power to remove their
appointed chairs at their discretion at any time, and to name a
replacement who shall serve the remainder of the original chair's
term.

It is the responsibility of the chairs to encourage rough consensus
within the RSWG and to follow that consensus in their decision making,
for instance regarding acceptance of new proposals and advancement of
proposals to the RSAB.

#### Mode of Operation

The intent is that the RSWG shall operate in a way similar to working 
groups in the IETF and research groups in the IRTF. Therefore, all 
RSWG meetings and discussion venues shall be open to all interested 
individuals, and all RSWG contributions shall be subject to intellectual 
property policies, which must be consistent with those of the IETF as 
specified in {{BCP78}} and {{BCP79}}.

The RSWG shall operate by rough consensus, a mode of operation
informally described in {{RFC2418}}.

When the RSWG is formed, all discussions shall take place on an
open email discussion list, which shall be publicly archived. The 
RSWG is also empowered to hold in-person or online meetings. The RSWG 
may also decide by rough consensus to use additional tooling (e.g., 
GitHub as specified in {{RFC8874}}), forms of communication,
and working methods (e.g., design teams) as long as they are 
consistent with {{RFC2418}}.

Absent specific guidance in this document regarding the operation
of the RSWG, the general guidance provided in Section 6 of {{RFC2418}} 
should be considered appropriate.

### RFC Series Approval Board (RSAB)

#### Purpose

The RFC Series Approval Board (RSAB) shall act as the approving body
for proposals generated within the RSWG. The only policy-making role
of the RSAB is to review policy proposals generated by the RSWG; it shall
have no independent authority to formulate policy on its own. It is
expected that the RSAB will respect the rough consensus of the
RSWG wherever possible, without ceding its responsibility to provide
appropriate review of RSWG proposals.

#### Members

The RSAB consists primarily of certain voting members. As specified 
herein, the RSAB also includes certain non-voting members.

The voting members of the RSAB are as follows:

* As the stream representative for the IETF stream, an IESG member
  or other person appointed by the IESG
* As the stream representative for the IAB stream, an IAB member
  or other person appointed by the IAB
* As the stream representative for the IRTF stream, the IRTF chair
  or other person appointed by the IRTF Chair
* As the stream representative for the Independent stream, the
  Independent Submissions Editor (ISE) {{RFC8730}} or other person
  appointed by the ISE
* The RFC Series Consulting Editor, in effect representing the 
  Editorial Stream

If and when a new stream is created, the document that
creates the stream shall specify if a voting member representing
that stream shall also be added to the RSAB, along with any rules
and processes related to that representative (e.g., whether the
representative is a member of the body responsible for the stream
or an appointed delegate thereof). 

To ensure the smooth operation of the RFC Series, the RSAB shall
include the following non-voting, ex-officio members:

* The IETF Executive Director or their delegate as an ex-officio 
  member; the rationale is that the IETF LLC is accountable for 
  implementation of policies governing the RFC Series
* A representative of the RPC, named by the RPC; the rationale
  is that the RPC is responsible for implementation of policies
  governing the RFC Series

In addition to the foregoing, the RSAB may at its discretion include
other non-voting members, whether ex-officio members or liaisons from
groups or organizations with which the RSAB deems it necessary to
formally collaborate or coordinate.

#### Appointment and Removal of Voting Members

The appointing bodies, i.e., the stream approval bodies (IESG, IAB, 
IRTF chair, ISE), shall determine their own processes for 
appointing RSAB members (note that processes related to the RSCE 
are described under {{rsce}}). Each appointing body shall have the power 
to remove its appointed RSAB member at its discretion at any time. 
Appointing bodies should ensure that voting members are seated at 
all times and should fill any vacancies with all due speed, if 
necessary on a temporary basis. 

In the case that the IRTF chair or ISE is incapacitated or otherwise 
unable to appoint another person to serve as a delegate, 
the IAB (as the appointing body for the IRTF chair and ISE 
respectively) shall act as the temporary appointing body for those 
streams and shall appoint a temporary member of the RSAB until the 
IAB has appointed an IRTF chair or ISE, who can then act as an 
RSAB member or appoint a delegate through normal processes.

#### Vacancies

In the case of vacancies by voting members, the RSAB shall operate
as follows:

* Activities related to implementation of policies already in force
  shall continue as normal.
* Voting on approval of policy documents produced by the RSWG shall
  be delayed until the vacancy or vacancies have been filled, up to a
  maximum of 3 months; this clause does not apply to a vacancy of the
  RSCE role, only of the stream representatives enumerated above. If
  during this 3-month period a further vacancy arises, the delay
  should be extended by up to another 3 months. After the delay
  period expires, the RSAB should continue to process
  documents as described below.

#### Chair

The RSAB shall annually choose a chair from among its members using
a method of its choosing.  If the chair position is
vacated during the chair's term, the RSAB chooses a new chair
from among its members.

#### Mode of Operation

The RSAB is expected to operate via email, in-person meetings,
teleconferencing systems, and any additional tooling it deems
necessary.

The RSAB shall keep a public record of its proceedings, including
minutes of all meetings and a record of all decisions.

The RSAB shall announce plans and agendas for their meetings on the
RFC Editor website and by email to the RSWG at least a week before
such meetings. The meetings shall be open for public attendance and
the RSAB may consider allowing open participation. If the RSAB needs
to discuss a confidential matter in executive session, that part of
the meeting shall be private to the RSAB, but must be noted on the
agenda, and must be documented in the minutes with as much detail as
confidentiality requirements permit.

## Process

### Intent

The intent is to provide an open forum by which policies related to the
RFC Series are defined and evolved. The general expectation is that all
interested parties will participate in the RSWG, and that only under
extreme circumstances should RSAB members need to hold "CONCERN"
positions (as described under {{workflow}}).

Because policy issues can be difficult and contentious, RSWG
participants and RSAB members are strongly encouraged to work together
in a spirit of good faith and mutual understanding to achieve rough
consensus (see {{RFC2418}}). In particular, RSWG members are
encouraged to take RSAB concerns seriously, and RSAB members are
encouraged to clearly express their concerns early in the process and
to be responsive to the community. All parties are encouraged to respect
the value of each stream and the long-term health and viability of
the RFC Series.

This process is intended to be one of continuous consultation. RSAB
members should consult with their constituent stakeholders (e.g.,
authors, editors, tool developers, and consumers of RFCs) on an ongoing
basis, so that when the time comes to consider the approval of a proposal, there should
be no surprises. Appointing bodies are expected to establish whatever
processes they deem appropriate to facilitate this goal.

### Workflow {#workflow}

The following process shall be used to formulate or modify processes
related to the RFC Series:

1. An individual or set of individuals generates a proposal in the form 
   of an Internet-Draft (which must be submitted in full conformance
   with the provisions of {{BCP78}} and {{BCP79}}
   and asks the RSWG to adopt the proposal as a working group item.

2. If by following working group procedures for rough consensus the chairs determine
   that there is sufficient interest in the proposal, the RSWG may
   adopt the proposal as a draft proposal of the RSWG, in much the
   same way a working group of the IETF or research group of the IRTF
   would (see {{RFC2418}}).

3. The RSWG shall then further discuss and develop the proposal. All
   participants, but especially RSAB members, should pay special
   attention to any aspects of the proposal that have the potential
   to significantly modify policies of long standing or historical
   characteristics of the Series as described under {{properties}}.
   Members of the RSAB are expected to participate as individuals in 
   all discussions relating to RSWG proposals so that they are fully 
   aware of proposals early in the policy definition process, and so 
   that any issues or concerns that they have will be raised during 
   the development of the proposal, not left until the RSAB review 
   period. The RSWG chairs are also expected to participate as 
   individuals.

4. At some point, if the RSWG chairs believe there may be rough
   consensus for the proposal to advance, they will issue a last call
   for comment within the working group.

5. After a comment period of suitable length, the RSWG chairs will
   determine whether rough consensus for the proposal exists (taking
   their own feedback as individuals into account along with feedback
   from other participants). If comments have been received and
   substantial changes have been made, additional last calls may be
   necessary. Once the chairs determine that consensus has been 
   reached, they shall announce their determination on the RSWG
   discussion list and forward the document to the RSAB.

6. Once consensus is established in the RSWG, the RSAB shall issue a
   community call for comments as further described under {{cfc}}. If 
   substantial comments are received in response to the community 
   call for comments, the RSAB may return the draft to the RSWG to 
   consider those comments and make revisions to address the feedback
   received. In parallel with the community call for comment, the RSAB
   shall also consider the proposal.

7. If the scope of revisions made in the previous step is large, an 
   additional community call for comment should be issued by the RSAB, 
   and the feedback received should be considered by the RSWG.

8. Once the RSWG chairs confirm that concerns received during the
   community call(s) for comment have been addressed, they shall
   inform the RSAB that the document is ready for balloting by the
   RSAB.

9. Within a reasonable period of time, the RSAB will then poll among
   its members regarding the proposal. Positions may be as follows:

   * "YES": the proposal should be approved
   * "CONCERN": the proposal raises substantial concerns that must be
     addressed
   * "RECUSE": the person holding the position has a conflict of
     interest

Any RSAB member holding a "CONCERN" position must explain their concern
to the community in detail. The explanation might or might not be actionable.

A position of CONCERN may be filed for several reasons:

   * The proposal represents a serious problem for one or more of 
     the individual streams.
   * The RSAB member believes that the proposal would cause serious harm
     to the overall Series, including harm to the long-term health and
     viability of the Series.
   * Comments received during a community call for comment need
     to be addressed, as described under {{cfc}}.

Because RSAB members are expected to participate in the discussions 
within the RSWG and to raise any concerns and issues during those 
discussions, most CONCERN positions should not come as a surprise to 
the RSWG. Notwithstanding, late CONCERN positions are always possible
if issues are identified during RSAB review or the community call for comment.

10. If a CONCERN exists, discussion will take place within the RSWG.
    Again, all RSAB members are expected to participate. If substantial 
    changes are made in order to address CONCERN positions, an additional 
    community call for comment might be needed.

11. A proposal without any CONCERN positions is approved. 

12. If, after a suitable period of time, any CONCERN positions remain,
    a vote of the RSAB is taken. If at least three voting members vote
    YES, the proposal is approved.

13. If the proposal is not approved, it is returned to the RSWG. The RSWG 
    can then consider making further changes.

14. If the proposal is approved, a notification is sent to the community,
    and the document enters the queue for publication as an RFC within
    the Editorial Stream.

15. Policies may take effect immediately upon approval by the RSAB and 
    before publication of the relevant RFC, unless the IETF LLC objects 
    pending resolution of resource or contract issues.

### Community Calls for Comment {#cfc}

The RSAB is responsible for initiating and managing community calls
for comment on proposals that have gained consensus within the RSWG.
The RSAB should actively seek a wide range of input. The RSAB seeks
such input by, at a minimum, sending a notice to the rfc-interest
mailing list or to its successor or future equivalent. RSAB members
should also send a notice to the communities they directly represent
(e.g., the IETF and IRTF). Notices are also to be made available and
archived on the RFC Editor website. In addition, other communication
channels can be established for notices (e.g., via an RSS feed or by
posting to social media venues).

In cases where a proposal has the potential to significantly modify
policies of long standing or historical characteristics of the
Series as described under {{properties}}, the RSAB should take extra care to reach out to even broader
communities that make use of RFCs, such as scholarly researchers,
procurement managers, and standards development organizations. The
RSAB should work with the stream representatives and the IETF LLC
to identify and establish contacts in such communities, assisted 
in particular by the RSCE.

A notice of a community call for comment contains the following:

*  A subject line beginning with 'Call for Comment:'

*  A clear, concise summary of the proposal

*  A URL to the Internet-Draft that defines the proposal

*  Any commentary or questions for the community that the RSAB deems
   necessary (using their usual decision-making procedures)

*  Clear instructions on how to provide public comments

*  A deadline for comments

A comment period will last not less than two weeks and should be
longer if wide outreach is required. Comments will be publicly
archived on the RFC Editor website.

The RSAB is responsible for considering comments received during 
a community call for comment. If RSAB members conclude that such
comments raise important issues that should be addressed, they 
should do so by discussing those issues within the RSWG or lodging 
a position of "CONCERN" during RSAB balloting.

### Appeals

Appeals of RSWG chair decisions shall be made to the RSAB. Decisions of the
RSWG charis can be appealed only on grounds of failure to follow the correct
process. Appeals should be made within thirty (30) days of any action, or in
the case of failure to act, of notice having been given to the RSWG.
The RSAB will then decide if the process was followed and will direct
the RSWG chairs as to what procedural actions are required.

Decisions of the RSAB can be appealed on grounds of failure to follow 
the correct process. Where the RSAB makes a decision in order to resolve 
a disagreement between authors and the RPC (as described under {{disagreements}}), appeals can 
be filed on the basis that the RSAB misinterpreted an approved policy. 
In other cases, disagreements about the conduct of the RSAB are not 
subject to appeal. Appeals of RSAB decisions shall be made to the IAB 
and should be made within thirty (30) days of public notice of the 
relevant RSAB decision (typically, when minutes are posted). The IAB 
shall decide whether a process failure occurred and what if any 
corrective action should take place.

### Anti-Harassment Policy {#coc}

The [IETF anti-harassment policy](https://www.ietf.org/about/groups/iesg/statements/anti-harassment-policy/) also applies to the RSWG and RSAB,
which strive to create and maintain an environment in which people
of many different backgrounds are treated with dignity, decency,
and respect. Participants are expected to behave according to
professional standards and to demonstrate appropriate workplace
behavior. For further information about these policies, see
{{RFC7154}}, {{RFC7776}}, and {{RFC8716}}.

### RFC Boilerplates

As part of the RFC Style Guide (see {{RFC7322}} and {{STYLEGUIDE}}),
new or modified RFC boilerplates (see {{RFC7841}}) considered under
version 3 of the RFC Editor Model must be approved by the following
parties, each of which has a separate area of responsibility with
respect to boilerplates:

* Each stream to which the boilerplate applies, which approves that
  the boilerplate meets its needs
* The RSAB, which approves that the boilerplate is not in conflict with
  the boilerplate used in the other streams
* The RPC, which approves that the language of the boilerplate conforms
  to the RFC Style Guide
* The IETF Trust, which approves that the boilerplate correctly states
  the Trust's position regarding rights and ownership

# Policy Implementation

## Roles and Processes

Publication of RFCs is handled by the RFC Production Center (RPC).

A few general considerations apply:

* The general roles and responsibilities of the RPC are defined by
  RFCs published in the Editorial Stream (i.e., not directly by the
  RSWG, RSAB, or RSCE), by legacy RFCs which apply to the 
  RPC and which have not yet been superseded by Editorial Stream 
  RFCs, and by the requisite contracts.

* The RPC is advised by the RSCE and RSAB, and has a duty to
  consult with them under specific circumstances, such as those
  relating to disagreements between authors and the RPC.

* The RPC is overseen by the IETF LLC to ensure that
  it performs in accordance with contracts in place.

All matters of budget, timetable, and impact on its performance
targets, are between the RPC and IETF LLC.

The RPC shall regularly provide reports to the IETF LLC, RSAB, RSWG,
and broader community regarding its activities and any key risks or
issues affecting it.

In the event that the RPC is required to make a decision without
consultation that would normally deserve consultation, or makes a
decision against the advice of the RSAB, the RPC must notify the
RSAB.

This document does not specify the exact relationship between the
IETF LLC and the RPC; for example, the work of the RPC could be
performed by a separate corporate entity under contract to the
IETF LLC, it could be performed by employees of the IETF LLC, or
the IETF LLC could engage with independent contractors for some or
all aspects of such work. The exact relationship is a matter for
the IETF LLC to determine.

The IETF LLC is responsible for the method of and management of the
engagement of the RPC. Therefore, the IETF LLC has authority over
negotiating performance targets for the RPC and also has responsibility
for ensuring that those targets are met. Such performance targets 
are set based on the RPC's publication load and additional efforts 
required by policies specified in the Editorial Stream, in legacy RFCs 
which apply to the RPC and which have not yet been superseded by 
Editorial Stream RFCs, and in the requisite contracts. The IETF LLC may 
consult with the community regarding these targets. The IETF LLC is 
empowered to appoint a manager or to convene a committee to complete 
these activities.

If individuals or groups within the community have concerns about the
performance of the RPC, they can request that the matter be investigated
by the IETF LLC board, the IETF LLC Executive Director, or a point of 
contact designated by the IETF LLC Board. Even if the IETF LLC opts to 
delegate this activity, concerns should be raised with the IETF LLC. 
The IETF LLC is ultimately answerable to the community via the mechanisms 
outlined in its charter.

## Working Practices

In the absence of a high-level policy documented in an RFC, or to specify the
detail of its implementation, the RPC can 
document working practices regarding the editorial preparation
and final publication and dissemination of RFCs. Examples include:

* Maintenance of a style guide that defines editorial standards to which
  RFCs must adhere (see the
  [style guide web page](https://www.rfc-editor.org/styleguide/), which 
  extends {{RFC7322}}).

* Instructions regarding the file formats that are accepted as input to the
  editing and publication process.

* Guidelines regarding the final structure and layout of published documents.
  In the context of the XML vocabulary ({{RFC7991}}), such guidelines could
  include clarifications regarding the preferred XML elements and attributes used to
  capture the semantic content of RFCs.

## RPC Responsibilities {#rpc}

The core responsibility of the RPC is the implementation of RFC Series 
policies through publication of RFCs (including the dimensions of document
quality, timeliness of production, and accessibility of results), while
taking into account issues raised by the community through the RSWG and
by the stream approving bodies. More specifically, the RPC's responsibilities
at the time of writing include the following:

1. Editing inputs from all RFC streams to comply with the RFC Style Guide.

2. Creating and preserving records of edits performed on documents.

3. Identifying where editorial changes might have technical impact
   and seeking necessary clarification.

4. Engaging in dialogue with authors, document shepherds, IANA, or
   stream-specific contacts (e.g., working group chairs and stream
   approving bodies) when clarification is needed.

5. Creating and preserving records of dialogue with document authors.

6. Requesting advice from the RSAB and RSCE as needed.

7. Providing suggestions to the RSAB and RSCE as needed.

8. Participating within the RSWG in the creation of new Editorial Stream RFCs that
   impact the RPC, at least in an advisory capacity.

9. Providing reports to the community on its performance and plans.

10. Consulting with the community on its plans.

11. Negotiating its specific plans and resources with the IETF LLC.

12. Providing sufficient resources to support reviews of RPC
    performance by the IETF LLC.

13. Coordinating with IANA to ensure correct documentation of
    IANA-performed protocol registry actions.

14. Assigning RFC numbers.

15. Establishing publication readiness of each document through
    communication with the authors, document shepherds, IANA, or
    stream-specific contacts, and, if needed, with the RSAB and RSCE.

16. Liaising with stream approving bodies and other representatives of the
    streams as needed.

17. Publishing RFCs, which includes:

    * depositing copies on the RFC Editor site both individually and in collections
    * depositing copies with external archives
    * creating catalogs and catalog entries
    * announcing the publication to interested parties

18. Providing online access to RFCs.

19. Providing an online system to submit RFC Errata.

20. Providing online access to approved RFC Errata.

21. Providing backups.

22. Providing storage and preservation of records.

23. Authenticating RFCs for legal proceedings.

## Resolution of Disagreements between Authors and the RPC {#disagreements}

During the process of editorial preparation and publication, disagreements
can arise between the authors of an RFC-to-be and the RPC. Where an existing
policy clearly applies, typically such disagreements are handled in a
straightforward manner through direct consultation between the authors and
the RPC, sometimes in collaboration with other individuals such as a document
shepherd, IETF working group chair, IRTF research group chair, or IETF Area
Director.

However, if it is unclear whether an existing policy applies, or if it is 
unclear how to interprete an existing policy, the parties may need to
consult with additional individuals or bodies (e.g., RSAB, IESG, IRSG, or
stream approving bodies) to help achieve a resolution. The following points are
intended to provide more specific guidance.

* If there is a conflict with a policy for a particular stream, the
  RPC should consult with the relevant stream approving body to help achieve a
  resolution, if needed also conferring with a per-stream body such as the
  IESG or IRSG.

* If there is a conflict with a cross-stream policy, the RPC should consult
  with the RSAB to achieve a resolution.

* The disagreement might raise a new issue that is not covered by an existing
  policy or that cannot be resolved through consultation between the RPC and
  other relevant individuals and bodies, as described above. In this case,
  the RSAB is responsible for (a) resolving the disagreement in a timely manner
  if necessary before a new policy is defined and (b) bringing the issue to
  the RSWG so that a new policy can be defined.

## Point of Contact

From time to time, individuals or organizations external to the IETF and
the broader RFC Series community may have questions about the RFC Series.
Such inquiries should be directed to the
[rfc-editor@rfc-editor.org](mailto:rfc-editor@rfc-editor.org) email
alias or to its successor or future equivalent and then handled by the 
appropriate bodies (e.g., RSAB, RPC) or individuals (e.g., RSWG chairs, RSCE).

## Administrative Implementation

The exact implementation of the administrative and contractual
activities described here are a responsibility of the IETF LLC. This
section provides general guidance regarding several aspects of such
activities.

### Vendor Selection for the RFC Production Center

Vendor selection is done in cooperation with the streams and
under the final authority of the IETF LLC.

The IETF LLC develops the work definition (the Statement of Work)
for the RPC and manages the vendor selection process.  The work
definition is created within the IETF LLC budget and takes into
account the RPC responsibilities (as described under {{rpc}}), 
the needs of the streams, and community input.

The process to select and contract for an RFC Production Center
and other RFC-related services is as follows:

*  The IETF LLC establishes the contract process, including the steps
   necessary to issue an RFP when necessary, the timing, and the
   contracting procedures.

*  The IETF LLC establishes a selection committee, which will
   consist of the IETF Executive Director and other
   members selected by the IETF LLC in consultation with the
   stream approving bodies. The committee shall select a chair from
   among its members.

*  The selection committee selects the vendor, subject to the
   successful negotiation of a contract approved by the IETF LLC.  In
   the event that a contract cannot be signed, the matter shall be
   referred to the selection committee for further action.

### Budget

The expenses discussed in this document are not new expenses. They
have been and remain part of the IETF LLC budget.

The RFC Series portion of the IETF LLC budget shall include funding
to support the RSCE, the RFC Production Center, and the Independent
Stream.

The IETF LLC has the responsibility to approve the total RFC Editor
budget (and the authority to deny it). All relevant parties must work
within the IETF LLC budgetary process.

# RFC Series Consulting Editor (RSCE) {#rsce}

The RFC Series Consulting Editor (RSCE) is a senior technical
publishing professional who will apply their deep knowledge of
technical publishing processes to the RFC Series.

The primary responsibilities of the RSCE are as follows:

* Serve as a voting member on the RSAB
* Identify problems with the RFC publication process and
  opportunities for improvement
* Provide expert advice within the RSWG regarding policy proposals
* Provide expert advice to the RPC and IETF LLC

Matters on which the RSCE might provide guidance could include the
following (see also Section 4 of {{RFC8729}}):

* Editing, processing, and publication of RFCs
* Publication formats for the RFC Series
* Changes to the RFC style guide
* Series-wide guidelines regarding document content and quality
* Web presence for the RFC Series
* Copyright matters related to the RFC Series
* Archiving, indexing, and accessibility of RFCs

The IETF LLC is responsible for the method of and management of the
engagement of the RSCE, including selection, evaluation, and the timely
filling of any vacancy. Therefore, whether the RSCE role is structured
as a contractual or employee relationship is a matter for the IETF LLC
to determine.

## RSCE Selection

The IETF LLC will form a selection committee, including members
from the community, that will be responsible for making a
recommendation to the IETF LLC for the RSCE role. The selection
committee will take into account the definition of the role
as well as any other information that the committee deems
necessary or helpful in making its decision. The IETF LLC is
responsible for contracting or employment of the RSCE.

## RSCE Performance Evaluation

Periodically, the IETF LLC will evaluate the performance of the 
RSCE, including a call for confidential input from the community. 
The IETF LLC will produce a draft evaluation of the RSCE's 
performance for review by RSAB members other than the RSCE, 
who will provide feedback to the IETF LLC.

## Temporary RSCE Appointment

In the case that the currently appointed RSCE is expected to be 
unavailable for an extended period, the IETF LLC may appoint a 
Temporary RSCE through whatever recruitment process it considers 
appropriate. A Temporary RSCE acts as the RSCE in all aspects 
during their term of appointment.

## Conflict of Interest

The RSCE is expected to avoid even the appearance of conflict of
interest or judgment in performing their role.  To ensure this, the
RSCE will be subject to a conflict of interest policy established by
the IETF LLC.

The RPC service provider may contract services from the RSCE service 
provider, and vice versa, including for services provided to the IETF 
LLC.  All contracts between the two must be disclosed to the IETF LLC.  
Where those services are related to services provided to the IETF LLC, 
IETF LLC policies shall apply, including publication of relevant parts 
of the contract.

# Editorial Stream

This document creates the Editorial Stream as separate space for
publication of policies, procedures, guidelines, rules, and related
information regarding the RFC Series as a whole.

The Editorial Stream will be used only to specify and update policies,
procedures, guidelines, rules, and related information regarding the
RFC Series as a whole; no other use of the Editorial Stream is authorized
by this memo and no other streams are so authorized. This policy may be
changed only by agreement of the IAB, IESG, and IETF LLC.

All documents produced by the RSWG and approved by the RSAB shall be
published as RFCs in the Editorial Stream with a status of Informational.
(Note that the Editorial Stream is not authorized to publish RFCs that
are Standards Track or Best Current Practice, since such RFCs are
reserved to the IETF Stream {{RFC8729}}.)

The requirements and process for creating any additional RFC streams are
outside the scope of this document.

## Procedures Request of the IETF Trust

The IAB requests that the IETF Trust and its Trustees assist in
meeting the goals and procedures set forth in this document.

The Trustees are requested to publicly confirm their willingness and
ability to accept responsibility for the Intellectual Property Rights
for the Editorial Stream.

Specifically, the Trustees are asked to develop the necessary
boilerplate to enable the suitable marking of documents so that the
IETF Trust receives the rights as specified in {{RFC5378}}.  These
procedures need to also allow authors to indicate either no rights to
make derivative works, or preferentially, the right to make unlimited
derivative works from the documents.  It is left to the Trust to
specify exactly how this shall be clearly indicated in each document.

## Patent and Trademark Rules for the Editorial Stream

As specified above, contributors of documents for the Editorial Stream 
are expected to use the IETF Internet-Draft process, complying therein
with the rules specified in the latest version of {{BCP9}}. This includes 
the disclosure of Patent and Trademark issues that are known, or can be
reasonably expected to be known, to the contributor.

Disclosure of license terms for patents is also requested, as
specified in the most recent version of {{BCP79}}. The Editorial 
Stream has chosen to use the IETF's IPR disclosure mechanism,
https://www.ietf.org/ipr/, for this purpose.  The IAB would prefer that
the most liberal terms possible be made available for Editorial Stream 
documents. Terms that do not require fees or licensing are preferable.  
Non-discriminatory terms are strongly preferred over those that
discriminate among users.  However, although disclosure is required
and the RSWG and the RSAB may consider disclosures and terms in making 
a decision as to whether to submit a document for publication, there 
are no specific requirements on the licensing terms for intellectual
property related to Editorial Stream publication.

## Editorial Stream Boilerplate

This document specifies the following text for the "Status of This Memo"
section of RFCs published in the Editorial Stream. Any changes to this
boilerplate must be made through the RFC Series Policy Definition process
specified in this document.

Because all Editorial Stream RFCs have a status of Informational,
the first paragraph of the "Status of This Memo" section shall be
as specified in Appendix A.2.1 of {{RFC7841}}.

The second paragraph of the "Status of This Memo" section shall be
as follows:

> This document is a product of the RFC Series Policy Definition process.
> It represents the consensus of the RFC Series Working Group approved by
> the RFC Series Approval Board. Such documents are not candidates for any
> level of Internet Standard; see Section 2 of RFC 7841.

The third paragraph of the "Status of This Memo" section shall be
as specified in Section 3.5 of {{RFC7841}}.

# Historical Properties of the RFC Series {#properties}

This section lists some of the properties that have been 
historically regarded as important to the RFC Series. Proposals 
that affect these properties are possible within the processes 
defined in this document. As described under {{workflow}} and {{cfc}},
proposals that might have a detrimental effect on these properties
should receive heightened scrutiny during RSWG discussion and RSAB 
review. The purpose of this scrutiny is to ensure that all changes are 
deliberate and that the consequences of a proposal, as far as they can be
identified, have been carefully considered.

## Availability

Documents in the RFC Series have been available for many decades, 
with no restrictions on access or distribution.

## Accessibility

RFC Series documents have been published in a format that was intended 
to be as accessible as possible to those with special needs, e.g., for 
those with impaired sight.

## Language

All existing RFC Series documents have been published in English. 
However, since the beginning of the RFC series, documents have been
published under terms that explicitly allow translation into 
languages other than English without asking for permission.

## Diversity

The RFC series has included many types of documents including standards for
the Internet, procedural and informational documents, thought experiments,
speculative ideas, research papers, histories, humor, and even eulogies.

## Quality

RFC Series documents have been reviewed for subject matter quality and 
edited by professionals with a goal of ensuring that documents are clear, 
consistent, and readable {{RFC7322}}.

## Stability

Once published, RFC Series documents have not changed.

## Longevity

RFC Series documents have been published in a form intended to be 
comprehensible to humans for decades or longer.

# Changes from Version 2 of the RFC Editor Model {#changes}

## RFC Editor Function

Several responsibilities previously assigned to the "RFC Editor"
or, more precisely, the "RFC Editor function" are now performed
by the RSWG, RSAB, RPC, and IETF LLC (alone or in combination).
These include various aspects of strategic leadership 
(Section 2.1.1 of {{RFC8728}}), representation of the RFC Series 
(Section 2.1.2 of {{RFC8728}}), development of RFC production and
publication (Section 2.1.3 of {{RFC8728}}), development of the
RFC Series (Section 2.1.4 of {{RFC8728}}), operational oversight
(Section 3.3 of {{RFC8729}}), policy oversight 
(Section 3.4 of {{RFC8729}}), the editing, processing, and publication of
documents (Section 4.2 of {{RFC8729}}), and development and
maintenance of Series-wide guidelines and rules 
(Section 4.4 of {{RFC8729}}). Among other things this changes the dependency on
the RSE included in Section 2.2 of {{RFC8730}} with regard to 
"coordinating work and conforming to general RFC Series policies
as specified by the IAB and RSE." In addition, various details 
regarding these responsibilities have been modified to accord with 
the new framework defined in this document.

## RFC Series Editor

Implied by the changes outlined in the previous section, the
responsibilities of the RFC Series Editor (RSE) as a person or
role (contrasted with the overall "RFC Editor function") are now
split or shared among the RSWG, RSAB, RPC, and IETF LLC (alone
or in combination). More specifically, the responsibilities of
the RFC Series Consulting Editor (RSCE) under version 3 of the RFC
Editor Model differ in many ways from the responsibilities of the
RFC Series Editor under version 2 of the Model. In general,
references in existing documents to the RSE can be taken as
referring to the "RFC Editor function" as described herein, but
should not be taken as referring to the RSCE.

## RFC Publisher

In practice the RFC Production Center (RPC) and RFC Publisher roles
have been performed by the same entity and this practice is expected
to continue; therefore this document dispenses with the distinction
between these roles and refers only to the RPC.

## IAB

Under earlier versions of the RFC Editor Model, the IAB was
responsible for oversight of the RFC Series and acted as a body
for final conflict resolution regarding the Series. The IAB's
authority in these matters is described in the IAB's charter
({{RFC2850}} as updated by {{I-D.draft-carpenter-rfced-iab-charter}}).
Under version 2 of the Model, the IAB delegated some
of its authority to the RFC Series Oversight Committee (see {{rsoc}}).
Under version 3 of the Model, authority for policy definition
resides with the RSWG as an independent venue for work by members
of the community (with approval of policy proposals as the
responsibility of the RSAB, representing the streams and including 
the RSCE), whereas authority for policy implementation resides with
the IETF LLC.

## RFC Series Oversight Committee (RSOC) {#rsoc}

In practice, the relationships and lines of authority and responsibility
between the IAB, RSOC, and RSE have proved unwieldy and somewhat opaque.
To overcome some of these issues, this document dispenses with the RSOC.
References to the RSOC in documents such as {{RFC8730}} are obsolete
because this document disbands the RSOC.

## RFC Series Advisory Group (RSAG)

Version 1 of the RFC Editor Model {{RFC5620}} specified the existence of
the RFC Series Advisory Group (RSAG), which was no longer specified in
version 2 of the Model. For the avoidance of doubt, this document affirms
that the RSAG has been disbanded.  (This is not to be confused with the
RFC Series Approval Board (RSA>B<), which this document establishes.)

## Editorial Stream

This document creates the Editorial Stream in addition to the streams
already described in {{RFC8729}}.

# Security Considerations

The same security considerations as those in {{RFC8729}} apply.
The processes for the publication of documents must prevent the
introduction of unapproved changes. Since the RFC Editor maintains
the index of publications, sufficient security must be in place to
prevent these published documents from being changed by external
parties. The archive of RFC documents, any source documents needed
to recreate the RFC documents, and any associated original documents
(such as lists of errata, tools, and, for some early items, originals
that are not machine-readable) need to be secured against
data storage failure.

The IETF LLC should take these security considerations into account
during the implementation and enforcement of any relevant contracts.

# IANA Considerations

This document places responsibility for coordination of registry
value assignments with the RPC. The IETF LLC facilitates management
of the relationship between the RPC and IANA.

This document does not create a new registry nor does it register any
values in existing registries, and no IANA action is required.

--- back

# Acknowledgments
{:numbered="false"}

Portions of this document were borrowed from {{RFC5620}},
{{RFC6635}}, {{RFC8728}}, {{RFC8729}}, the Frequently Asked 
Questions of the IETF Trust, and earlier proposals
submitted within the IAB's RFC Editor Future Development Program
by Martin Thomson, Brian Carpenter, and Michael StJohns. Thanks
to Eliot Lear and Brian Rosen in their role as chairs of the Program
for their leadership and assistance. Thanks also for feedback and
proposed text to
Jari Arkko,
Sarah Banks,
Carsten Bormann,
Scott Bradner,
Nevil Brownlee,
Ben Campbell,
Jay Daley,
Martin Duerst,
Lars Eggert,
Adrian Farrel,
Stephen Farrell,
Sandy Ginoza,
Bron Gondwana,
Joel Halpern,
Wes Hardaker,
Bob Hinden,
Russ Housley,
Christian Huitema,
Ole Jacobsen,
John Klensin,
Mirja Kuehlewind,
Ted Lemon,
John Levine,
Lucy Lynch,
Andrew Malis,
Larry Masinter,
S. Moonesamy,
Mark Nottingham,
Tommy Pauly,
Colin Perkins,
Julian Reschke,
Eric Rescorla,
Adam Roach,
Alice Russo,
Doug Royer,
Rich Salz,
Tim Wicinski,
and Nico Williams.
