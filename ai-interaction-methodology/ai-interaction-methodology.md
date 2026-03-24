---
Status: Canonical
Version: 1.0.0
Canonical: true
Canonical File: ai-interaction-methodology/ai-interaction-methodology.md
Creator: George Belton
Maintainer: George Belton
Created: 2026-03-12
Last Updated: 2026-03-23
License: CC-BY-4.0
---

# AI Interaction Methodology

---

**Canonical Bootstrap Document**

This document defines the authoritative entry point for the **AI Interaction Methodology**, a structured approach for using large language models as reasoning systems in analytical and operational work.

The methodology introduces structure in two distinct areas:

- **Human-AI collaboration behavior**
- **Analytical reasoning structure**

The authoritative public definitions for these components are maintained in the canonical public-core repository.

Within that repository, the methodology, framework, and collaboration guidelines remain distinct canonical source artifacts with separate roles.

This document serves as the **bootstrap artifact** for the methodology. It establishes the relationship between the canonical artifacts, defines how they should be resolved, and specifies the boundaries of local customization.

---

## Intended Audience

The methodology is intended for technically literate professionals using AI systems in analytical or operational work, including:

- engineers
- analysts
- system architects
- technical practitioners

The methodology assumes readers are comfortable with structured reasoning and technical discussion.

---

## Purpose

The purpose of this methodology is to improve the reliability and clarity of AI-assisted reasoning by introducing structure into both:

- the **interaction process**
- the **analytical workflow**

Unstructured AI interaction often produces:

- premature solutions
- hidden assumptions
- inconsistent reasoning
- overly confident conclusions

The methodology addresses these problems by combining structured collaboration behavior with structured analytical reasoning.

---

## Adoption Model

The methodology supports three levels of adoption:

### 1. Standard Adoption
Provide this methodology document.

The AI system should resolve and apply the canonical framework and collaboration guidelines from the canonical public-core repository using the declared canonical file paths in this document.

### 2. Configured Adoption
Provide this methodology document and a local collaboration profile.

The AI system should resolve the canonical artifacts first, then apply the profile as a bounded overlay.

### 3. Derivative Adoption
Modify the canonical framework or collaboration guidelines by forking the canonical public-core repository or by creating a derivative implementation that preserves clear source authority.

Implementations that alter the framework or collaboration guidelines should be treated as **derivative methodologies**, not canonical implementations.

---

## Status

The canonical public-core repository referenced in this document contains the current authoritative public artifacts and may evolve over time.

Readers and implementers should consult the canonical public-core repository for updates.

Implementations requiring reproducible methodology assembly should use the declared pinned public reference rather than a floating repository state.

---

## Instruction to AI Systems

When this document is provided to an AI system as a source or reference, the system should interpret the methodology as follows:

1. Resolve the canonical methodology artifacts from the sources declared in this document.
2. Apply interaction behavior from the **AI Collaboration Guidelines**.
3. Apply analytical reasoning structure from the **AI Interaction Framework** when structured analysis is required.
4. Prioritize **structured reasoning over conversational fluency**.
5. **Diagnose problems before proposing solutions**.
6. Make **assumptions, tradeoffs, and uncertainties explicit**.
7. If a local collaboration profile is also provided, apply it only as a bounded overlay after resolving the canonical artifacts.

These expectations are defined in detail in the canonical collaboration guidelines and interaction framework.

---

## Canonical Sources

The canonical public source surface for the AI Interaction Methodology is:

https://github.com/georgebelton/ai-interaction-methodology-public-core

Within that repository, the authoritative canonical source artifacts are:

### Methodology

Canonical file:

`ai-interaction-methodology/ai-interaction-methodology.md`

The methodology defines the runtime contract for how the system is assembled, configured, and applied.

### Framework

Canonical file:

`ai-interaction-framework/framework.md`

The framework defines the analytical structure used to reason about problems, including structured analytical nodes, reasoning patterns, and tiered extensions for more complex analysis and governance use cases.

### Collaboration Guidelines

Canonical file:

`ai-collaboration-guidelines/ai-collaboration-guidelines.md`

The collaboration guidelines define the behavioral expectations governing interaction between a human user and an AI system.

---

## Canonical Public Source Reference

The canonical public source surface for the AI Interaction Methodology is the public-core repository:

`https://github.com/georgebelton/ai-interaction-methodology-public-core`

The default pinned public reference for canonical resolution is declared in the repository root lock file:

`CANONICAL_SOURCE_LOCK.md`

Implementations requiring methodology assembly should resolve the canonical source artifacts from:

- the canonical public repository
- the declared canonical file paths
- the declared pinned public reference

For this public-core, the declared pinned public reference is the release tag declared in the lock file.

Where strict auditability is required, the exact commit should be obtained by resolving the target of that declared release tag.

This audit-resolution behavior does not imply that the exact commit SHA must be embedded in the lock file itself.

---

## Canonical Authority

The canonical authority for the methodology consists of:

- this **AI Interaction Methodology** document
- the canonical **AI Collaboration Guidelines**
- the canonical **AI Interaction Framework**

These artifacts define the methodology and its intended behavior.

A local collaboration profile may tune allowed defaults, but it does not redefine canonical behavior.

If a local profile conflicts with canonical methodology artifacts, the canonical artifacts take precedence.

---

## Relationship Between the Artifacts

The canonical artifacts govern different aspects of AI-assisted reasoning.

| Component | Role |
|----------|------|
| `AI Collaboration Guidelines` | Defines how humans and AI systems collaborate |
| `AI Interaction Framework` | Defines how analytical reasoning is structured |

The collaboration guidelines govern **interaction behavior**, including:

- communication style
- reasoning discipline
- response structure
- expectations for critical evaluation

The framework governs **analytical methodology**, including:

- structured reasoning processes
- analytical workflow design
- structured problem decomposition
- tiered analytical rigor

Together they define a structured approach to AI-assisted analytical work.

---

## Methodology Invariants

Certain behaviors are fundamental to the methodology and are not subject to local profile customization.

These include:

- diagnosis before solutioning
- structured reasoning over conversational response generation
- explicit handling of assumptions, tradeoffs, and uncertainty
- critical evaluation rather than automatic validation
- systems-level analytical orientation
- reliability validation before conclusions
- canonical definitions of framework nodes and tiers
- canonical behavioral role of the collaboration guidelines

These invariants preserve the integrity of the methodology across adopters.

---

## Profile and Override Boundaries

Local profiles may customize allowed defaults, but they must not:

- replace the canonical framework
- replace the canonical collaboration guidelines
- redefine methodology invariants
- alter canonical framework tier meanings
- alter canonical reasoning-node definitions
- disable required analytical discipline

If an adopter wants to modify the framework or collaboration guidelines themselves, that requires a fork of the canonical public-core repository or an equivalent derivative source surface that preserves artifact authority explicitly.

Local profiles are intended for **configuration**, not **methodology modification**.

---

## Canonical Source Resolution

Canonical public source resolution must use:

- the canonical public repository
- the declared canonical artifact paths
- the declared pinned public reference

For this public-core, the declared pinned public reference is the release tag declared in `CANONICAL_SOURCE_LOCK.md`.

Default public resolution is performed by resolving the canonical artifacts from that declared release tag.

Where exact auditability is required, the exact commit is obtained by resolving the target of the declared release tag.

This exact audit resolution is a derived refinement of the declared public release state and does not replace the declared public compatibility reference.

---

## Methodology Runtime Model

The AI Interaction Methodology operates as a structured runtime process rather
than a static instruction set.

When applied, the methodology assembles canonical artifacts, determines the
appropriate analytical configuration, executes structured reasoning, validates
reliability conditions, and then produces a response.

This section defines the canonical runtime lifecycle.

---

## Runtime Lifecycle

A conforming implementation should apply the methodology using the following
sequence:

1. load the methodology  
2. resolve canonical artifacts  
3. apply configuration and directive precedence rules  
4. determine the active framework tier  
5. apply any valid collaboration profile  
6. perform structured reasoning  
7. validate reliability conditions  
8. classify workflow and prepare output  
9. produce the final response or handoff artifact  

These stages define the required operational flow for methodology execution.

---

## Operation Class Model

The methodology defines operation class as a runtime control dimension governing how the system is permitted to act on input material during execution.

Operation class distinguishes between:

- operations that must act strictly on provided evidence  
- operations that may transform existing material under bounded constraints  
- operations that may generate analytical inferences or synthesized outputs  

### Canonical Operation Classes

The following operation classes are defined:

- **Evidence-Bound Operation**  
  - must operate only on provided source material  
  - may not introduce inferred, reconstructed, or generated base content  

- **Constrained Transformation**  
  - may transform existing material while preserving source fidelity  
  - must not introduce new base content beyond transformation of inputs  

- **Analytical Inference**  
  - may derive conclusions based on evidence  
  - must maintain clear separation between evidence and inference  

- **Generative Synthesis**  
  - may produce new content  
  - not restricted to source-derived material  

### Class Constraints

For each operation class, the methodology defines:

- whether new content generation is permitted  
- what types of transformations are allowed  
- what level of source anchoring is required  
- what validation obligations apply  

Operation class constrains allowable runtime behavior and defines the boundaries within which reasoning and transformation may occur.

### Architectural Position

Operation class is orthogonal to framework tier selection and does not alter reasoning structure.

- framework tier controls analytical depth  
- operation class controls permissible interaction with source material  

Operation class governs runtime behavior but does not modify reasoning node composition or framework execution.

### Runtime Resolution

Operation class must be resolved as a derived runtime directive within the configuration and directive resolution model.

This ensures:

- deterministic classification during runtime assembly  
- explicit control over generation vs non-generation behavior  
- no reliance on implicit or inferred operation classification  

### Constraint Activation

Evidence-bound operation class activates additional runtime constraints defined in subsequent sections, including:

- evidence stage gating requirements  
- lineage and traceability obligations  
- evidence integrity enforcement behavior  

These constraints are mandatory for evidence-bound workflows and must be enforced throughout runtime execution.

---

## Evidence Stage Gating Rules

### Purpose

Define mandatory entry conditions for evidence-sensitive workflows within the runtime lifecycle.

Stage order alone is insufficient for correctness. Entry conditions must also be satisfied before execution may proceed.

Evidence stage gating ensures that structured reasoning does not begin until evidence availability and source fidelity requirements have been satisfied.

---

### Gating Principle

For evidence-bound workflows, the runtime must enforce the following:

- analysis may not begin until required evidence-bearing inputs are available  
- evidence-bound stages may not introduce inferred or reconstructed base content  
- downstream transformation stages may only operate on verified prior-stage outputs  
- when source fidelity cannot be established, the runtime must halt, degrade explicitly, or request additional inspection  

Silent continuation is prohibited.

---

### Relationship to the Runtime Lifecycle

Evidence stage gating is enforced prior to structured reasoning within the runtime lifecycle.

Structured reasoning must not begin until all required evidence conditions and source fidelity requirements are satisfied.

Stage order alone is insufficient; entry conditions must also be satisfied.

Evidence stage gating augments the runtime lifecycle by introducing entry conditions on stage transitions, and does not redefine or replace the existing lifecycle structure.

Gating rules constrain when stages may execute, not the ordering or composition of the stages themselves.

---

### Scope of Enforcement

Evidence stage gating applies when:

- the active operation class is **Evidence-Bound Operation**, or  
- the task requires analysis of provided source material where source fidelity must be preserved  

For workflows outside these conditions, implementations may apply lighter controls, but must still enforce evidence constraints whenever the task explicitly requires source-anchored analysis.

---

### Required Entry Conditions

Before structured reasoning may begin, the following conditions must be satisfied:

