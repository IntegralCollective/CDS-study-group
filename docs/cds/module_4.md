# Module 4: Norms & Constraint Checking

## Inputs

- ContextModel
- StructuredIssueView
- candidate Scenario
- formal rules from FRS, COS, ITC, CDS policy, OAD standards

## Outputs:

- ConstraintReport
- pass/fail by constraint domain
- required modifications
- feasible/revisable scenario set

## Functionality: 

Test candidate scenarios against boundaries: ecological ceilings, resources, labor, fairness/accessibility, safety, node constitution, and federated rules.

Handoff: Module 4 passes feasible or revisable scenarios to Module 5.

## New Additions/ Comments

Strenghts:

- Returns modification requirements instead of silent rejection.
- Correctly treats CDS as normative authority while other systems provide reasons for constraints.

Minimum viable version:
Shadow version placeholder/ Possible facilitator checklist

- ecological red flags
- material availability
- labor capacity
- accessibility/fairness
- safety/legal/constitutional constraints
- certification/design dependency
- FRS monitoring requirement
- Other important fields

## Open questions: 

- If no scenario is passed on to Module 5, what signal is sent where? 
e.g. it sends issue back to bridge step “scenario generation” or Module 2 or ... ?
- Constraint rules may be incomplete, outdated, or illegitimate. How is this managed?
- Quantifiable constraints may dominate non-quantifiable social values. How is ensured that social values are not cut off?
- Module 4 depends on candidate scenarios, but scenario generation is not fully specified in the module sequence.
- What process comes up with constraint rule?
- What is the distinction between the "formal" rules/constraints and the context model from module 3? Both are inputs for module 4, but they almost seem redundant. In my mind, the context model is a data packet of conditions, which are, in effect, constraints. Maybe they function as two separate layers of constraints? (samw)
