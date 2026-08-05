# Module 3: Knowledge Integration & Context Engine

Module 3 aggregates data from other modules, other subsystems, and external datasets
in order to determine the conditions that surround an issue
and potentially constrain enaction of an issue's scenarios.

## Inputs

**Structured Issue View**\
from Module 2

**Evidence in Support of Scenarios**\
from Module 1

**Ecological Data**\
from FRS

**Resource Availability**\
from COS

**Labor Capacity**\
from COS

**Fairness Constraints**\
from ITC

**Historical Precedent**

**Relevant External Data**

## Outputs

**Context Model**\
Organized packet of information containing:
resource requirements and resource availability,
labor requirements and labor capacity,
ecological conditions, fairness considerations, historical precedent,
evidence in support of scenarios, and context score vector.

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

How is a codebase intended to automatically display and make meaning from any kind of ecological metric data?
Any different ecological region/system would need different ways to display it,
and its data would be in different forms.
Are we assuming AI can display any data type?

How is the ecological data integrated with the resource availability, capacity/ labour data in a meaningful way?
In order to search for the right resources / gain insight on the labour specialization needed,
I imagine OAD would need to be involved.

The OAD is said to be involved in module 3 on page 24 of the white paper,
but it is left out of the pseduocode.
Is this a mistake?

Is the Historical Data and rationale sourced from previous instances of this node (perhaps from module 7?),
or from outside cases where these projects were done.

Shouldn't the context score vector be considered an output?
Or, is it technically part of the Context Model?
Or, is it merely symbolic and not actually involved in a module?

What exactly does "dependency mapping" mean?

How is content overload prevented/ managed?