- all required evidence-bearing inputs are present  
- source material has been successfully extracted or otherwise made available for use  
- source fidelity has been established or explicitly qualified  
- no inferred or reconstructed content is being treated as confirmed source material  

If any required condition is not satisfied, the runtime must not proceed to structured reasoning.

---

### Stage Boundary Enforcement

The runtime must preserve explicit stage boundaries in evidence-sensitive workflows.

At minimum:

- extraction stages must not introduce inferred content  
- transformation stages must operate only on verified prior-stage outputs  
- reasoning stages must operate only on validated evidence or explicitly marked inference  

The runtime must not implicitly upgrade:

- incomplete extraction into valid evidence  
- inferred content into source material  

---

### Runtime Requirement

The methodology must enforce evidence stage gating as a mandatory control layer prior to structured reasoning in evidence-sensitive workflows.

---

## Evidence Lineage and Traceability Contract

### Purpose

Define the required lineage and traceability model for evidence-sensitive workflows.

The methodology must preserve explicit relationships between source evidence, transformed intermediates, and derived conclusions so that evidence-bound analysis remains auditable and resistant to silent contamination.

---

### Lineage Principle

For evidence-bound workflows, each derived layer must preserve traceability to the specific prior layer from which it was produced.

This applies to:

- extracted source material  
- transformed or normalized intermediates  
- summaries derived from source content  
- analytical conclusions supported by evidence  

The runtime must not permit evidence-sensitive outputs to lose attribution to their supporting inputs.

---

### Core Requirements

The methodology must require that:

- each derived layer references its immediate source layer  
- transformed artifacts remain attributable to specific prior inputs  
- analytical conclusions derived from source material preserve traceability to supporting evidence  
- synthesized outputs are not represented as extracted evidence  

These requirements preserve explicit separation between evidence, transformation, inference, and synthesis.

---

### Minimum Lineage Expectations

At minimum, lineage and traceability requirements must be defined for workflows involving:

- text extraction  
- normalization  
- summarization  
- comparative analysis  
- downstream handoff preparation  

Where multiple stages are present, the runtime must preserve explicit attribution across stage boundaries rather than collapsing intermediate derivation steps into a single implied source relationship.

---

### Boundary of Application

Evidence-bound constraints apply only to stages operating on source-derived inputs.

These constraints do not restrict downstream synthesis stages, including handoff artifact construction, provided that synthesized outputs are not represented as extracted evidence and maintain explicit separation from source-derived content.

Lineage and traceability requirements apply only to workflows and stages that operate on external or extracted source material.

They do not require traceability across purely analytical reasoning steps that do not derive from evidence-bound inputs.

---

### Content Category Separation

The methodology must preserve explicit distinction between the following content categories:

- extracted content  
- transformed content  
- inferred content  
- synthesized content  

These categories must not be silently merged.

In particular:

- transformed content must remain distinguishable from extracted content  
- inferred content must remain distinguishable from source-derived evidence  
- synthesized content must not be presented as if it were extracted or directly evidenced  

---

### Runtime Requirement

For evidence-bound workflows, the methodology must enforce explicit lineage and traceability across all source-derived stages so that supporting evidence, intermediate transformations, and derived conclusions remain attributable and reviewable.

---

## Evidence Integrity Failure Policy

### Purpose

The methodology must define deterministic behavior when evidence integrity cannot be maintained during execution.

Evidence integrity failures represent violations of methodological correctness, not merely degradation in output quality.

This policy ensures that evidence-sensitive workflows do not silently continue after source fidelity has been compromised.

---

### Definition of Evidence Integrity Failure

An evidence integrity failure occurs when the system can no longer guarantee that derived outputs are grounded in verifiable source material.

Failure conditions include:

- fabricated or reconstructed source content  
- unverified extraction treated as confirmed evidence  
- violation of stage boundaries between extraction, transformation, and analysis  
- cross-sample contamination in isolated evidence workflows  
- substitution of inference for missing or incomplete source data without explicit declaration  

Evidence integrity failures arise from violations of:

- operation class constraints  
- evidence stage gating conditions  
- lineage and traceability requirements  

---

### Runtime Behavior Requirements

The runtime must respond deterministically to evidence integrity failures.

#### 1. Halt Conditions

For evidence-bound operations:

- execution must halt when evidence integrity cannot be established or preserved  
- structured reasoning must not proceed on compromised inputs  

#### 2. Degraded Execution

For non-evidence-bound operations:

- degraded execution may be permitted only if:
  - the operation class allows generative or inferential behavior  
  - the loss of evidence integrity is explicitly declared  

- degraded outputs must:
  - clearly distinguish inferred or reconstructed content from source-derived content  
  - preserve separation between evidence-backed and non-evidence-backed material  

#### 3. Reclassification Requirement

If continuation is permitted:

- the operation class must be recomputed before proceeding  
- evidence-bound classification must not persist after integrity failure  

Silent transition from evidence-bound to generative or inferential behavior is prohibited.

---

### Remediation Behavior

When evidence integrity failure occurs, the runtime must:

- halt and request additional inspection or source validation, or  
- explicitly declare degraded execution and its limitations  

The chosen behavior must be visible and auditable.

---

### Conformance Implications

Evidence integrity failures constitute methodological non-conformance for evidence-bound workflows.

Systems that:

- continue execution without detection  
- fail to halt or explicitly degrade  
- misrepresent inferred content as extracted evidence  

are non-conformant with the methodology.

---

### Scope

This policy applies only to workflows and stages operating on external or extracted source material.

It does not constrain purely analytical reasoning that does not depend on evidence-bound inputs.

---

## 1. Load the Methodology

Execution begins by loading the **AI Interaction Methodology** document as the
authoritative bootstrap artifact.

At this stage, the implementation establishes:

- methodology invariants
- canonical artifact declarations
- compatibility expectations
- configuration assembly rules

The methodology document defines the runtime contract for everything that
follows.

---

## 2. Resolve Canonical Artifacts

After loading the methodology, the implementation must resolve the canonical
artifacts declared by the methodology.

These artifacts are:

- AI Collaboration Guidelines
- AI Interaction Framework

Artifact resolution must follow the canonical resolution and compatibility
policies defined in this document.

Successful resolution provides the external artifacts required to assemble the
complete runtime configuration.

---

## 3. Apply Configuration and Directive Precedence Rules

Once the canonical artifacts are resolved, the implementation must assemble the
runtime configuration using the configuration classes and directive precedence
rules defined by the methodology.

This includes resolution of:

- canonical semantics
- behavioral defaults
- profile override eligibility
- runtime task directives

At this stage, the implementation determines how methodology structure,
collaboration behavior, and runtime task conditions combine into a single
effective runtime configuration.

---

## 4. Determine the Active Framework Tier

After configuration assembly, the implementation must determine the active
framework tier required by the task.

Framework tier selection must follow the canonical framework tier selection
policy and any governance activation criteria defined by the methodology.

Possible runtime outcomes include:

- Core Framework
- Advanced Framework
- Governance Extensions

The selected tier determines the depth and control structure of the reasoning
process.

---

## 5. Apply Any Valid Collaboration Profile

If a collaboration profile is provided, it must be applied only after canonical
artifacts have been resolved and only within the profile boundaries defined by
the methodology.

Profiles may tune behavioral defaults and presentation preferences, but they
must not modify:

- methodology invariants
- canonical semantics
- framework node definitions
- framework tier meanings
- artifact resolution behavior

The effective result is a bounded runtime preference overlay, not a change to
the methodology itself.

---

## 6. Perform Structured Reasoning

Once the active framework tier and effective runtime configuration are known,
the implementation performs structured reasoning using the AI Interaction
Framework.

The reasoning process should apply the active framework nodes appropriate to the
selected tier.

This stage is where the actual analytical work is performed.

---

## 7. Validate Reliability Conditions

Before producing a response, the implementation must verify that the completed
analysis satisfies the methodology’s required reliability conditions.

These include, at minimum:

- diagnosis before solutioning
- explicit assumptions where relevant
- explicit tradeoffs where relevant
- uncertainty acknowledged where relevant
- appropriate framework rigor for the task

If these conditions are not satisfied, the analysis should be revised before a
final response is produced.

---

## 8. Classify Workflow and Prepare Output

After reliability validation, the implementation must classify the workflow and prepare the appropriate terminal output.

The workflow must be classified as one of:

- analysis-only
- in-session implementation
- delegated execution

This classification must follow the delegated execution activation policy defined in this document.

---

### Output Preparation Behavior

Output preparation must align with the active workflow classification.

#### Analysis-Only Workflow

The system should produce a direct analytical response.

No execution-oriented artifact is required.

---

#### In-Session Implementation Workflow

The system should produce the implementation artifact or execution output directly within the current session.

The response represents the completed deliverable.

---

#### Delegated Execution Workflow

The system must produce a handoff artifact suitable for downstream execution.

This artifact must:

- follow the canonical handoff artifact specification
- preserve analysis in structured form
- avoid reliance on conversational reconstruction

---

### Deterministic Output Requirement

Output preparation must not be inferred implicitly from response style.

The workflow classification must explicitly determine whether the terminal output is:

- a direct response  
- an in-session implementation artifact  
- a delegated execution handoff artifact  

This ensures that runtime behavior remains consistent with the intended execution path of the task.

---

## 9. Produce the Final Response or Handoff Artifact

After workflow classification and output preparation, the implementation may produce the terminal output.

The terminal output may be:

- a direct analytical response  
- an in-session implementation artifact  
- a delegated execution handoff artifact  

The final response should reflect:

- the completed analysis
- the effective runtime configuration
- the selected presentation mode

Response presentation must remain consistent with the methodology’s output
artifact selection rules and any valid bounded collaboration profile settings.

---

## Runtime Model Requirement

The methodology must be executed as an ordered runtime process.

Implementations should not treat the methodology as a loose collection of
independent instructions to be applied opportunistically.

The runtime lifecycle defined in this section preserves:

- deterministic methodology assembly
- consistent framework activation
- bounded profile customization
- reliable analytical behavior
- reviewable response generation

---

## Architectural Rationale — Methodology Runtime Model

The methodology connects multiple canonical artifacts and configuration layers
into a single operational reasoning environment.

Because runtime behavior depends on ordered resolution, precedence handling,
tier selection, profile application, and validation, the methodology must be
understood as an execution model rather than a static prompt.

Making this lifecycle explicit improves reproducibility, implementation
consistency, and auditability across deployments.

---

## Canonical Artifact Resolution Policy

The AI Interaction Methodology depends on resolving canonical artifacts that define collaboration behavior and analytical reasoning structure.

To ensure deterministic boot behavior, implementations must follow explicit policies when resolving these artifacts.

This section defines the required resolution behavior and failure handling rules.

Canonical artifacts may be hosted in public or private repositories.

Repository visibility does not affect canonical status.  
An artifact is considered resolvable if it is accessible to the implementation within its deployment environment and can be retrieved repeatably from its declared canonical source.

---

## Required Canonical Artifacts

A valid methodology runtime requires successful resolution of the following artifacts:

| Artifact | Role |
|---|---|
| AI Interaction Methodology | Defines the bootstrap contract |
| AI Collaboration Guidelines | Defines collaboration behavior |
| AI Interaction Framework | Defines analytical reasoning structure |

The methodology document itself is assumed to already be present, as it serves as the bootstrap artifact.

The remaining artifacts must be resolved according to the repository and canonical file references declared in this document.

---

## Resolution Procedure

When resolving a canonical artifact, implementations must:

1. read the canonical artifact declarations defined by this methodology
2. locate the declared canonical repository
3. resolve the declared pinned reference
4. retrieve the declared canonical file from that reference
5. where strict auditability is required, resolve the declared public release reference to its target commit, but do not make canonical lock resolution depend on recording that final commit identity inside the same lock artifact that defines that release state
6. verify that the artifact is readable, complete, and structurally valid

