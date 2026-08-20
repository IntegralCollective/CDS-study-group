
# Module 5: Participatory Deliberation Workspace

Module 5 is where the community actually thinks.
- It provides a structured deliberation environment:
	- Where *ideas* are clarified, misunderstandings resolved.
	- Where *objections* are aggregated.
	- Where *scenarios* are modified.
	- Where *constraint reports* are interpreted.
	- Where cooperation emerges organically.
	- Where the *output* is refined, so that Module 6 can evaluate *agreements* reached.

[White Paper p.48]

## Inputs

- *StructuredIssueView* (from Module 2)
- *ContextModel* (from Module 3)
- *ConstraintReport* (from Module 4)
- *Submissions* and *revisions* from *participants*
- Optional *mediation signals* (e.g., from facilitators or *CDS norms engine*)
- [White Paper p.46]

## Outputs

- A refined set of scenarios or scenario variants
- A consolidated objections list
- *Gradient preference signal*, not a binary ballot. [WP.31,33]
- A structured dataset ready for weighted consensus in Module 6
- Updated issue lifecycle state
- [WP.46]
  
## Process

Participants explore *structured issues* using tools for:
- objection mapping
- semantic discussion threads
- scenario comparison
- preference gradients
- pros/cons visualization

Deliberation is non-coercive and fully transparent. *Arguments* evolve in public view, and *objections* are treated as information — not obstacles.
This module ensures that disagreement becomes productive rather than adversarial.
- [White Paper p.24]

## Questions

- The *Gradient preference signal* is not expressly associated with any particular CDS Module?
- Maybe it is referenced in CDS Module 1 "preference gradients", "conditional approvals",
- input in *Submissions* and "micro-surveys", used in Module 5 and processed in module 6?
- [WP.23] [GaryRKent]

## Comments

- CDS Module 5* is *deferred* from the *Minimum Viable System(MVS)* build. [DevGuide PDF p.15]
- Note:  Module 5 does not decide. It outputs a clean, consensus-ready deliberation state for Module 6.
- [WP.47]
- The *gradient preference signal* is implied in the pseudo-code among the "Core CDS enums / literals" defined
- for *Supportlevel* [WP.31] and the "foundational entity" defined as *Vote* [WP.33].
- The *Signal* is likely an integrating deliberative process that spans multiple CDS Modules.
- The implication is that the CDS Mudule 5 process is not a "secret-star-chamber" process but instead a truly
- open grassroots democratic process that may at times engage the entire node community.
- At certain stages of deliberation, all node participants might be asked to participate, surveyed,
- both to offer Scenario proposals and Scenario preferences. Module 6 then assesses the feedback
- and would determine the next stage in the deliberative process. It's actually quite brilliant!
- [GaryRKent]
