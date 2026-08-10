# Module 3: Knowledge Integration & Context Engine

Module 3 gathers all data that affects an issue,
so later modules have the data they need.

## Inputs

**Structured Issue View**\
from Module 2

**Evidence Submissions**\
from Module 1

**Other Relevant Data**\
For example:

- Ecological data from the FRS.
- Resource availability from the COS.
- Labor Capacity from the COS.
- Fairness constraints from the ITC.
- Historical decisions.

## Outputs

**Context Model**\
Information packet containing:

- Resource requirements and resource availability.
- How much labor is available, when it is available,
  and what skills are required.
- Ecological conditions, fairness considerations, historical precedent.
- Evidence submissions.
- Context score vector.

## Functionality

**Evidence Indexing**\
An organized catalog of evidence is created.

**Context Extraction**\
Ecological, resource, labor, and fairness inputs are pulled from the appropriate subsystem.

**Historical Matching**\
Similar previous cases are identified and matched to a current case.

**Dependency Mapping**\
Required resources external to node identified.

**Context Score Vector**\
The Context Score Vector is a quantification of
ecological, resource, labor, and fairness conditions
identified in the Context Model.
Modules 4-6 test proposals against this.

## Open Questions

### How to Display Data?

How is a codebase intended to automatically display and make meaning from any kind of ecological metric data?
Any different ecological region/system would need different ways to display it,
and its data would be in different forms.
Are we assuming AI can display any data type?

### How is Data Integrated?

How is the ecological data integrated with the resource availability, capacity/ labour data in a meaningful way?
In order to search for the right resources / gain insight on the labour specialization needed,
I imagine OAD would need to be involved.

### Why is the OAD Missing From the Pseudocode?

The OAD is said to be involved in module 3 on page 24 of the white paper,
but it is left out of the pseduocode.
Is this a mistake?

### Where Does Historical Data Come From?

Is the Historical Data and rationale sourced from previous instances of this node (perhaps from module 7?),
or from outside cases where these projects were done.

### Why Isn't the Context Score Vector an Output?

Shouldn't the context score vector be considered an output?
Or, is it technically part of the Context Model?
Or, is it merely symbolic and not actually involved in a module?

### What is "Dependency Mapping"?

What exactly does "dependency mapping" mean?

### How to Manage Too Much Content?

How is content overload prevented/ managed?