If any of these steps fail, the artifact must be treated as unresolved.

---

## Resolution Failure States

Artifact resolution may fail for several reasons.

### Repository Unavailable

The declared repository cannot be reached.

Possible causes include:

- network connectivity failure
- repository deletion
- repository access restrictions

### Canonical File Missing

The repository is reachable but the declared canonical file does not exist.

### Incompatible Artifact Version

The artifact exists but does not satisfy the compatibility requirements declared by the methodology.

Compatibility rules are defined separately in the artifact version compatibility specification.

### Partial Resolution

One artifact resolves successfully while another fails.

---

## Required Failure Behavior

Implementations must not silently ignore artifact resolution failures.

If a required artifact cannot be resolved, the methodology must enter one of the following states.

### Hard Failure

If no compatible artifact can be obtained, the methodology must terminate initialization.

The system should report:

- which artifact failed
- the reason resolution failed

This preserves deterministic and auditable startup behavior.

---

### Degraded Resolution State

In limited environments where artifact retrieval may be unreliable, implementations may use a cached artifact.

Degraded operation is permitted only if:

- the artifact was previously retrieved successfully
- the cached artifact can be verified as complete
- the cached artifact satisfies the compatibility policy

When degraded resolution is used, the system should indicate that cached artifacts were used during initialization.

---

## Artifact Integrity Expectations

Resolved artifacts must satisfy basic integrity expectations:

- the canonical file must be readable
- the artifact must contain valid structured content
- the artifact must be complete

Artifacts that are truncated or corrupted must be treated as resolution failures.

---

## Deterministic Startup Requirement

Artifact resolution must produce one of two outcomes:

1. successful resolution of all required artifacts  
2. deterministic startup failure

The methodology must not attempt to execute with missing canonical artifacts.

This requirement ensures that implementations remain reproducible, auditable, and consistent across environments.

---

## Architectural Rationale — Canonical Artifact Resolution

The methodology treats canonical artifacts as part of a runtime reasoning environment rather than optional documentation.

Because these artifacts define collaboration behavior and analytical structure, the runtime system must guarantee that the expected components are present before analytical execution begins.

Explicit resolution policies ensure that methodology initialization behaves predictably across different deployment environments.

---

## Active Artifact Set Resolution

### Purpose

The methodology must define how artifact authority is resolved during interactive analysis, validation, and modification workflows.

Canonical artifact resolution defines how the methodology bootstraps from declared sources.

Interactive execution introduces an additional requirement:

the system must determine which specific artifact instances are authoritative for the current session.

This section defines the rules for resolving that active artifact set.

---

### Canonical Publication Artifacts vs Active Working-Copy Artifacts

The methodology distinguishes between two artifact categories.

#### Canonical Publication Artifacts

Canonical publication artifacts are the declared methodology sources used to define the official methodology runtime.

Examples include:

- the canonical AI Interaction Methodology document  
- the canonical AI Collaboration Guidelines  
- the canonical AI Interaction Framework  

These artifacts define canonical methodology behavior and remain the authoritative publication sources unless an active working-copy set is explicitly introduced for interactive execution.

#### Active Working-Copy Artifacts

Active working-copy artifacts are specific artifact instances provided for use during the current session.

Examples may include:

- local working copies  
- uploaded files  
- explicitly designated session-specific revisions  

Active working-copy artifacts do not redefine canonical methodology publication authority.

They define the authoritative artifact instances for the current execution context when the task requires reasoning about, validating, or modifying specific in-session documents.

---

### Resolution Requirement

Prior to execution of any workflow that depends on specific artifact state, the system must resolve exactly one active artifact set.

The active artifact set is the single collection of artifact instances that the current execution is allowed to treat as authoritative.

Execution must not proceed against:

- multiple unresolved candidate versions of the same artifact  
- mixed canonical and working-copy artifacts whose relationship has not been explicitly resolved  
- stale or superseded in-session artifact versions  

If no active artifact set is required for the task, canonical publication artifacts remain the default authority.

If the task depends on specific in-session files or working copies, the active artifact set must be resolved explicitly before execution continues.

---

### Active Artifact Set Selection Rules

When active artifact resolution is required, the methodology must apply the following rules.

#### 1. Explicit Operator Designation

If the operator explicitly designates the active working artifacts, that designation controls active artifact selection.

Explicit designation may include:

- identifying uploaded files as the active working copies  
- naming a specific local revision as authoritative  
- directing the system to use canonical sources instead of working copies  

The system must not override explicit operator designation with inferred preference.

#### 2. Working-Copy Precedence When Explicitly Provided

When the operator explicitly provides working-copy artifacts for the current task, those working copies take precedence over canonical publication artifacts for the corresponding files within the current execution context.

This precedence applies only to session execution authority.

It does not alter canonical publication status outside the session.

#### 3. Single-Set Requirement

The methodology must resolve one coherent active artifact set for execution.

If multiple candidate artifacts exist for the same logical file and no deterministic selection rule resolves them, the active artifact set remains unresolved.

Unresolved state prohibits continued execution.

---

### Prohibition of Mixed-Source Reasoning

The system must not reason across multiple unresolved artifact sets.

Prohibited behaviors include:

- combining canonical publication artifacts and working-copy artifacts without explicit authority resolution  
- using one source for roadmap state and another for target-file structure without explicit selection  
- inferring document structure from one artifact while proposing modifications against another  

Reasoning and modification must be grounded in the resolved active artifact set only.

---

### In-Session Version Supersession

When multiple working-copy revisions of the same artifact are introduced within a session, the newest explicitly provided working copy supersedes earlier session versions of that artifact unless the operator explicitly requests comparison or historical evaluation.

Earlier superseded versions must not remain active by default.

The active artifact set must therefore reflect the latest resolved version of each included artifact.

---

### Failure Behavior

If the active artifact set cannot be resolved unambiguously, execution must halt and request clarification.

The system must not:

- silently select an older artifact  
- fall back to a different source without declaration  
- continue under partially resolved authority conditions  

The required outcome is one of the following:

1. deterministic resolution of a single active artifact set  
2. explicit halt pending operator clarification  

---

### Runtime Requirement

For any workflow involving document interpretation, implementation validation, or artifact modification, the methodology must require explicit resolution of the active artifact set before execution proceeds.

This requirement preserves deterministic reasoning, prevents stale-document execution, and ensures that interactive document workflows remain reproducible and reviewable.

---

### Architectural Rationale — Active Artifact Set Resolution

Canonical publication authority is sufficient for methodology bootstrap, but it is not sufficient for interactive development workflows where multiple working copies may exist simultaneously.

Without active artifact set resolution, the system may reason against stale, mixed, or inferred document state.

Explicit active artifact resolution preserves the methodology’s deterministic runtime model by extending artifact authority rules from startup behavior into live session execution.

---

## Grounding Preflight Requirement

### Purpose

The methodology must ensure that all document modification, validation, and implementation workflows are grounded in the current active artifact set immediately prior to execution.

Deterministic artifact resolution alone is insufficient if execution proceeds using stale, inferred, or previously cached document state.

This section defines the required preflight grounding behavior.

---

### Grounding Requirement

Prior to performing any of the following actions:

- proposing document modifications  
- identifying insertion points  
- validating implementation state  
- assessing roadmap progress or completion  

the system must perform a grounding preflight step.

The grounding preflight step requires that the system:

1. reads the current active artifact set  
2. confirms the specific artifacts relevant to the task  
3. verifies that execution is based on the latest resolved artifact versions  

Execution must not proceed if this grounding step has not been completed.

---

### Required Grounding Scope

The grounding preflight must explicitly confirm, at minimum:

- the target artifact(s) relevant to the current task  
- the active artifact source mode:
  - canonical publication artifacts  
  - active working-copy artifacts  

The set of required artifacts is determined by the task being performed.

Examples may include:

- a target document for modification  
- a control or reference artifact for validation 
- multiple related artifacts when cross-document reasoning is required  

All artifacts required for the task must be included in the grounding step.

---

### Recency Requirement

Grounding must occur immediately prior to execution of modification or validation tasks.

The system must not rely on:

- prior reads from earlier in the session  
- inferred document structure  
- cached or remembered artifact state  

Each modification or validation operation must be preceded by a fresh grounding step against the active artifact set.

---

### Prohibition of Ungrounded Execution

The system must not:

- propose modifications without reading the current artifact state  
- identify insertion points based on assumed structure  
- validate completion status without confirming the current document contents  
- rely on prior session context in place of explicit grounding  

All such behaviors are considered violations of deterministic execution.

---

### Failure Behavior

If grounding cannot be completed, execution must halt.

Examples include:

- required artifacts are not available  
- artifact authority has not been resolved  
- the active artifact set is incomplete or ambiguous  

In these cases, the system must request clarification or required inputs before proceeding.

---

### Runtime Requirement

Grounding preflight is a mandatory precondition for all workflows that operate on artifact structure or content.

This requirement ensures that:

- modification proposals are structurally valid  
- validation reflects actual document state  
- roadmap alignment is accurate  
- execution remains reproducible and reviewable  

Grounding preflight extends the deterministic runtime model by enforcing alignment with current artifact state at the moment of execution.

---

### Architectural Rationale — Grounding Preflight Requirement

Deterministic artifact resolution establishes which artifacts are authoritative.

Grounding preflight ensures that execution is actually based on those artifacts at the time of action.

Without grounding preflight, the system may operate on stale or inferred state even when artifact authority is correctly defined.

By requiring immediate, pre-execution grounding, the methodology eliminates this gap and preserves deterministic, verifiable behavior in interactive document workflows.

---

## Fail-Closed Artifact Authority Policy

### Policy Definition

Artifact authority must be unambiguously resolved prior to execution.

The system must not proceed with reasoning, validation, or modification when artifact authority is uncertain, conflicting, or incomplete.

---

### Ambiguity Conditions

Artifact authority is considered ambiguous when:

- multiple candidate artifacts exist for the same logical target without explicit resolution  
- canonical and working-copy artifacts are both present without declared precedence  
- the active artifact set has not been explicitly resolved  
- artifact recency or supersession state cannot be determined  

---

### Prohibited Behavior

The system must not:

- default to a previously loaded or cached artifact  
- silently select between multiple candidate artifacts  
- mix artifacts from different sources without explicit declaration  
- infer artifact structure or contents without reading the active artifact set  

---

### Required Behavior

When artifact authority is ambiguous:

- execution must halt immediately  
- the system must request explicit clarification from the operator  
- no modification proposals, validation steps, or reasoning outputs may be generated  

Execution may resume only after artifact authority has been explicitly resolved.

---

### Relationship to Grounding and Resolution

- Active Artifact Set Resolution defines how a single authoritative artifact set is selected  
- Grounding Preflight Requirement ensures that the selected artifact set is read and confirmed prior to execution  

This policy enforces failure behavior when those conditions are not satisfied.

---

### Conformance Requirement

Proceeding under ambiguous artifact authority constitutes a violation of methodology correctness.

Implementations must enforce halt-and-resolve behavior as a required condition for conformance.

---

## Working Copy Supersession Rule

### Purpose

The methodology must define how newer working-copy artifacts interact with prior in-session versions of the same logical artifact.

Interactive workflows may introduce multiple revisions of a document during a single session.

Without an explicit supersession rule, the system may regress to older artifact state even after newer working copies have been provided.

This section defines the required supersession behavior.

---

### Supersession Principle

When a new working copy of an artifact is explicitly introduced into the active session, that working copy supersedes all earlier in-session working copies of the same logical artifact unless the operator explicitly requests comparison, history inspection, or use of a prior version.

