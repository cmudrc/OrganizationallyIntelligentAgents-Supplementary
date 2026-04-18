# Classification Rationale for OIA Taxonomy

This document provides the reasoning behind each paper's classification in the Organizationally-Intelligent Agents (OIA) taxonomy. The taxonomy consists of two dimensions:

**Organizational Structure:**
- **Sequential**: Agents execute in a fixed linear order
- **Networked**: Agents collaborate as peers without central coordination
- **Orchestrated**: A dedicated coordinator manages agent interactions

**Operational Methodology:**
- **Iterative-Feedback**: Agents refine outputs through feedback loops
- **Staged-Pipeline**: Fixed phases transform inputs to outputs
- **Graph-Routed**: Dynamic routing determines execution paths

---

## Summary Statistics (n=30)

| Organizational Structure | Count | Percentage |
|--------------------------|-------|------------|
| Orchestrated | 16 | 53% |
| Networked | 8 | 27% |
| Sequential | 6 | 20% |

| Operational Methodology | Count | Percentage |
|-------------------------|-------|------------|
| Iterative-Feedback | 15 | 50% |
| Staged-Pipeline | 7 | 23% |
| Graph-Routed | 8 | 27% |

---

## Paper Classifications

### 1. turbulence.ai: an end-to-end AI Scientist for fluid mechanics
**Citation:** `feng2025turbulence`

- **Organizational Structure: SEQUENTIAL.** It follows a "three-stage, multi-agent architecture" (Idea Generation, Simulation, Draft Write-Up) where one stage passes its output to the next in a linear progression.
- **Operational Methodology: STAGED-PIPELINE.** The workflow is explicitly divided into "five distinct phases" that transform a research idea into a manuscript PDF via a fixed sequence.

---

### 2. MechAgents: LLM multi-agent collaborations
**Citation:** `ni2024mechagents`

- **Organizational Structure: ORCHESTRATED.** The system utilizes a "Group chat manager" agent that repeats steps to "dynamically select a speaker" and manage the group.
- **Operational Methodology: ITERATIVE-FEEDBACK.** It relies on "self- and mutual-corrections" and "continuous conversation" to iteratively debug scripts until results are valid.

---

### 3. Power Electronics Design
**Citation:** `cui2024large`

- **Organizational Structure: ORCHESTRATED.** The framework utilizes a "Manager Agent" to parse user demands and assign sub-tasks to functional agents.
- **Operational Methodology: ITERATIVE-FEEDBACK.** The process involves "iterative refinement" where agents respond to high-level instructions to improve control design.

---

### 4. Alloy Design (AlloyAgents)
**Citation:** `ghafarollahi2024rapid`

- **Organizational Structure: NETWORKED.** The study highlights agents with "distinct roles and expertise that dynamically collaborate" to explore materials.
- **Operational Methodology: ITERATIVE-FEEDBACK.** It employs an "iterative feedback loop" between a planner and a reviewer to optimize alloy structures.

---

### 5. Materials Laws Discovery
**Citation:** `hu2024multi`

- **Organizational Structure: NETWORKED.** Peer agents act as generation, translation, and reflection nodes without a central orchestrator.
- **Operational Methodology: ITERATIVE-FEEDBACK.** It utilizes "repeated Depth-First Search (DFS) iterations" to refine and store formulas in long-term memory.

---

### 6. Factorio Systems Engineering
**Citation:** `kant2025develop`

- **Organizational Structure: ORCHESTRATED.** Built on the "Viable System Model," which is a management hierarchy with specialized levels for policy and coordination.
- **Operational Methodology: STAGED-PIPELINE.** The management levels operate as a structured stack of controls, moving from operational tasks up to high-level policy.

---

### 7. FROM IDEA TO CAD
**Citation:** `ocker2025idea`

- **Organizational Structure: SEQUENTIAL.** The architecture is designed to follow "established development processes" such as the "waterfall model".
- **Operational Methodology: STAGED-PIPELINE.** It explicitly mirrors the "V-model" phases, progressing from requirement clarification to design and handover.

---

### 8. CrossMatAgent: Metamaterial Design
**Citation:** `tian2025multi`

- **Organizational Structure: ORCHESTRATED.** A dedicated "Supervisor" agent is tasked with overseeing the entire design process to ensure property alignment.
- **Operational Methodology: ITERATIVE-FEEDBACK.** It features a "single iteration loop" where agents refine designs based on generative outcomes.

---

### 9. Marco: Hardware Design
**Citation:** `ho2025marco`

