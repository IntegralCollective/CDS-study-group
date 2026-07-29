# Module 4: Norms & Constraint Checking

Function: Test candidate scenarios against boundaries: ecological ceilings, resources, labor, fairness/accessibility, safety, node constitution, and federated rules.

Inputs:

- ContextModel
- StructuredIssueView
- candidate Scenario 
- formal rules from FRS, COS, ITC, CDS policy, OAD standards

Outputs:

- ConstraintReport
- pass/fail by constraint domain
- required modifications
- feasible/revisable scenario set
- issue status: constrained

Handoff: Module 4 passes feasible or revisable scenarios to Module 5. If all fail, it sends issue? back to bridge step “scenario generation” or Module 2 or?

Strengths:

- Makes constraints explicit rather than political.
- Returns modification requirements instead of silent rejection.
- Correctly treats CDS as normative authority while other systems provide constraints.
- Strong candidate for rule-engine implementation later.

Failure modes:

- Constraint rules may be incomplete, outdated, or illegitimate.
- Quantifiable constraints may dominate non-quantifiable social values.
- Module 4 depends on candidate scenarios, but scenario generation is not fully specified in the module sequence.

Critique:

- Logic problem: Module 4 requires candidate scenarios, but Modules 1-3 do not necessarily produce scenarios. The orchestration file names a generate_candidate_scenarios(...) bridge, but this is not a formal module.
- Governance/legitimacy issue: constraint rule ownership must be explicit.

Minimum viable version:

Use a mandatory facilitator checklist:

- ecological red flags
- material availability
- labor capacity
- accessibility/fairness
- safety/legal/constitutional constraints
- OAD certification/design dependency
- FRS monitoring requirement
- "unknown but important" fields

Build-readiness: Needs clarification for full system; MVB checklist is build-ready.