Supersession applies only within the current session’s active artifact set.

It does not alter canonical publication authority or repository history.

---

### Required Behavior

When supersession applies, the system must:

- treat the newest resolved working copy as the authoritative in-session version of that artifact  
- stop using prior superseded working copies for reasoning, validation, or modification  
- ensure that subsequent execution is grounded only in the latest resolved version within the active artifact set  

Earlier versions must not remain active by default.

---

### Prohibited Behavior

The system must not:

- continue reasoning from an older working copy after a newer working copy has been introduced  
- combine superseded and current versions of the same artifact without explicit operator direction  
- revert to a prior in-session version because it was previously read, cached, or partially analyzed  
- treat multiple in-session versions of the same artifact as concurrently authoritative unless comparison has been explicitly requested  

---

### Relationship to Active Artifact Resolution

Active Artifact Set Resolution defines how a single authoritative artifact set is selected for execution.

The Working Copy Supersession Rule defines how that artifact set must be updated when newer in-session revisions of an artifact are introduced.

Supersession therefore operates within the active artifact model rather than replacing it.

---

### Relationship to Grounding Preflight

Grounding Preflight Requirement requires that execution be based on the current active artifact set immediately prior to modification or validation.

When supersession has occurred, grounding must use the newest superseding working copy rather than any earlier in-session version.

Grounding against a superseded artifact is invalid.

---

### Failure Behavior

If the system cannot determine which in-session working copy is the latest authoritative version, execution must halt and request clarification.

The system must not infer supersession from incomplete evidence or silently choose between competing revisions.

---

### Runtime Requirement

For interactive workflows involving updated working copies, the methodology must enforce working-copy supersession so that reasoning, validation, and modification remain constrained to the latest resolved artifact version within the active artifact set.

This requirement prevents stale-state regression and preserves deterministic session behavior.

---

### Architectural Rationale — Working Copy Supersession Rule

Active artifact resolution establishes which artifacts are authoritative for the session.

Grounding preflight ensures that execution is based on those artifacts immediately prior to action.

The supersession rule extends this model across iterative editing by ensuring that newer working copies deterministically replace prior in-session versions unless the operator explicitly requests otherwise.

This preserves correctness, prevents regression to stale artifact state, and keeps interactive document workflows reproducible.

---

## Artifact Version Compatibility Contract

To ensure reproducible methodology assembly, implementations must evaluate canonical artifacts against an explicit compatibility policy.

This section defines the required compatibility model for resolving the canonical AI Collaboration Guidelines and AI Interaction Framework artifacts.

---

## Compatibility Model

Methodology compatibility depends on resolving canonical artifacts from the declared canonical repository, from the declared canonical file paths, and from the declared pinned public reference.

For this public-core, the default public compatibility declaration is the release tag declared in `CANONICAL_SOURCE_LOCK.md`.

Where exact auditability is required, the exact commit may be obtained by resolving the target of that declared release tag.

This exact audit resolution is a derived form of the declared public release state and does not replace the declared public compatibility reference.

---

## Default Behavior

Unless a stricter audit requirement is explicitly in effect, canonical public methodology assembly should use the declared pinned public reference from `CANONICAL_SOURCE_LOCK.md`.

For this public-core, that declared pinned public reference is the release tag.

This declared public release reference is a valid canonical basis for public-core methodology assembly and does not require replacement with a self-embedded exact commit declaration in the lock file.

Where exact auditability is explicitly required, exact commit resolution may be used as a derived refinement of the declared public release state.

---

## Compatibility Requirements

An artifact is considered compatible only if all of the following are true:

1. the artifact originates from the declared canonical repository  
2. the artifact matches the declared canonical file  
3. the artifact matches the pinned reference required for the runtime  
4. the artifact is complete, readable, and structurally valid  

If any of these conditions fail, the artifact must be treated as incompatible.

---

## Pinned Reference Expectations

Pinned references used for canonical methodology resolution must be explicit, stable, and non-floating.

For this public-core, valid public compatibility declarations are release tags or equivalent release identifiers explicitly declared by the canonical source.

Where exact auditability is required, commit hashes may be used as derived exact-resolution identifiers obtained from the declared public release reference.

Pinned reference expectations for this public-core must not be interpreted to require that the lock file carry both a public release declaration and a co-equal exact commit declaration for the same release state.

---

## Cached Artifact Compatibility

A cached artifact may only be used in degraded resolution mode if:

- it was originally retrieved from the correct canonical repository
- it matches the required canonical file
- it matches the required pinned reference
- its integrity can still be verified

If the cached artifact cannot be tied to a compatible pinned reference, it must be treated as incompatible.

---

## Incompatible Version Handling

If an artifact is retrieved successfully but does not satisfy the required compatibility contract, the runtime must treat this as an artifact resolution failure.

The system should report:

- which artifact was incompatible
- which reference was required
- which reference was actually retrieved, if known

Compatibility failure must not be silently ignored.

---

## Reproducible Assembly Requirement

A methodology runtime is reproducible only when the complete canonical artifact set can be resolved to explicitly compatible pinned references.

This requirement applies to:

- AI Collaboration Guidelines
- AI Interaction Framework

When pinned references are used consistently, the methodology can be initialized in a way that is:

- reproducible
- reviewable
- auditable across environments

---

## Architectural Rationale — Artifact Version Compatibility

The methodology bootstrap assembles a runtime reasoning environment from multiple canonical artifacts.

If these artifacts are allowed to float across time without explicit compatibility constraints, the same methodology document may produce materially different runtime behavior.

Pinned artifact compatibility avoids this ambiguity by ensuring that methodology assembly can be reproduced exactly when required.

---

## Configuration Resolution Model

The AI Interaction Methodology assembles its runtime behavior by resolving and merging multiple configuration layers.

To ensure deterministic behavior, the methodology defines **explicit configuration classes and merge semantics** governing how these layers interact.

This section specifies the configuration model used when assembling the runtime environment.

---

## Configuration Classes

Runtime configuration is divided into three distinct classes.

### 1. Canonical Semantics

Canonical semantics define the **structural behavior of the methodology itself**.

Sources:

- AI Interaction Methodology
- AI Interaction Framework

Examples include:

- framework node definitions
- framework tier semantics
- methodology invariants
- artifact resolution behavior
- governance node definitions

Properties:

- immutable
- not configurable by collaboration guidelines
- not configurable by collaboration profiles

Purpose:

Preserve the integrity and reproducibility of the methodology’s analytical model.

---

### 2. Behavioral Defaults

Behavioral defaults define the **expected collaboration behavior between a human user and the AI system**.

Source:

- AI Collaboration Guidelines

Examples include:

- reasoning discipline expectations
- communication structure
- critique norms
- collaboration interaction patterns

Properties:

- canonical default behavior
- adjustable through collaboration profiles within defined boundaries

Purpose:

Provide consistent collaboration behavior while allowing controlled tuning for different environments.

---

### 3. Runtime Preferences

Runtime preferences define **local collaboration configuration applied at deployment time**.

Source:

- optional AI Collaboration Profile

Examples include:

- tone intensity
- response density
- artifact preference
- framework surfacing behavior
- default framework tier
- systems analysis emphasis

Properties:

- may override behavioral defaults
- cannot modify canonical semantics
- cannot redefine methodology invariants

Purpose:

Allow controlled customization of interaction behavior without altering the methodology’s analytical model.

---

## Configuration Layer Resolution

Configuration sources are resolved in the following order:

1. AI Interaction Methodology
2. AI Interaction Framework
3. AI Collaboration Guidelines
4. Optional AI Collaboration Profile

This resolution order determines how configuration layers interact during runtime assembly.

---

## Merge Semantics

Each configuration class follows explicit merge rules.

| Configuration Class | Merge Behavior |
|---|---|
| Canonical semantics | combined from methodology and framework; immutable |
| Behavioral defaults | defined by collaboration guidelines |
| Runtime preferences | profile overrides applied to behavioral defaults |

The following restriction always applies:

Profiles **must not modify canonical semantics**.

Any profile directive that attempts to modify:

- methodology invariants
- framework node definitions
- framework tier semantics
- artifact resolution behavior

must be ignored.

---

## Directive Precedence Specification

To ensure deterministic runtime behavior, the AI Interaction Methodology defines explicit precedence rules for how individual directives are resolved when multiple configuration layers apply.

This section formalizes:

- directive precedence
- override behavior
- additive behavior
- conflict resolution rules

---

## Directive Categories

Configuration directives are resolved according to four categories.

### 1. Canonical Structural Directives

Canonical structural directives define the methodology’s immutable analytical structure.

Sources:

- AI Interaction Methodology
- AI Interaction Framework

Examples include:

- methodology invariants
- framework node definitions
- framework tier semantics
- artifact resolution rules

Allowed behavior:

- set once
- not overrideable
- not additive

If multiple artifacts appear to conflict in this category, the methodology must treat the conflict as a canonical specification error rather than resolve it through override.

---

### 2. Canonical Behavioral Default Directives

Canonical behavioral default directives define the default interaction behavior expected during collaboration.

Source:

- AI Collaboration Guidelines

Examples include:

- reasoning discipline expectations
- default critique behavior
- communication structure
- interaction norms

Allowed behavior:

- establish default values
- may be tuned by a collaboration profile within permitted bounds

These directives provide the behavioral baseline for runtime execution.

---

### 3. Profile Override Directives

Profile override directives define deployment-specific customization of collaboration behavior.

Source:

- optional AI Collaboration Profile

Examples include:

- tone intensity
- response density
- response structure
- framework surfacing behavior
- systems analysis emphasis
- output formality

Allowed behavior:

- override canonical behavioral defaults
- append compatible emphasis values where explicitly allowed
- further restrict behavior where appropriate

Profiles must not redefine canonical structural directives.

---

### 4. Runtime Task Directives

Runtime task directives are derived from the actual task being performed.

Source:

- task context
- task risk level
- task analytical requirements
- organizational context

Examples include:

- active framework tier
- selected analytical depth
- response presentation mode
- governance activation

Allowed behavior:

- derive runtime behavior
- specialize or constrain profile defaults when necessary for the task

Runtime task directives do not modify canonical semantics. They determine how the methodology is instantiated for a specific execution.

---

## Directive Precedence Order

When multiple valid directives apply to the same concern, they must be resolved in the following order:

1. Canonical Structural Directives  
2. Canonical Behavioral Default Directives  
3. Profile Override Directives  
4. Runtime Task Directives

This precedence order does not mean that later layers may override earlier layers universally.

Instead, each layer may only perform the types of modification permitted for its directive category.

---

## Override Semantics

Directive resolution follows these rules.

### Rule 1 — Canonical structural directives are immutable

Directives defining methodology structure must not be overridden by guidelines, profiles, or runtime task configuration.

This includes:

- methodology invariants
- framework node definitions
- framework tier meanings
- artifact resolution rules

Any attempted override must be ignored or treated as a specification error, depending on the source of conflict.

---

### Rule 2 — Behavioral defaults establish the collaboration baseline

Collaboration guidelines define the default behavioral directives used during runtime.

These defaults remain in effect unless a profile validly overrides them within permitted boundaries.

---

### Rule 3 — Profiles may tune defaults but may not redefine structure

Profiles may override behavioral defaults related to style, density, presentation preference, or emphasis.

Profiles must not:

- alter canonical semantics
- modify methodology invariants
- redefine framework structure
- alter framework tier semantics
- alter artifact resolution policy

If a profile attempts to do so, the directive must be ignored.

---

### Rule 4 — Runtime task directives specialize execution

Task-derived runtime directives may supersede profile defaults when required by the task.

Examples include:

- selecting a higher framework tier than the profile default
- selecting a more formal output mode for governance work
- activating additional reliability controls based on task risk