- **Organizational Structure: ORCHESTRATED.** The framework features a "Group Manager" responsible for configuring and coordinating agent nodes.
- **Operational Methodology: GRAPH-ROUTED.** It leverages "dynamic task graphs" where execution flows are determined by circuit relations and task plans.

---

### 10. Small Language Graph (SLG)
**Citation:** `bogachov2025lightweight`

- **Organizational Structure: ORCHESTRATED.** An "orchestrator" node serves as the primary entry point to coordinate domain-specific experts.
- **Operational Methodology: GRAPH-ROUTED.** The system "connects expert nodes using a graph approach" to route queries through specialized knowledge paths.

---

### 11. MenTeR: RF/Analog Circuits
**Citation:** `chen2025menter`

- **Organizational Structure: ORCHESTRATED.** It features a "Meta Agent" that acts as the central orchestrator to delegate circuit components to specialists.
- **Operational Methodology: STAGED-PIPELINE.** The methodology follows a "Chain-of-Stage (CoS)" approach, where the design is methodically advanced through prescribed stages.

---

### 12. Foundation Design Automation
**Citation:** `youwai2025investigating`

- **Organizational Structure: ORCHESTRATED.** It employs a "router multi-agent subsystem" to manage adaptive task distribution.
- **Operational Methodology: GRAPH-ROUTED.** The workflow uses "context-aware routing decisions" to direct tasks based on foundation type.

---

### 13. Automotive Styling
**Citation:** `jin2025closed`

- **Organizational Structure: NETWORKED.** The framework consists of "collaborative sub-agents" that work together on creative exploration.
- **Operational Methodology: ITERATIVE-FEEDBACK.** It utilizes a "search-reflect" iterative loop to continuously refine design queries based on market analysis.

---

### 14. MASSE: Structural Engineering
**Citation:** `liang2025automating`

- **Organizational Structure: ORCHESTRATED.** The specialized roles are "orchestrated through the AutoGen" framework.
- **Operational Methodology: ITERATIVE-FEEDBACK.** It mirrors "expert iteration" loops to reduce hours of manual design to minutes of automated checking.

---

### 15. Engineering.ai: Computational Design
**Citation:** `xu2025engineering`

- **Organizational Structure: ORCHESTRATED.** The framework is governed by an "LLM controller" that guides specialized agents.
- **Operational Methodology: ITERATIVE-FEEDBACK.** It implements a "closed-loop, self-correcting architecture" using iterative error correction.

---

### 16. Knowledge-Guided NACA Design
**Citation:** `kumar2025toward`

- **Organizational Structure: ORCHESTRATED.** A human "Manager" acts as an orchestrator and gatekeeper to terminate the design-review cycle.
- **Operational Methodology: ITERATIVE-FEEDBACK.** It formalizes a "structured iterative design and review" loop between Design and Systems engineers.

---

### 17. MDO Agent
**Citation:** `guo2025multidisciplinary`

- **Organizational Structure: NETWORKED.** It is described as a "synergistic multi-agent system" where agents work in tandem.
- **Operational Methodology: ITERATIVE-FEEDBACK.** The agent conducts evaluation with "iterative optimization" to refine candidate concept variants.

---

### 18. GridMind: Power System Analysis
**Citation:** `jin2025gridmind`

- **Organizational Structure: ORCHESTRATED.** It utilizes an "agent coordinator" that manages all inter-agent communication.
- **Operational Methodology: ITERATIVE-FEEDBACK.** It follows a "reason-act-reflect" loop where solver results are validated and narrated.

---

### 19. AutoForma: CAD Automation
**Citation:** `liao2024autoforma`

- **Organizational Structure: SEQUENTIAL.** It is a pipeline where agents perform tasks across "four primary stages".
- **Operational Methodology: STAGED-PIPELINE.** It follows a fixed sequence: Analysis → Planning → Coding → Execution.

---

### 20. DesignGPT: Product Design
**Citation:** `ding2023designgpt`

- **Organizational Structure: NETWORKED.** It simulates a "Meeting Room" where agents "simulate the roles of different positions" to collaborate.
- **Operational Methodology: ITERATIVE-FEEDBACK.** The system uses "design thinking" to support designers in completing conceptual designs iteratively.

---

### 21. Senior Design Project Copilot
**Citation:** `mushtaq2025harnessing`

- **Organizational Structure: ORCHESTRATED.** It utilizes a "Coordinator Agent" to oversee task execution among specialized experts.
- **Operational Methodology: STAGED-PIPELINE.** Role-playing AI agents are organized as a "cohesive 'crew' to complete tasks" in a prescribed workflow.

