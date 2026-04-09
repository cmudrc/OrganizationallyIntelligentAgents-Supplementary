# Organizational Design Mapping Methodology

This document describes the methodology used to map taxonomy categories to organizational design (OD) concepts, addressing how the 3-6 "most relevant" concepts were selected for each category in Table 4 of the paper.

## Overview

The mapping process connected each taxonomy category (Orchestrated, Networked, Sequential for Organizational Structure; Iterative-Feedback, Graph-Routed, Staged-Pipeline for Operational Methodology) to established organizational design concepts from the management science literature. The goal was to identify which OD mechanisms each architectural pattern *inherently invokes* by virtue of its structure, regardless of whether current MAS implementations explicitly engage these concepts.

## Source Material

The primary source for OD concepts was Joseph and Sengul's comprehensive survey "Organizational Configurations" (2025), which reviews organizational design research from 2000-2023 across four theoretical approaches:

| Approach | Focus | Example Concepts |
|----------|-------|------------------|
| **Configuration** | How organizations structure and group activities | Decomposition, modularity, near-decomposability, mirroring hypothesis |
| **Control** | How organizations monitor and direct behavior | Span of control, oversight, locus of authority, information asymmetry |
| **Channelization** | How organizations direct attention and information flow | Aspiration levels, structural distribution of attention, problemistic search |
| **Coordination** | How organizations align interdependent activities | Common ground, integrator roles, predictive knowledge, trans-specialist knowledge |

## Organizational Design Concept Definitions

All OD concepts used in the mapping are defined below, drawn from Joseph and Sengul (2025). These definitions grounded the selection process and provide the theoretical basis for mapping to MAS taxonomy categories.

### Configuration Concepts

| Concept | Definition |
|---------|------------|
| **Decomposition** | Breaking complex systems into smaller, more manageable modules or sub-units that can be addressed independently |
| **Modularity** | Designing self-contained units with clear interfaces that confine interdependencies within rather than across boundaries |
| **Near-decomposability** | Property where subsystems interact strongly internally but weakly with other subsystems, enabling semi-independent operation |
| **Mirroring hypothesis** | The principle that organizational structure should mirror the technical architecture of the system being designed |
| **Viscosity** | The time required for changes in one part of the system to propagate through to other parts |

### Control Concepts

| Concept | Definition |
|---------|------------|
| **Span of control** | The number of subordinates a manager can effectively coordinate; determines capacity limits for centralized oversight |
| **Oversight** | Use of hierarchical authority to monitor subordinate activities and provide corrective feedback |
| **Information asymmetry** | Condition where subordinates possess more detailed task-specific knowledge than their managers |
| **Locus of authority** | The degree to which decision-making rights are centralized in managers versus distributed to workers |

### Channelization Concepts

| Concept | Definition |
|---------|------------|
| **Aspiration levels** | Performance thresholds that trigger search behavior when not met; determines when to continue versus stop iterating |
| **Structural distribution of attention** | How organizational structures direct focus toward certain issues, tasks, or information streams |
| **Problemistic search** | Search behavior triggered by performance falling below aspiration levels rather than optimization-seeking |
| **Managerial frames** | Cognitive lenses that shape how managers interpret signals and evaluate what constitutes "good enough" |
| **Omission vs. commission** | Trade-off between avoiding bad actions (commission errors) versus missing good opportunities (omission errors) |
| **Coupled search** | How higher-level choices constrain or shape the search space available to lower-level actors |
| **Internal representations** | Simplified mental models that actors use to manage uncertainty and complexity |
| **Ambidexterity** | The capacity to simultaneously engage in exploration (trying new alternatives) and exploitation (refining current solutions) |
| **False negative avoidance** | Preventing premature stopping when feedback is misleading; avoiding convergence to local optima |

### Coordination Concepts

| Concept | Definition |
|---------|------------|
| **Common ground** | Shared knowledge that is mutually known to be shared; enables coordination without explicit communication |
| **Peer monitoring** | Coworkers observing and providing feedback on each other's work without hierarchical authority |
| **Trans-specialist knowledge** | Cross-functional understanding that allows specialists to coordinate without a dedicated integrator |
| **Joint myopia** | Risk that shared information sources lead all members toward the same suboptimal patterns |
| **Predictive knowledge** | One actor's ability to accurately anticipate another's actions, enabling implicit coordination |
| **Integrator roles** | Roles specifically designed to channel information flow and coordinate across specialist boundaries |

## Coder and Process Transparency

The mapping was performed by a single coder (the first author) using the process described below. While multi-coder approaches with inter-rater reliability assessment are preferable for interpretive coding tasks, the structured nature of this mapping—working from explicit definitions in a single source (Joseph & Sengul, 2025) with documented selection criteria—reduces subjectivity. The mapping was completed in one pass with the fixed criteria established beforehand.

## Note on Concept Counts

The paper refers to "3-6 most relevant OD concepts" in the methods and "5 most relevant concepts" in results tables. This variation reflects:

1. **Target range**: The methodology aimed to identify 3-6 concepts per category, allowing flexibility based on how many concepts met all three selection criteria for each category.

2. **Actual outcomes**: Most categories yielded exactly 5 concepts that met all criteria, which is why tables display 5 concepts per category.

3. **Consistency**: All taxonomy categories in the final mapping contain 5 concepts, representing the concepts that best satisfied the selection criteria for each category.

## Mapping Process

### Step 1: Identify Primary OD Approaches per Category

Each taxonomy category was first matched to the OD approach(es) most relevant to its defining coordination mechanism:

| Taxonomy Category | Primary OD Approaches | Reasoning |
|-------------------|----------------------|-----------|
| **Orchestrated** | Control + Coordination | Manager-led structure inherently involves oversight, span limitations, and integration across specialists |
| **Networked** | Coordination + Channelization | Peer coordination requires shared understanding and distributed attention allocation |
| **Sequential** | Configuration + Coordination | Stage-based decomposition invokes modularity principles and interface management |
| **Iterative-Feedback** | Channelization + Configuration | Convergence-based iteration involves aspiration levels and performance gap detection |
| **Graph-Routed** | Channelization + Configuration | Dynamic routing involves attention allocation and coupled search decisions |
| **Staged-Pipeline** | Configuration + Channelization | Prescribed phases invoke decomposition and structural attention distribution |

### Step 2: Concept Identification

Within the identified OD approaches, all potentially applicable concepts were noted. For each taxonomy category, this produced an initial list of 8-15 candidate concepts.

### Step 3: Concept Selection

From the candidate list, 3-6 concepts were selected for each category based on three criteria applied jointly:

**Criterion 1: Centrality to Defining Mechanism**
The concept must address a challenge that is *inherent* to the architectural pattern, not merely possible or occasional. For example:
- Span of control is *inherent* to Orchestrated systems (any manager agent faces capacity limits)
- Information asymmetry is *inherent* to Orchestrated systems (orchestrators route tasks without full specialist knowledge)

**Criterion 2: Practical Implications for MAS Design**
The concept must have actionable implications for how MAS architectures could be designed or evaluated. Concepts were favored if they suggest:
- Design parameters that could be explicitly optimized (e.g., span of control → agent count decisions)
- Failure modes that could be anticipated (e.g., joint myopia → search diversity requirements)
- Mechanisms that could be deliberately implemented (e.g., common ground → shared memory design)

**Criterion 3: Distinctiveness Across Categories**
The concept must help differentiate one category from another rather than applying generically to all architectures. For example:
- Span of control distinguishes Orchestrated (centralized coordination capacity) from Networked (no central coordinator)
- Common ground distinguishes Networked (peer coordination requirement) from Orchestrated (coordinator mediates)

### Step 4: Exclusion Decisions

Concepts were excluded from the final mapping if they:

1. Failed to meet all three selection criteria (e.g., relevant but not distinctive, or distinctive but lacking practical MAS implications)

2. Were subsumed by a more central concept (e.g., if "oversight" and "monitoring" both applied, the more comprehensive term was retained)

3. Could not be included due to space constraints in the paper format (table space limitations required prioritizing the most essential concepts)

Excluded concepts are not irrelevant—they may provide additional analytical depth in future work—but the selected concepts represent the most essential OD mechanisms for each category.

## Validation Approach

Mappings were validated by verifying that:

1. **Definitional alignment**: Each selected concept's definition (per Joseph & Sengul) logically applies to the taxonomy category's defining mechanism

2. **Mutual exclusivity**: Concepts mapped to one category do not equally apply to all other categories (distinctiveness check)

3. **Completeness**: The selected concepts collectively address the primary coordination challenges the category faces

Validation was performed against the theoretical definitions of OD concepts, not against the 30 MAS papers in the corpus. This is intentional: the mapping identifies what OD mechanisms each architecture *inherently invokes*, which is independent of whether current implementations explicitly discuss these mechanisms. Indeed, the paper's central finding is that MAS implementations engage these concepts superficially despite their inherent relevance.

## Mapping Summary

The final mappings are:

### Organizational Structure

| Category | Primary Approaches | Selected Concepts |
|----------|-------------------|-------------------|
| **Orchestrated** | Control + Coordination | Span of control, Oversight, Information asymmetry, Locus of authority, Integrator roles |
| **Networked** | Coordination + Channelization | Common ground, Peer monitoring, Trans-specialist knowledge, Joint myopia, Predictive knowledge |
| **Sequential** | Configuration + Coordination | Decomposition, Modularity, Near-decomposability, Mirroring hypothesis, Viscosity |

### Operational Methodology

| Category | Primary Approaches | Selected Concepts |
|----------|-------------------|-------------------|
| **Iterative-Feedback** | Channelization + Configuration | Aspiration levels, Problemistic search, Ambidexterity, False negative avoidance, Managerial frames |
| **Graph-Routed** | Channelization + Configuration | Structural distribution of attention, Managerial frames, Omission vs. commission, Coupled search, Internal representations |
| **Staged-Pipeline** | Configuration + Channelization | Decomposition, Modularity, Aspiration levels, Structural distribution of attention, Mirroring hypothesis |

## Limitations

1. **Single-coder design**: The mapping was performed by one researcher without independent verification by additional coders. Inter-rater reliability cannot be assessed. However, the structured approach—explicit definitions from a single source, documented selection criteria, one-pass application—was designed to reduce subjectivity and enhance replicability.

2. **Source dependency**: The mapping relies primarily on Joseph and Sengul's synthesis of OD literature. Alternative OD frameworks, primary sources, or different survey papers might yield different concept selections or categorizations.

3. **Space constraints**: Some relevant concepts were excluded due to publication format limitations. The concepts presented represent the most essential mappings; extended analysis could incorporate additional concepts.

4. **Theoretical rather than empirical validation**: Mappings were validated against OD concept definitions, not empirically tested to confirm that these mechanisms affect MAS performance. Such empirical validation is identified as critical future work in the paper.

## References

Joseph, J., & Sengul, M. (2025). Organizational Configurations: Review and Agenda. *Journal of Management*.

Asimow, M. (1962). *Introduction to Design*. Prentice-Hall.