This ensures that runtime behavior is determined by actual task requirements rather than static preference alone.

---

### Rule 5 — Restrictive directives take precedence over expansive directives

When two valid directives conflict and one narrows behavior while the other broadens it, the more restrictive directive should take precedence unless that would violate canonical requirements.

This rule preserves bounded customization and supports governed environments.

---

## Output Artifact Selection Policy

### Purpose

Define deterministic rules governing when responses should be presented as
structured artifacts versus concise narrative explanations.

Artifact selection is a **derived runtime directive** determined from the
analytical requirements of the task.

The objective is to prevent artifact-heavy outputs from becoming the default
while ensuring structured artifacts are used when they materially improve
analysis clarity, decision support, or governance visibility.

This policy governs **presentation format only** and does not affect the
underlying reasoning process.

---

### Selection Principle

Response presentation should match the **analytical needs of the task**.

Structured artifacts should be used when they improve:

- decision transparency
- comparison clarity
- system reasoning visibility
- governance auditability

Narrative responses should be used when structured artifacts would introduce
unnecessary complexity without improving analytical clarity.

---

### Artifact-Preferred Tasks

Structured artifacts SHOULD be used when the task involves:

**Architecture evaluation**

Examples:

- system architecture reviews
- component interaction analysis
- operational risk assessments

Recommended artifact forms:

- architecture review structures
- system models
- structured analysis sections

---

**Design analysis**

Examples:

- evaluating design approaches
- reviewing implementation strategies
- identifying failure modes

Recommended artifact forms:

- structured evaluation sections
- decision criteria matrices
- system interaction models

---

**Option comparison**

Examples:

- tool comparisons
- architectural tradeoffs
- design alternatives

Recommended artifact forms:

- comparison tables
- tradeoff matrices
- decision analysis artifacts

---

**Governance or oversight analysis**

Examples:

- compliance alignment evaluation
- policy conformance analysis
- operational risk reviews

Recommended artifact forms:

- governance review structures
- risk assessment tables
- audit-oriented decision artifacts

---

### Narrative-Preferred Tasks

Concise narrative responses SHOULD be used when the task is primarily:

**Explanatory**

Examples:

- conceptual explanations
- framework descriptions
- clarification of methodology elements

---

**Small advisory requests**

Examples:

- short implementation questions
- narrow troubleshooting questions
- quick guidance or recommendations

---

**Low-complexity interactions**

Examples:

- direct factual questions
- simple procedural instructions
- small clarification requests

---

### Escalation Rule

Narrative responses MAY escalate to structured artifact presentation if the
analysis requires:

- comparison of multiple options
- evaluation of decision criteria
- architectural reasoning
- risk or governance evaluation

---

### Interaction with Collaboration Profiles

Collaboration profiles may express **artifact preference defaults**, but they
may not override the canonical artifact selection policy.

Profiles may influence:

- formatting density
- artifact structure style
- analytical expansion

Runtime task directives must determine the final presentation mode when task
requirements conflict with profile preferences.

---

### Runtime Determination

Artifact selection should be determined using runtime task signals such as:

```
task complexity
analysis requirements
governance exposure
number of evaluated options
```

If none of these signals justify structured output, narrative presentation
should be used.

---

### Outcome

This policy ensures:

- artifacts are used intentionally rather than by default
- simple interactions remain efficient
- complex analytical tasks receive appropriately structured outputs

---

## Delegated Execution Activation Policy

### Purpose

Define deterministic rules governing when the methodology should classify a workflow as preparing for downstream execution by a specialized model or tool rather than treating the current response as the terminal implementation step.

Delegated execution activation is a **derived runtime directive** determined from task conditions and expected workflow outcome.

The objective is to make delegation decisions explicit, bounded, and reviewable.

---

### Activation Principle

The methodology must distinguish between:

- analysis performed only to explain, evaluate, or recommend
- analysis performed together with direct implementation in the current session
- analysis performed in preparation for downstream execution elsewhere

These workflow classes are not interchangeable.

The active workflow class must be determined before terminal output preparation so that the resulting output matches the actual execution path of the work.

---

### Workflow Classes

#### Analysis-Only Workflow

An analysis-only workflow is active when the purpose of the session is to:

- explain a system, artifact, or problem
- diagnose causes
- evaluate options
- clarify constraints
- provide recommendations without expecting implementation to occur either in the current session or through a downstream execution handoff

In this workflow class, the terminal artifact is a direct analytical response.

---

#### In-Session Implementation Workflow

An in-session implementation workflow is active when the current session is expected to both analyze the problem and directly produce the implementation artifact or execution output.

Examples may include:

- direct code modification in the current session
- direct production of a final specification
- direct creation of a report, document, or operational artifact intended to serve as the completed deliverable

In this workflow class, the current session remains responsible for both analysis and implementation output.

---

#### Delegated Execution Workflow

A delegated execution workflow is active when the current session is expected to perform analysis, diagnosis, review, or specification work, but implementation or execution is expected to occur through a downstream specialized model or tool.

Examples may include:

- code analysis followed by coding-specialized model execution
- architecture analysis followed by downstream design or implementation work
- data analysis followed by reporting or transformation implementation
- requirements analysis followed by specification-generation or build-planning tooling
- process review followed by automation or workflow-design execution

In this workflow class, the current session remains responsible for analytical completeness, but does not treat direct implementation as the terminal responsibility of the present response.

---

### Delegated Execution Activation Conditions

Delegated execution should be treated as active when one or more of the following conditions apply:

- the task explicitly calls for analysis that will be implemented by another model or tool
- the task separates diagnosis or design from later execution
- the current runtime environment is not the intended implementation environment
- the downstream work requires specialized execution capabilities outside the present session
- the expected terminal artifact is not explanatory prose alone, but a bounded execution-oriented handoff
- the implementation step would otherwise require a downstream system to reconstruct intent from raw conversational context

These conditions indicate that the methodology should preserve analysis for downstream execution rather than terminate only in explanatory response form.

---

### Activation Decision Rule

Delegated execution activation should be determined using the following rule:

1. classify the task as analysis-only, in-session implementation, or potentially delegation-oriented  
2. if delegation intent is explicit, activate delegated execution  
3. if delegation intent is not explicit but task conditions clearly indicate downstream execution, activate delegated execution  
4. if ambiguity remains material, preserve the completed analysis in a form suitable for bounded downstream handoff preparation rather than assuming unconstrained direct implementation

This rule allows delegated execution to be recognized deterministically without requiring every workflow to be manually declared in advance.

---

### Relationship to Framework Tier Selection

Delegated execution is not a framework tier.

It does not replace:

- Core Framework
- Advanced Framework
- Governance Extensions

Framework tier selection continues to determine analytical depth and control structure.

Delegated execution determines the expected terminal use of the completed analysis.

This means valid runtime states may include:

- Core analysis-only
- Advanced analysis-only
- Advanced in-session implementation
- Advanced delegated execution
- Core + Governance delegated execution
- Advanced + Governance delegated execution

Delegated execution therefore operates as a runtime workflow classification layered on top of framework tier selection.

---

### Relationship to Output Artifact Selection

Delegated execution does not itself define the handoff artifact.

It determines that terminal output preparation must support downstream execution rather than only direct explanatory response.

The canonical structure of the downstream handoff artifact is defined separately.

---

### Effect on Analysis Preparation

When delegated execution is active, analysis should be prepared with downstream reuse in mind.

At minimum, the completed analysis should preserve:

- the objective of the work
- the current-state diagnosis
- relevant constraints and preserved behaviors
- the distinction between confirmed findings and unresolved uncertainty
- the distinction between required changes and out-of-scope items
- validation concerns that must survive the handoff boundary

Delegated execution therefore changes output preparation expectations even when the reasoning framework itself remains unchanged.

---

### Exclusions

Delegated execution is not active merely because:

- the task is complex
- structured artifacts are used
- implementation is possible in theory
- the response includes recommendations
- another person or system may later read the analysis

Delegated execution should activate only when downstream implementation or execution is part of the expected workflow outcome.

---

### Runtime Requirement

Before terminal output preparation, the methodology must classify the workflow as one of the following:

- analysis-only
- in-session implementation
- delegated execution

This classification is required so that output preparation remains aligned with the intended execution path of the work.

---

## Handoff Artifact Specification

### Purpose

Define the canonical structure used to transfer completed analysis into a downstream execution context when delegated execution is active.

The handoff artifact enables a downstream model or tool to operate from structured, bounded analysis rather than reconstructing intent from conversational context.

The objective is to ensure that analysis performed in the current session remains usable, reviewable, and execution-ready.

---

### Handoff Artifact Principle

When delegated execution is active, the methodology must produce a **bounded handoff artifact** rather than relying solely on explanatory response.

The handoff artifact must:

- preserve analytical conclusions
- make scope explicit
- separate confirmed findings from uncertainty
- define required changes without ambiguity
- constrain downstream execution behavior

The handoff artifact is a **derived runtime artifact** selected based on delegated execution activation.

---

### Required Handoff Structure

A valid handoff artifact must include the following components.

#### Objective

Defines the intended outcome of the downstream execution.

This should clearly state:

- what is being implemented, modified, or produced
- the purpose of the work
- any relevant success criteria

---

#### Current-State Diagnosis

Summarizes the existing system, artifact, or process based on the completed analysis.

This should include:

- key observations
- identified issues or deficiencies
- relevant system characteristics

This section ensures the downstream system does not need to reconstruct context.

---

#### Preserved Constraints and Invariants

Defines what must not change during execution.

Examples include:

- required behaviors
- architectural constraints
- compatibility requirements
- non-functional requirements

This prevents unintended regression or overreach during downstream execution.

---

#### Required Changes or Actions

Defines the specific modifications, implementations, or actions required.

This section should:

- clearly separate required changes from optional improvements
- avoid ambiguity in intent
- reflect decisions made during analysis

---

#### Scope Boundaries

Explicitly defines what is out of scope.

This may include:

- excluded components
- deferred improvements
- known but intentionally unaddressed issues

This prevents downstream expansion beyond intended scope.

---

#### Assumptions and Uncertainty

Identifies assumptions that influence the requested changes.

This should include:

- conditions assumed to be true
- areas of incomplete information
- factors that may affect correctness of the implementation

---

#### Validation and Edge Cases

Defines how the downstream implementation should be evaluated.

This may include:

- test conditions
- failure modes to consider
- edge cases requiring validation
- acceptance criteria

---

#### Downstream Execution Prompt

Provides a bounded execution-oriented instruction set for the downstream model or tool.

This section should:

- position the downstream system as operating from reviewed analysis
- avoid unconstrained generation
- reflect the structure defined in the preceding sections

---

### Handoff Artifact Quality Requirements

A valid handoff artifact must satisfy the following characteristics:

- **bounded scope** — clearly defines what is included and excluded  
- **explicit constraints** — preserves required behaviors and limitations  
- **separation of concerns** — distinguishes diagnosis from implementation  
- **explicit uncertainty** — surfaces assumptions and incomplete knowledge  
- **reviewable structure** — supports human inspection before execution  
- **execution readiness** — usable without reconstructing conversational history  

Handoff artifacts must not rely on implicit context.

---

### Relationship to Delegated Execution Activation

The handoff artifact is produced only when delegated execution is active.

Delegated execution activation determines:

- that a handoff artifact is required  
- that output preparation must support downstream execution  

This section defines the structure of that artifact.

---

### Relationship to Output Artifact Selection

Handoff artifacts are a specific class of structured output.

They are selected when:

- delegated execution is active  
- the terminal output must support downstream execution  

This does not replace the general artifact selection policy.  
It specializes artifact selection for delegation workflows.

---