---

### 22. MEDA: Parametric CAD
**Citation:** `panta2025meda`

- **Organizational Structure: NETWORKED.** It implements a "division of labor with mutual corrections" among specialized agent peers.
- **Operational Methodology: GRAPH-ROUTED.** Transitions between agents are constrained and determined by a "finite state machine (FSM)".

---

### 23. Mechatronics Design
**Citation:** `wang2025llm`

- **Organizational Structure: ORCHESTRATED.** Governed by a "High-Level Planning Agent" that decomposes challenges for domain agents.
- **Operational Methodology: ITERATIVE-FEEDBACK.** It employs an "iterative design process" to refine propellers and hulls based on validation feedback.

---

### 24. AtomAgents: Alloy Discovery
**Citation:** `ghafarollahi2025automating`

- **Organizational Structure: NETWORKED.** Team of agents "collaborate autonomously" within a synergistic core-and-tool strategy.
- **Operational Methodology: ITERATIVE-FEEDBACK.** Agents perform "iterative evaluation" and self-correction to refine materials based on molecular data.

---

### 25. Elicitron: Requirements Engineering
**Citation:** `ataei2025elicitron`

- **Organizational Structure: SEQUENTIAL.** It uses a "serial" generation approach where each agent acts as context for the next in line.
- **Operational Methodology: STAGED-PIPELINE.** Follows a fixed process: Agent Generation → Simulation → Interview → Needs Identification.

---

### 26. Cost-Aware MAS
**Citation:** `chen2025cost`

- **Organizational Structure: NETWORKED.** It models the "collaboration between multiple rational agents" operating in distinct regions.
- **Operational Methodology: GRAPH-ROUTED.** Decisions on where to sample and when to stop are determined by "cost-aware routing logic".

---

### 27. Conceptual Systems Engineering
**Citation:** `massoudi2025agentic`

- **Organizational Structure: ORCHESTRATED.** Features a "Supervisor agent (SU)" that "oversees execution" and controls advancement.
- **Operational Methodology: GRAPH-ROUTED.** The framework "leverages a graph-based approach" (Design State Graph) to capture and route refinements.

---

### 28. Car Design
**Citation:** `elrefaie2025ai`

- **Organizational Structure: SEQUENTIAL.** The paper explicitly categorizes its agents into "Sequential, Hierarchical, and Hybrid" structures, noting that car design involves "sequential dependencies" where one agent must complete a task (e.g., 2D sketching) before the next begins (e.g., 3D styling).
- **Operational Methodology: ITERATIVE-FEEDBACK.** Within this sequential workflow, certain tasks like "styling and aerodynamic simulation can be iterated independently." This "Hybrid" approach combines a Sequential stage-to-stage handoff with an Iterative-Feedback methodology for refining specific components of the car.

---

### 29. Satellite Mission Design
**Citation:** `navarro2025autonomous`

- **Organizational Structure: ORCHESTRATED.** Features an "AI Study Manager" central coordinator managing a crew of specialists.
- **Operational Methodology: GRAPH-ROUTED.** The Study Manager "dynamically assigns tasks" and "revisits prior assumptions" based on real-time assessments.

---

### 30. DesAgent: Mechanical Design
**Citation:** `zhang2025desagent`

- **Organizational Structure: SEQUENTIAL.** Although the system features a Task Planner for coordination, the system executes its optimized sequence in a pipeline fashion where agents follow a determined order.
- **Operational Methodology: GRAPH-ROUTED.** The Task Planner creates a "structured task graph" that defines a "logical sequencing of the agents." While the execution appears Sequential (Stage A → Stage B), the determination of that sequence is dynamic and based on multidisciplinary coupling analysis, making its underlying methodology Graph-Routed.

---

## 3×3 Taxonomy Grid

| | Sequential | Networked | Orchestrated |
|---|---|---|---|
| **Iterative-Feedback** | Elrefaie | Ghafarollahi (2024), Hu, Jin (Automotive), Guo, Ding, Ghafarollahi (2025) | Ni, Cui, Tian, Liang, Xu, Kumar, Jin (GridMind), Wang |
| **Graph-Routed** | Zhang | Panta, Chen (Cost) | Ho, Bogachov, Youwai, Massoudi, Navarro |
| **Staged-Pipeline** | Feng, Ocker, Liao, Ataei | — | Kant, Chen (MenTeR), Mushtaq |
