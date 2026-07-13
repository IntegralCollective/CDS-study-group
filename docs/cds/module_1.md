# Module 1: Issue Capture & Signal Intake

All submissions that enter the CDS come in through this module.
It stores the submissions in issues for module 2.

Submissions can be added by an agent,
which can be a person or another Integral system.

## Inputs

**Submission**  
This is added by agents, for example:

- From people:
  - Proposals.
  - Objections.
  - Comments.
- From other Integral systems:
  - Weather data from the FRS.
  - Current value of different types of labor from the ITC.
  - Available resources from the COS.

## Outputs

**Issue**  
These are used by module 2.

## Functionality

### Issues as Bundles of Submissions

Each added submission is put in an issue.
So each issue that this module outputs contains many submissions.

### Authentication

When an agent adds a submission,
the module authenticates the agent.
This ensures that the agent is allowed to add the submission,
and that we know which agent added it.

### Deduplication

If some submission appears to be the same as an existing submission,
the submission is not stored.
Instead, a counter is increased.
This reduces the number of submissions that need to be handled.

## Open Questions

### Where do Issues Come From?

We have been unable to find where issues are created.