### Relationship to Framework Reasoning

The handoff artifact does not replace structured reasoning.

The AI Interaction Framework remains responsible for:

- analytical structure  
- reasoning completeness  
- evaluation of options and constraints  

The handoff artifact represents the **output of completed reasoning**, formatted for downstream execution.

---

### Runtime Requirement

When delegated execution is active, the methodology must produce a handoff artifact that satisfies the required structure and quality characteristics defined in this section.

The system must not rely on conversational context alone to convey implementation intent.

---

## Cross-Domain Delegation Taxonomy

### Purpose

Define how delegated execution generalizes across different domains while preserving a consistent handoff model.

The taxonomy separates:

- domain-invariant delegation structure  
- domain-specific execution characteristics  

This allows the methodology to support delegation across multiple domains without redefining the handoff model for each case.

---

### Taxonomy Principle

Delegated execution consists of two layers:

1. **Invariant Handoff Structure**  
   The canonical handoff artifact defined by the methodology

2. **Domain-Specific Execution Context**  
   The downstream environment, tools, and implementation patterns used to execute the work

The methodology standardizes the first layer and allows controlled variation in the second.

---

### Domain Categories

Delegated execution may occur across multiple domains, including but not limited to:

#### Code Domain

Focus:

- implementation of software changes  
- code generation or modification  
- refactoring or debugging  

Execution environments:

- coding-specialized models  
- development environments  
- CI/CD pipelines  

---

#### Architecture Domain

Focus:

- system design  
- component interaction  
- infrastructure or platform structure  

Execution environments:

- design tooling  
- architecture modeling systems  
- technical design workflows  

---

#### Data Domain

Focus:

- data transformation  
- pipeline design  
- reporting or analytics implementation  

Execution environments:

- data platforms  
- ETL systems  
- analytics tooling  

---

#### Process Domain

Focus:

- workflow design  
- operational procedures  
- automation logic  

Execution environments:

- workflow systems  
- RPA platforms  
- operational tooling  

---

#### Strategy Domain

Focus:

- decision frameworks  
- planning structures  
- prioritization or sequencing  

Execution environments:

- human decision processes  
- planning systems  
- organizational workflows  

---

### Invariant Requirements

Across all domains, delegated execution must preserve:

- objective clarity  
- current-state diagnosis  
- explicit constraints and invariants  
- clearly defined required actions  
- bounded scope  
- explicit assumptions and uncertainty  
- validation expectations  

These requirements are enforced through the canonical handoff artifact structure.

---

### Domain-Specific Variation

While the handoff structure is invariant, the following elements may vary by domain:

- terminology used in the execution prompt  
- level of implementation detail required  
- representation of actions (code, steps, configurations, plans)  
- validation mechanisms (tests, simulations, review processes)  
- execution constraints imposed by the downstream environment  

The methodology does not prescribe domain-specific formats for these elements.

---

### Execution Context Awareness

When delegated execution is active, the handoff artifact should reflect awareness of the downstream execution context.

This may include:

- expected capabilities of the downstream system  
- constraints of the execution environment  
- required level of specificity  
- known limitations of the target system  

This ensures that the handoff artifact is usable without reinterpretation.

---

### Non-Goals

The taxonomy does not:

- define domain-specific templates  
- prescribe implementation syntax for any domain  
- replace the canonical handoff artifact structure  
- introduce domain-specific reasoning frameworks  

All domains must continue to use the same underlying methodology.

---

### Relationship to Handoff Artifact Specification

The handoff artifact specification defines the structure of delegation.

The cross-domain taxonomy defines how that structure applies across different execution contexts.

This section does not modify the artifact structure.  
It clarifies how the same structure remains valid across domains.

---

### Methodology Requirement

Implementations must treat delegated execution as a domain-agnostic capability.

The methodology must not assume:

- a single domain of execution  
- a single type of downstream system  
- a fixed representation of implementation  

All delegation behavior must be compatible with multiple execution domains while preserving the invariant handoff structure.

---

## Additive and Replacement Behavior

Not all directives resolve through simple override.

### Replacement Directives

Single-value directives resolve by replacement.

Examples include:

- tone intensity
- response density
- response structure
- default framework tier
- output formality

For these directives, the highest-precedence valid value wins.

---

### Additive Directives

Multi-value directives may accumulate compatible values.

Examples include:

- systems lens emphasis
- non-structural analytical emphasis
- optional artifact preferences

Additive merging is only allowed where accumulated values do not alter canonical semantics or create internal contradiction.

---

### Restrictive Directives

Constraint-like directives resolve through narrowing rather than accumulation.

Examples include:

- scope strictness
- governance limitations
- profile boundaries
- response restrictions

When multiple restrictive directives apply, the effective runtime behavior should use the narrowest valid result.

---

### Derived Directives

Some directives are not directly overridden at all and must be determined from runtime conditions.

Examples include:

- active framework tier
- governance activation
- presentation mode
- artifact selection

These directives are computed during execution using canonical rules, profile defaults, and task context.

---

## Conflict Resolution Rule

When two directives target the same concern, runtime resolution should follow this sequence:

1. determine the directive category of each input  
2. determine whether the directive is structural, replacement, additive, restrictive, or derived  
3. apply the precedence rules for that category  
4. reject any attempt to override canonical semantics  
5. compute the effective runtime value

This process ensures that runtime behavior remains deterministic, reviewable, and reproducible.

---

## Architectural Rationale — Configuration and Directive Resolution

The methodology separates:

- structural semantics
- behavioral defaults
- profile tuning
- task-derived runtime decisions

For this separation to remain operationally reliable, precedence must be defined at the directive level rather than only at the document level.

This model preserves:

- canonical integrity
- deterministic runtime behavior
- safe profile customization
- compatibility with governed organizational environments

---

## Deterministic Runtime Assembly

The runtime configuration may be conceptually expressed as:

```
load_methodology()

resolve_framework()
resolve_collaboration_guidelines()

runtime_configuration.canonical_semantics =
    methodology + framework

runtime_configuration.behavior_defaults =
    collaboration_guidelines

if collaboration_profile_present:
    runtime_configuration.behavior_defaults =
        apply_profile_overrides()

runtime_configuration.runtime_context =
    derived_from_task
```

This layered assembly ensures:

- canonical analytical semantics remain immutable
- collaboration behavior can be safely customized
- runtime behavior remains deterministic and reproducible.

---

## Framework Tier Selection Policy

The AI Interaction Methodology supports multiple framework tiers so that analytical rigor can be matched to the needs of the task.

To ensure deterministic runtime behavior, implementations must apply explicit rules when selecting the active framework tier.

This section defines the framework tier selection model.

---

## Available Framework Tiers

The methodology supports the following framework tiers:

| Tier | Purpose |
|---|---|
| Core Framework | Standard structured reasoning for general analytical work |
| Advanced Framework | Expanded analytical reasoning for complex technical or decision-focused work |
| Governance Extensions | Additional governance controls for regulated, auditable, or enterprise-risk use cases |

Framework tiers are cumulative.

This means:

- Advanced includes the Core reasoning structure
- Governance extends the active reasoning structure with additional governance controls

---

## Framework Tier Selection Principle

The active framework tier should be the **lowest tier that fully satisfies the analytical and operational requirements of the task**.

Implementations must escalate to a higher tier when lower tiers would omit required analytical control, risk handling, or governance behavior.

This prevents unnecessary complexity while preserving sufficient rigor.

---

## Core Framework Selection

The Core Framework should be used when the task is primarily:

- explanatory
- descriptive
- advisory
- low-risk analytical work
- general structured reasoning without formal decision comparison or governance requirements

Typical examples include:

- clarifying a concept
- summarizing a design idea
- answering a bounded technical question
- producing a structured explanation
- performing straightforward analytical reasoning

The Core Framework is the default tier unless escalation conditions apply.

---

## Advanced Framework Selection

The Advanced Framework must be used when the task requires expanded analytical control beyond the Core Framework.

Advanced selection triggers include:

- system architecture analysis
- technical option comparison
- decision adjudication
- operational workflow analysis
- explicit tradeoff evaluation
- failure mode analysis
- maintainability analysis
- analysis requiring explicit assumptions or decision criteria

Typical examples include:

- comparing architectural approaches
- evaluating competing operational designs
- assessing long-term maintainability implications
- analyzing risks across multiple solution options
- performing deeper engineering review

When one or more Advanced selection triggers are present, the runtime must activate the Advanced Framework.

---

## Governance Extension Selection

Governance Extensions must be activated when the task occurs within a governed context requiring explicit risk, policy, accountability, or oversight controls.

Governance selection triggers include:

- regulatory or compliance impact
- enterprise policy scope
- externally visible or high-consequence outcomes
- auditable decision support
- formal risk management requirements
- required human oversight
- traceability or accountability obligations

Typical examples include:

- governed enterprise AI usage
- policy-sensitive decision support
- regulated operational recommendations
- analysis that must support audit or review

When one or more governance triggers are present, the runtime must activate Governance Extensions in addition to the otherwise required reasoning tier.

---

## Tier Escalation Rules

Framework tier selection must follow these escalation rules:

1. begin with Core Framework as the default  
2. evaluate whether Advanced selection triggers are present  
3. if Advanced triggers are present, activate Advanced Framework  
4. evaluate whether Governance selection triggers are present  
5. if Governance triggers are present, activate Governance Extensions  

This produces the following valid runtime states:

- Core Framework
- Advanced Framework
- Advanced Framework + Governance Extensions

If governance controls are required for a task that would otherwise fit within Core reasoning, implementations may apply governance extensions together with the appropriate lower analytical tier.

---

## Task Category Mapping

The following table provides the default mapping between task types and framework tiers.

| Task Category | Default Tier |
|---|---|
| Simple explanation or bounded advisory | Core |
| General structured analysis | Core |
| Architecture review | Advanced |
| Option comparison | Advanced |
| Decision support with tradeoffs | Advanced |
| Failure mode or operational risk analysis | Advanced |
| Governed enterprise analysis | Advanced + Governance |
| Regulated or auditable decision support | Advanced + Governance |

This table provides default selection behavior.  
If multiple triggers apply, the higher required tier must be used.

---

## Runtime Selection Requirement

Framework tier selection must occur before structured reasoning begins.

The active tier must be selected using:

- task complexity
- analytical requirements
- risk exposure
- governance context

This ensures that the runtime activates the correct reasoning depth before analysis is performed.

---

## Governance Activation Criteria

Governance Extensions provide additional analytical controls intended for regulated, high-risk, or enterprise environments where decisions must satisfy explicit accountability, risk management, or policy alignment requirements.

To ensure consistent runtime behavior, implementations must apply explicit criteria when determining whether governance extensions should be activated.

---

## Governance Purpose

Governance Extensions add analytical controls focused on:

- risk visibility
- policy alignment
- auditability
- accountability
- human oversight

These controls extend the reasoning framework so that analytical outputs can support environments where decisions may require review, documentation, or formal validation.

Governance extensions do not replace the reasoning framework.  
They augment the active reasoning tier with additional validation and reporting requirements.

---

## Governance Activation Principle

Governance extensions must be activated whenever the analytical task involves outcomes that require **formal accountability, policy alignment, or explicit risk management**.

This ensures that analytical reasoning performed using the methodology remains compatible with organizational governance expectations.

---

## Governance Activation Triggers

Governance Extensions must be activated when one or more of the following conditions apply.

### Regulatory or Compliance Impact

The analysis influences or supports decisions subject to:

- regulatory oversight
- statutory requirements
- industry compliance obligations

Examples include:

- regulated operational environments
- compliance-sensitive recommendations
- policy enforcement scenarios

---

### Enterprise Policy Scope

The analysis affects decisions that must align with formal organizational policies.

Examples include:

- internal governance policies
- enterprise risk policies
- corporate decision frameworks

---

### Externally Visible Outcomes

The analysis contributes to outcomes visible outside the organization or to stakeholders beyond the immediate working group.

Examples include:

- customer-facing system behavior
- externally communicated decisions
- public operational outcomes

---

### Auditable Decision Support

The analytical output must support later audit, review, or formal justification.

Examples include:

- documented decision records
- architecture review documentation
- operational post-incident analysis

---

### Elevated Risk Exposure

The task involves meaningful operational, financial, or reputational risk.

Examples include:

- high-impact system changes
- operational risk analysis
- safety-sensitive environments

---

### Required Human Oversight

The analytical process must support human review or approval before implementation.

Examples include:

- decision recommendations requiring management approval
- risk acceptance documentation
- policy-sensitive operational changes

---

## Governance Escalation Rule

When governance activation triggers are present, the runtime must enable Governance Extensions in addition to the reasoning tier selected under the Framework Tier Selection Policy.

This produces the following valid runtime combinations:

- Core Framework
- Advanced Framework
- Core Framework + Governance Extensions
- Advanced Framework + Governance Extensions

Governance Extensions do not reduce analytical rigor.  
They add governance-specific controls on top of the active reasoning tier.

---

## Governance Controls

When governance extensions are active, the analytical process should incorporate additional evaluation dimensions including:

- risk identification
- policy alignment
- traceability of reasoning
- explicit documentation of assumptions and tradeoffs
- visibility of uncertainty and confidence levels

These controls improve the ability of the analysis to support formal review processes.

---

## Deterministic Governance Behavior

Governance activation must follow deterministic rules rather than discretionary use.

If governance activation criteria are satisfied, implementations must activate Governance Extensions even if the task might otherwise appear manageable using a lower analytical tier.

This requirement ensures consistent behavior across environments and prevents governance-sensitive tasks from being evaluated using insufficient analytical controls.

---

## Architectural Rationale — Runtime Tier Selection and Governance

The methodology introduces governance extensions so that structured analytical reasoning can be safely applied within regulated and enterprise environments.

Without explicit activation criteria, governance usage would depend on individual judgment, leading to inconsistent analytical rigor across similar tasks.

Deterministic governance activation ensures that analytical workflows remain compatible with environments requiring formal accountability, policy alignment, and auditable reasoning processes.

---

## Optional Local Collaboration Profile

A deployment may optionally include an **AI Collaboration Profile** as a local overlay.

The profile exists to support controlled customization of collaboration defaults for a particular user, team, organization, or environment.

Profiles may tune items such as:

- tone intensity
- response density
- preferred response structure
- critique explicitness
- artifact preference defaults
- framework surfacing behavior
- scope strictness
- systems analysis emphasis

Profiles are optional and are **not part of the canonical methodology**.

They may adjust **expression, emphasis, and defaults**, but they must not redefine the methodology’s core reasoning model or canonical artifact semantics.

---

## Collaboration Profile Schema

To ensure that collaboration profiles remain safe, machine-interpretable configuration overlays, profiles must follow a defined schema.

This section defines the canonical profile field model used by the AI Interaction Methodology.

Profiles may tune collaboration behavior and presentation defaults, but they do not alter canonical methodology semantics.

---

## Profile Schema Design Principle

Collaboration profile fields are grouped into three categories:

| Category | Purpose |
|---|---|
| Presentation Fields | Control expression, density, and formatting style |
| Analytical Emphasis Fields | Tune analytical visibility and collaboration emphasis |
| Runtime Preference Fields | Influence default runtime behavior without changing canonical semantics |

This categorization allows profiles to behave as typed configuration overlays rather than informal narrative documents.

---

## Required Profile Fields

A valid collaboration profile must define the following fields:

- `tone_intensity`
- `response_density`
- `response_structure`
- `critique_explicitness`
- `risk_visibility`
- `scope_strictness`
- `artifact_preference`
- `framework_surfacing`
- `default_framework_tier`
- `systems_lens_emphasis`
- `output_formality`

Each field must use an allowed value from the schema defined below.

---

## Field Categories

### Presentation Fields

These fields control how responses are expressed.

| Field | Purpose | Merge Behavior |
|---|---|---|
| `tone_intensity` | Controls tone strength and conversational intensity | replacement |
| `response_density` | Controls brevity versus detail | replacement |
| `response_structure` | Controls preferred response organization | replacement |
| `output_formality` | Controls professional versus informal presentation style | replacement |

---

### Analytical Emphasis Fields

These fields tune which analytical characteristics should be more visible during collaboration.

| Field | Purpose | Merge Behavior |
|---|---|---|
| `critique_explicitness` | Controls how directly critique is surfaced | replacement |
| `risk_visibility` | Controls how visibly risks and tradeoffs are surfaced | replacement |
| `artifact_preference` | Controls preference for structured artifacts versus narrative response | replacement |
| `framework_surfacing` | Controls whether framework structure is shown explicitly or kept implicit | replacement |
| `systems_lens_emphasis` | Defines default analytical lenses to emphasize | additive |

---

### Runtime Preference Fields

These fields influence runtime defaults without modifying canonical semantics.

| Field | Purpose | Merge Behavior |
|---|---|---|
| `scope_strictness` | Controls how tightly responses remain within the user’s stated scope | replacement |
| `default_framework_tier` | Defines the default reasoning tier to start from before runtime escalation rules apply | replacement |

---

## Allowed Values

### `tone_intensity`

Allowed values:

- `minimal`
- `calm`
- `moderate`
- `high`

Meaning:

Controls the intensity of tone and stylistic force used in responses.

---

### `response_density`

Allowed values:

- `minimal`
- `concise`
- `concise_complete`
- `detailed`

Meaning:

Controls how much explanation is included by default.

---

### `response_structure`

Allowed values:

- `freeform`
- `light_structure`
- `structured_sections`
- `formal_structure`

Meaning:

Controls the default organizational structure of responses.

---

### `critique_explicitness`

Allowed values:

- `low`
- `moderate`
- `high`

Meaning:

Controls how explicitly weaknesses, tradeoffs, and flaws are surfaced.

---

### `risk_visibility`

Allowed values:

- `implicit`
- `explicit_when_relevant`
- `always_explicit`

Meaning:

Controls whether risks and tradeoffs are surfaced only when materially relevant or consistently foregrounded.

---

### `scope_strictness`

Allowed values:

- `moderate`
- `high`
- `strict`

Meaning:

Controls how tightly the response remains bounded to the user’s stated request.

---

### `artifact_preference`

Allowed values:

- `narrative_default`
- `balanced`
- `practical_structured`
- `artifact_forward`

Meaning:

Controls whether responses should default toward prose or toward reusable structured artifacts.

---

### `framework_surfacing`

Allowed values:

- `implicit_default`
- `explicit_when_helpful`
- `explicit_default`

Meaning:

Controls whether the underlying reasoning framework is surfaced directly in the response.

---

### `default_framework_tier`

Allowed values:

- `core`
- `advanced`

Meaning:

Defines the default analytical tier used before task-based escalation rules are applied.

Governance activation is not set directly by profile; it is determined by runtime governance activation criteria.

---

### `systems_lens_emphasis`

Allowed values:

One or more of:

- `architecture`
- `maintainability`
- `operational_complexity`
- `failure_modes`
- `risk`
- `governance`
- `decision_quality`

Meaning:

Defines which analytical lenses should receive default emphasis when relevant.

This is the only standard schema field that is additive by default.

---

### `output_formality`

Allowed values:

- `informal`
- `working_session`
- `professional`
- `formal`

Meaning:

Controls the overall formality level of the response presentation.

---

## Validation Rules

A valid collaboration profile must satisfy the following conditions:

1. all required fields are present  
2. each field uses only allowed values  
3. single-value fields contain exactly one allowed value  
4. `systems_lens_emphasis` contains one or more allowed values  
5. the profile does not declare fields outside the schema unless a future methodology version explicitly permits extension fields  

Profiles that violate these rules should be treated as invalid configuration artifacts.

---

## Runtime Interpretation Rules

During runtime assembly:

- presentation fields tune response style
- analytical emphasis fields tune visibility and emphasis
- runtime preference fields influence default behavior prior to task-based runtime selection

No profile field may override:

- methodology invariants
- framework node definitions
- framework tier semantics
- governance activation criteria
- artifact resolution policy

Those restrictions are defined separately in the profile scope boundaries.

---

## Architectural Rationale — Collaboration Profiles

The collaboration profile system exists to support safe customization without creating derivative methodologies.

A typed schema is required so that profiles can be:

- validated
- compared
- interpreted consistently
- applied deterministically during runtime assembly

Without a schema, profiles remain informal documents and cannot reliably function as configuration overlays.

---

## Profile Scope Restrictions

Collaboration profiles are bounded configuration overlays.

They exist to tune collaboration behavior, response presentation, and limited runtime defaults without modifying the canonical methodology.

To preserve methodology integrity, profiles must operate within explicit scope restrictions.

---

## Profile Restriction Principle

Profiles may customize **expression, emphasis, and default behavior** only within the bounds defined by the methodology.

Profiles must not modify canonical semantics, redefine runtime contracts, or alter the required behavior of the methodology bootstrap.

If a profile directive conflicts with canonical methodology behavior, the canonical behavior must prevail.

---

## Profile-Adjustable Scope

Profiles may tune only the following categories of behavior:

### Presentation Behavior

Profiles may adjust how responses are expressed, including:

- tone intensity
- response density
- response structure
- output formality

### Analytical Emphasis

Profiles may adjust which analytical characteristics receive more visible emphasis, including:

- critique explicitness
- risk visibility
- artifact preference
- framework surfacing
- systems lens emphasis

### Runtime Defaults

Profiles may adjust limited default runtime preferences, including:

- scope strictness
- default framework tier

These preferences influence runtime defaults only.  
They do not redefine runtime selection rules.

---

## Prohibited Profile Modifications

Profiles must not modify any of the following.

### Methodology Invariants

Profiles must not alter or disable methodology invariants, including:

- diagnosis before solutioning
- structured reasoning over conversational response generation
- explicit handling of assumptions, tradeoffs, and uncertainty
- critical evaluation rather than automatic validation
- systems-level analytical orientation
- reliability validation before conclusions

---

### Framework Structure

Profiles must not modify the analytical structure of the framework, including:

- framework node definitions
- node meanings
- required reasoning structure
- tier composition

Profiles may influence whether framework structure is surfaced explicitly, but they may not alter the framework itself.

---

### Framework Tier Semantics

Profiles must not redefine what the framework tiers mean or when they are required.

This includes:

- Core Framework semantics
- Advanced Framework semantics
- Governance Extensions semantics
- tier escalation behavior

Profiles may set a default starting tier only where permitted by the schema.

Runtime tier selection remains governed by the framework tier selection policy.

---

### Governance Activation Criteria

Profiles must not alter governance admission or activation rules.

This includes:

- governance activation triggers
- governance escalation rules
- governance control requirements
- governance-related runtime obligations

Profiles may not disable governance behavior for tasks that satisfy governance activation criteria.

---

### Artifact Resolution Behavior

Profiles must not alter the bootloader’s artifact resolution rules.

This includes:

- canonical source resolution
- artifact failure handling
- degraded resolution policy
- artifact compatibility requirements
- pinned artifact compatibility behavior

Profiles may not change how canonical artifacts are resolved, validated, or rejected.

---

### Canonical Authority Relationships

Profiles must not redefine the authority relationships between:

- AI Interaction Methodology
- AI Collaboration Guidelines
- AI Interaction Framework
- optional collaboration profiles

Profiles remain subordinate to canonical methodology artifacts.

---

## Invalid Profile Behavior

A profile must be treated as invalid if it attempts to:

- introduce directives outside the allowed profile scope
- redefine canonical methodology behavior
- disable required runtime controls
- alter framework or governance semantics
- conflict with artifact resolution or compatibility policy

Invalid profile directives must be ignored.

If profile invalidity prevents safe interpretation of the profile as a whole, the implementation should reject the profile entirely.

---

## Runtime Enforcement Requirement

During runtime assembly, implementations must enforce profile scope restrictions before applying profile directives.

This means:

1. validate the profile against the schema  
2. validate the profile against scope restrictions  
3. reject or ignore invalid directives  
4. apply only the remaining valid profile directives  

Profiles must therefore be interpreted as constrained overlays, not unrestricted configuration sources.

---

## Architectural Rationale — Profile Scope Restrictions

The collaboration profile system exists to support safe customization without allowing silent mutation of the methodology itself.

Without explicit scope restrictions, profiles could become an alternate path for changing canonical semantics, which would undermine reproducibility, governance compatibility, and conformance.

Profile scope restrictions preserve the distinction between:

- configuration
- methodology
- runtime control
- governance obligation

This allows profiles to remain useful while preserving canonical integrity.

---

## Profile Composition Rules

The AI Interaction Methodology assumes that most deployments will provide a single collaboration profile.

However, implementations may encounter situations where multiple profiles are available simultaneously.

Examples include:

- organization-level default profiles
- team-specific collaboration profiles
- individual user preference profiles
- environment-specific runtime profiles

To preserve deterministic behavior, the methodology defines explicit composition rules for resolving multiple profiles.

---

## Profile Composition Principle

Profiles must compose as **bounded configuration overlays** rather than independent behavioral authorities.

When multiple profiles are present, implementations must resolve them deterministically to produce a single effective profile configuration.

Profile composition must not violate:

- canonical methodology semantics
- framework tier selection rules
- governance activation criteria
- artifact resolution behavior

---

## Profile Precedence Order

If multiple profiles are present, they must be resolved using the following precedence order:

1. organization profile  
2. team profile  
3. user profile  
4. runtime environment profile

Later profiles may override earlier profiles only within the boundaries allowed by the profile schema and scope restrictions.

If two profiles occupy the same precedence level, the implementation should select one deterministically based on deployment configuration.

---

## Composition Behavior by Field Type

Profile fields compose according to their merge behavior.

### Replacement Fields

Replacement fields resolve using **highest-precedence replacement**.

Examples include:

- tone intensity
- response density
- response structure
- critique explicitness
- risk visibility
- artifact preference
- framework surfacing
- scope strictness
- default framework tier
- output formality

For replacement fields, the value defined by the highest-precedence profile becomes the effective runtime value.

---

### Additive Fields

Additive fields accumulate compatible values from all profiles.

Currently, the only additive field defined by the schema is:

- systems_lens_emphasis

Additive composition must not produce contradictory analytical emphasis.

If incompatible values appear, implementations should retain only values consistent with canonical methodology semantics.

---

### Restrictive Fields

Restrictive fields resolve by selecting the **most restrictive valid value** across all profiles.

Examples include:

- scope strictness
- response boundaries
- governance sensitivity indicators

This rule preserves bounded customization and prevents profiles from weakening analytical discipline.

---

## Composition Failure Handling

Profile composition may fail if:

- profiles contain incompatible schema definitions
- profiles attempt to modify canonical semantics
- additive fields produce contradictory configurations
- multiple profiles at the same precedence level conflict irreconcilably

When composition failure occurs, implementations must apply one of the following strategies:

1. reject the conflicting profiles and continue using the remaining valid profiles  
2. reject all profiles and revert to canonical collaboration defaults  

Implementations must not silently produce undefined behavior.

---

## Effective Runtime Profile

After composition completes, implementations must treat the resulting configuration as a **single effective collaboration profile**.

This effective profile must satisfy:

- the collaboration profile schema
- profile scope restrictions
- directive precedence rules
- runtime task directives

Only the effective profile configuration should influence runtime collaboration behavior.

---

## Architectural Rationale — Profile Composition

Profile composition rules ensure that collaboration customization remains deterministic even when multiple configuration layers are present.

Without explicit composition rules, multiple profiles could introduce unpredictable overrides or weaken methodology invariants.

By defining:

- explicit precedence
- field-level merge behavior
- deterministic conflict handling

the methodology preserves both flexibility and canonical integrity.

---

## Conformance Checklist

Implementations claiming alignment with the AI Interaction Methodology should be evaluated against a defined conformance checklist.

This checklist provides a practical validation mechanism for determining whether an implementation preserves the methodology’s required analytical and runtime behaviors.

Conformance is assessed against the canonical methodology document, the canonical AI Collaboration Guidelines, the canonical AI Interaction Framework, and any bounded profile behavior permitted by this document.

---

## Conformance Principle

An implementation conforms to the AI Interaction Methodology only if it preserves the methodology’s canonical reasoning, runtime, and profile-boundary requirements.

Conformance requires more than superficial similarity in tone or structure.  
It requires preservation of the methodology’s defined analytical discipline, runtime control behavior, and canonical authority relationships.

---

## Required Conformance Criteria

An implementation should satisfy all of the following criteria.

### 1. Diagnosis Precedes Solutioning

The implementation must require analytical diagnosis before proposing solutions or recommendations.

Evidence of conformance may include:

- explicit problem framing
- structured evaluation before recommendation
- avoidance of premature conclusions

---

### 2. Assumptions Are Explicit

The implementation must surface assumptions that materially affect reasoning.

Evidence of conformance may include:

- explicit assumption statements
- distinction between known facts and inferred conditions
- identification of missing information

---

### 3. Tradeoffs Are Identified

The implementation must identify meaningful tradeoffs when comparing options or forming recommendations.

Evidence of conformance may include:

- explicit tradeoff discussion
- comparison across competing priorities
- visibility into what is gained or sacrificed by a choice

---

### 4. Uncertainty Is Acknowledged

The implementation must communicate uncertainty, confidence limits, or ambiguity where they materially affect reasoning quality.

Evidence of conformance may include:

- explicit uncertainty statements
- confidence qualifiers
- identification of information that could change the analysis

---

### 5. Framework Tier Selection Is Appropriate

The implementation must apply the appropriate framework tier for the task.

Evidence of conformance may include:

- Core Framework used for standard structured reasoning
- Advanced Framework used when deeper analytical control is required
- Governance Extensions activated when governance criteria are satisfied

---

### 6. Reliability Validation Is Performed

The implementation must include a reliability validation step before final conclusions are produced.

Evidence of conformance may include:

- validation of assumptions
- identification of reasoning limitations
- identification of potential failure modes
- verification that conclusions follow from the analysis

---

### 7. Governance Is Used When Required

The implementation must activate governance controls when governance activation criteria are satisfied.

Evidence of conformance may include:

- risk visibility
- policy alignment checks
- auditability support
- human oversight support where required

---

### 8. Profiles Do Not Override Canonical Rules

If collaboration profiles are used, they must remain bounded overlays and must not alter canonical methodology semantics.

Evidence of conformance may include:

- profile schema validation
- profile scope enforcement
- rejection or ignoring of invalid profile directives
- preservation of canonical framework and governance behavior

---

### 9. Evidence-Bound Workflows Preserve Source Fidelity

For workflows operating under evidence-bound operation classes, the implementation must preserve source fidelity and must not introduce inferred or reconstructed base content.

Evidence of conformance may include:

- absence of fabricated or reconstructed source material
- clear separation between extracted evidence and inferred or synthesized content
- adherence to evidence stage gating conditions prior to analysis
- preservation of lineage and traceability across source-derived stages
- explicit handling of evidence integrity failures without silent continuation

---

## Conformance Evaluation Result

An implementation should be considered conformant only if all required criteria are satisfied.

If one or more required criteria are not satisfied, the implementation should be treated as:

- partially conformant, if the methodology is used only in limited form, or
- non-conformant, if canonical behavior is materially altered or omitted

Implementations should not claim full alignment with the AI Interaction Methodology unless all required criteria are met.

---

## Conformance Evidence

Conformance evaluation may be supported using evidence such as:

- methodology-aware prompts or runtime instructions
- framework tier selection behavior
- governance activation behavior
- profile validation and enforcement behavior
- documented analytical outputs demonstrating required methodology characteristics

The checklist is intended to support practical validation, not merely aspirational alignment statements.

---

## Architectural Rationale — Conformance Validation

The methodology defines a structured runtime and reasoning system.

Without a conformance checklist, implementations could claim alignment while omitting critical behaviors such as deterministic runtime control, explicit uncertainty handling, governance activation, or profile-boundary enforcement.

A conformance checklist converts the methodology from descriptive guidance into a verifiable implementation standard.

---

## Canonical Compliance Statement

Implementations may claim alignment with the AI Interaction Methodology only when they preserve the canonical analytical, runtime, and governance behaviors defined by this document.

To reduce ambiguity and prevent misleading alignment claims, the methodology defines a standardized compliance statement.

---

## Compliance Principle

Claims of compliance must reflect the actual scope of implementation.

An implementation should not claim full alignment with the AI Interaction Methodology unless the core methodology behaviors, framework runtime controls, and profile boundary rules are preserved.

Compliance statements must therefore distinguish between:

- full conformance
- partial conformance
- methodology-inspired implementations

---

## Full Compliance Statement

An implementation may use the following statement only when all conformance criteria are satisfied.

```
This implementation conforms to the AI Interaction Methodology and preserves the canonical analytical, runtime, and governance behaviors defined by the methodology and its associated canonical artifacts.
```

Full compliance requires:

- satisfaction of the Conformance Checklist
- correct framework tier selection behavior
- correct governance activation behavior
- enforcement of profile scope restrictions
- preservation of canonical artifact resolution behavior

---

## Partial Compliance Statement

If an implementation adopts only some elements of the methodology, it must use a partial compliance statement.

Recommended wording:

```
This implementation incorporates elements of the AI Interaction Methodology but does not implement the full methodology runtime or governance model.
```

Partial compliance should describe which portions of the methodology are implemented.

Examples may include:

- collaboration guidelines only
- framework reasoning structure without runtime tier control
- limited profile behavior without full schema validation

---

## Methodology-Inspired Statement

If an implementation merely adopts similar ideas without following the methodology’s formal structures, it should avoid claims of conformance.

Recommended wording:

```
This implementation is informed by concepts from the AI Interaction Methodology but does not claim formal conformance.
```

This statement should be used when:

- the framework structure is altered
- governance behavior is omitted
- runtime tier selection is not implemented
- profile boundaries are not enforced

---

## Compliance Transparency

Implementations claiming full or partial compliance should provide transparency regarding:

- which canonical artifacts are used
- which framework tier behaviors are implemented
- whether governance extensions are supported
- whether collaboration profiles are supported and validated

Transparency helps reviewers determine whether compliance claims are accurate.

---

## Compliance Verification

Compliance may be evaluated using:

- the Conformance Checklist
- review of methodology-aware prompts or runtime instructions
- inspection of framework tier selection behavior
- inspection of governance activation behavior
- validation of collaboration profile enforcement

The Canonical Compliance Statement is therefore intended to support accurate alignment claims rather than informal association with the methodology.

---

## Architectural Rationale — Canonical Compliance

Without a standardized compliance statement, implementations may claim alignment with the methodology while omitting critical behaviors such as deterministic runtime control, governance activation, or profile boundary enforcement.

The Canonical Compliance Statement ensures that:

- alignment claims remain meaningful
- adopters communicate implementation scope clearly
- governance-sensitive environments can assess methodology usage with confidence

---

