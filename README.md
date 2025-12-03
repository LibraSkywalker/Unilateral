# Unilateral: The Epistemic Fabrication Engine
## 1. The Architectural Axioms: 
    
### The Four Planes 
| Plane (平面) | 针对 Active Entity (Worker)<br>*(如: Pods, Agents)* | 针对 Passive Entity (Data)<br>*(如: Datasets, Configs)* | **通用抽象 (General Abstraction)** |
| :--- | :--- | :--- | :--- |
| **Data Plane**<br>*(Substance)* | **Skillset (Capabilities)**<br>技能集：它能执行什么操作？<br>*(e.g., CUDA支持, Python库)* | **Schema (Properties)**<br>模式/属性：它能被如何读取？<br>*(e.g., 列定义, 压缩格式)* | **Definition (定义域)**<br>**它拥有什么潜能？(Potentials)**<br>内禀的静态属性。 |
| **Control Plane**<br>*(Order)* | **Orchestration (Policy)**<br>编排：它如何被调度？<br>*(e.g., 重试逻辑, 资源限制)* | **Lifecycle (Policy)**<br>生命周期：它如何流转？<br>*(e.g., 保留期, 冷热分层)* | **Mechanics (执行域)**<br>**它如何被操作？(Kinematics)**<br>外在的动态规则。 |
| **Cognitive Plane**<br>*(Meaning)* | **Role / Agent Type**<br>角色：它在系统中是谁？<br>*(e.g., "数据清洗工", "网关")* | **Semantic Meaning**<br>语义：它代表什么业务概念？<br>*(e.g., "2024年销售额")* | **Identity (认知域)**<br>**它代表什么意义？(Meaning)**<br>逻辑身份与元数据索引。 |
| **Interaction Plane**<br>*(Boundary)* | **API / Interface**<br>接口：如何向它发送指令？<br>*(e.g., gRPC, REST)* | **Access Protocol**<br>协议：如何获取它的内容？<br>*(e.g., FUSE mount, S3 get)* | **Boundary (交互域)**<br>**它如何被触达？(Visibility)**<br>可见性与访问边界。 |

### The Four Dimensions
| Fabrication Dimension | Active Worker | Passive Entity |
| :--- | :--- | :--- |
| **1. Spec** | Defines the execution logic through code references or image digests. | Defines the data structure through schema definitions and source locations. |
| **2. Config** | Applies runtime constraints such as compute quotas and environment variables. | Applies access controls such as mount paths and permission views. |
| **3. Instance** | Produces a dynamic process that consumes time and computational resources. | Produces a local handle or materialized view that occupies storage space. |
| **4. Termination** | The process stops, releasing compute resources and resetting state. | The mount detaches, removing the local view and reclaiming cache. |

### The Three Factors

| Factor | Focus | Core Definition (Business Logic) | Corresponds to Your Need |
| :--- | :--- | :--- | :--- |
| **Entity (E)**<br>*(Substance)* | **Identity & Substance**<br>(The Core) | **"Who am I?"**<br>The intrinsic, immutable core of the entity. Its unique ID and essential business properties (e.g., "This is a contract," "Here is its value"). | The nucleus of the entity dependency, the essence that does not change with the observer. |
| **Temporal (T)**<br>*(Flow)* | **State & Causality**<br>(The Lifecycle) | **"What stage am I at?"**<br>From a business process view: Is it a "draft," "pending approval," or "archived"? This defines its mutability in time. | The lifecycle and version progression of the entity. |
| **Scoping (S)**<br>*(Exposure)* | **Visibility & Exposure**<br>(The Interface) | **"What do I show you?"**<br>This is the entity's **surface area**. Based on the observer (Context), the entity decides which attributes to **expose** and which details to **mask**. | **"Need it to be visible during observation"**<br>**"Need to expose specific attributes"** |
---

## 2. Layer 3: The Landscape (The Canonical Zone Specification)

Layer 3 is the living territory where the system evolves. 

## Zone 0: Meta (World Definition)
*Before an entity exists, we must define what it means to "be" and what tools are available.*

Objective: Definition, Standardization, and Legislation. (Its purpose is to establish the rules, not to play the game.)

Context: Zone 0 does not contain specific projects or data. It contains the definitions that allow projects and data to exist. It establishes the "Standard Model" of the digital universe.

### Phenomenon 1: Ontological Anchoring
**The establishment of the cognitive framework.**

| Term | Definition within Zone 0 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Archetype** | The abstract template of an Entity. Defines required Planes (e.g., "All Services must have an API"). | **Cognitive Plane** (Identity) |
| **Taxonomy** | The hierarchical classification system (e.g., `System > Domain > Service`). | **Cognitive Plane** (Role) |
| **Semantics** | The dictionary of reserved business concepts (e.g., "GrossRevenue" vs "NetRevenue"). | **Cognitive Plane** (Meaning) |

### Phenomenon 2: Capability Registration
**The cataloging of potential.**

| Term | Definition within Zone 0 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Primitive** | The atomic units of technology (e.g., "Postgres 15", "Redis 7", "WASM Module"). | **Data Plane** (Skillset) |
| **Metaschema** | The syntax rules for defining schemas (e.g., "All specs must be valid CUE or JSON Schema"). | **Data Plane** (Schema) |
| **Registry** | The trusted repository of immutable artifacts (The "Periodic Table" of elements). | **Data Plane** (Substance) |

### Phenomenon 3: Protocol Legislation
**The setting of immutable laws for interaction.**

| Term | Definition within Zone 0 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Contract** | Standardized interface definitions (e.g., "Standard Health Check", "OpenAPI Spec"). | **Interaction Plane** (API) |
| **Governance** | Global policies applied to all entities (e.g., "Data Retention Laws", "Audit Requirements"). | **Control Plane** (Lifecycle) |
| **Invariant** | Rules that cannot be broken (e.g., "No Entity exists without a Creator ID"). | **Control Plane** (Policy) |

### Phenomenon 4: Dimensional Bifurcation (Forking)
**The physics of duplication and lineage.**

| Term | Definition within Zone 0 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Lineage ID** | The cryptographic trace of origin. Defines the genealogical tree of the world. | **Cognitive Plane** (Identity) |
| **Mutation Vector** | The specific variables allowed to change during a fork (e.g., "Keep Code, Reset Data"). | **Data Plane** (Properties) |
| **Inheritance Mode** | The copy mechanic: "Deep Copy" (Independent) vs. "Cow" (Copy-on-Write / Linked). | **Control Plane** (Mechanics) |

### Phenomenon 5: Quantum Entanglement (Sync)
**The physics of connection between Origin and Twin.**

| Term | Definition within Zone 0 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Resonance Link** | The channel connecting a `Source Entity` to its `Twin Entity`. | **Interaction Plane** (Boundary) |
| **Drift Metric** | The quantification of difference between worlds (e.g., "Schema Drift", "Data Lag"). | **Control Plane** (Orchestration) |
| **Reconciliation Logic** | The laws of resolving conflict between worlds (e.g., "Origin Wins", "Merge", "Reject"). | **Control Plane** (Policy) |

### Phenomenon 6: Resource Calibration (Economics)
**The definition of mass and energy.**

| Term | Definition within Zone 0 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Unit** | The atomic measure of consumption (e.g., "vCPU-Hour", "Storage-GB"). | **Data Plane** (Schema) |
| **Tier (QoS)** | Service level definitions (e.g., "Critical", "Best-Effort"). | **Control Plane** (Orchestration) |
| **Quota** | The meta-definition of limits and scarcity. | **Control Plane** (Policy) |

### Phenomenon 7: Causality Synchronization (Time)
**The definition of the flow of time.**

| Term | Definition within Zone 0 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Epoch** | The universal reference point for time. | **Control Plane** (Lifecycle) |
| **Consistency Model** | The rules of data propagation (e.g., "Strong" vs "Eventual"). | **Data Plane** (Potential) |
| **Version Strategy** | The logic of mutation naming (e.g., SemVer, Hashing). | **Control Plane** (Mechanics) |

### Phenomenon 8: Signal Standardization (Senses)
**The definition of how the system perceives itself.**

| Term | Definition within Zone 0 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Telemetry Schema** | The standard format for logs, metrics, and traces. | **Interaction Plane** (Boundary) |
| **Severity** | The taxonomy of urgency (e.g., "P0", "P1", "Info"). | **Cognitive Plane** (Meaning) |
| **Correlation** | The logic for linking events across boundaries (Trace IDs). | **Control Plane** (Orchestration) |
---

## Zone 1: Declaration (The Architect's Studio)

**Objective:** Design, Specification, and Intent.

**Context:** The Laws of Zone 0 are applied here to create a specific Project/Entity. This is the realm of the "Manifest" and the "Code Repository."

### Phenomenon 1: Archetypal Inheritance
*The act of selecting a form.*

| Term | Definition within Zone 1 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Class Extension** | The declaration of the parent type (e.g., `kind: Service`). | **Cognitive Plane** (Identity) |
| **Trait Adoption** | The selection of optional behaviors (e.g., `mixins: [auth]`). | **Data Plane** (Skillset) |
| **Metadata Tagging** | Labels for organization (e.g., `owner: team-a`). | **Cognitive Plane** (Meaning) |

### Phenomenon 2: Logic Composition
*The encoding of intrinsic behavior (The DNA).*

| Term | Definition within Zone 1 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Source Binding** | Pointer to logic repo (e.g., `git_repo: xyz`). | **Fabrication Dimension** (Spec) |
| **Schema Declaration** | Definition of internal structure (e.g., SQL DDL). | **Data Plane** (Schema) |
| **Immutable Artifact** | Frozen build object (e.g., Docker Image Digest). | **Data Plane** (Substance) |

### Phenomenon 3: Lineage Assertion (Twin World)
*The declaration of origin and relation.*

| Term | Definition within Zone 1 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Origin Reference** | Pointer to source entity (e.g., `fork_from: prod`). | **Cognitive Plane** (Identity) |
| **Drift Policy** | Tolerance for divergence. | **Control Plane** (Mechanics) |
| **Snapshot ID** | The specific Epoch of the Twin's creation. | **Temporal Factor** (State) |

### Phenomenon 4: Interface Projection
*The promise of contact.*

| Term | Definition within Zone 1 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Port Exposure** | Declaration of listening channels. | **Interaction Plane** (API) |
| **Contract Publication** | Attachment of API Spec (Swagger). | **Interaction Plane** (Access Protocol) |
| **Visibility Scope** | Who can see this interface. | **Scoping Factor** (Exposure) |

### Phenomenon 5: Dependency Binding
*The network of needs.*

| Term | Definition within Zone 1 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Service Link** | Requirement for other workers. | **Interaction Plane** (Boundary) |
| **Volume Claim** | Requirement for passive data. | **Data Plane** (Potentials) |
| **Secret Reference** | Pointer to secured config. | **Control Plane** (Orchestration) |

### Phenomenon 6: Contextual Parameterization
*The environmental fit.*

| Term | Definition within Zone 1 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Config Map** | Non-sensitive variables (e.g., `ENV=DEV`). | **Fabrication Dimension** (Config) |
| **Feature Flag** | Toggles for code paths. | **Control Plane** (Mechanics) |
| **Override Layer** | Modifications for Twin status. | **Temporal Factor** (State) |

### Phenomenon 7: Resource Reservation
*The economic request.*

| Term | Definition within Zone 1 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Request Spec** | Minimum resources to start. | **Data Plane** (Skillset) |
| **Limit Spec** | Maximum allowed consumption. | **Control Plane** (Policy) |
| **Affinity Rule** | Physical placement preference. | **Control Plane** (Orchestration) |

### Phenomenon 8: Integrity Certification
*The seal of validity.*

| Term | Definition within Zone 1 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Schema Validation** | Check against Zone 0 Metaschema. | **Control Plane** (Policy) |
| **Policy Check** | Governance verification. | **Control Plane** (Lifecycle) |
| **Signature Verify** | Proof of authorship. | **Cognitive Plane** (Identity) |

### Phenomenon 9: Semiotic Embedding (Agent Readiness)
*The encoding of meaning for AI consumption.*

| Term | Definition within Zone 1 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Tool Definition** | JSON Schema for LLM function calling. | **Interaction Plane** (API) |
| **System Prompt Injection** | Natural language instructions for the Agent. | **Cognitive Plane** (Meaning) |
| **Vector Signature** | Semantic keywords for Agent discovery. | **Data Plane** (Properties) |

---

## Zone 2: Fabrication (The Factory Floor)

**Objective:** Materialization, Hydration, and Instantiation.

**Context:** Zone 2 transforms the *potential* of Zone 1 into the *kinetic energy* of a running process. It manages the physical resources and the "birth" of the entity.

### Phenomenon 1: Artifact Hydration
*The assembly of substance and context.*

| Term | Definition within Zone 2 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Container Assembly** | Merging Image Layers with Env Vars. | **Fabrication Dimension** (Instance) |
| **Volume Mounting** | Attaching physical storage. | **Data Plane** (Properties) |
| **Secret Decryption** | Transforming references to values. | **Control Plane** (Mechanics) |

### Phenomenon 2: Ephemeral Identity Minting
*The assignment of temporary, runtime names.*

| Term | Definition within Zone 2 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Instance UUID** | Unique ID for this specific run. | **Cognitive Plane** (Identity) |
| **Certificate Issuance** | Creating mTLS proofs for this instance. | **Interaction Plane** (Protocol) |
| **DNS Registration** | Updating the service discovery phonebook. | **Interaction Plane** (Boundary) |

### Phenomenon 3: Economic Encumbrance
*The locking and deduction of resources.*

| Term | Definition within Zone 2 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Bin Packing** | Scheduling logic (Node placement). | **Control Plane** (Orchestration) |
| **Quota Deduction** | Subtraction from tenant allowance. | **Control Plane** (Policy) |
| **Lease Creation** | Time-bound right to exist. | **Temporal Factor** (Lifecycle) |

### Phenomenon 4: Dimensional Divergence
*The physics of forking for Twin entities.*

| Term | Definition within Zone 2 | Corresponding Axiom |
| :--- | :--- | :--- |
| **State Forking (COW)** | Copy-on-Write storage layer creation. | **Data Plane** (Potential) |
| **Traffic Shadowing** | Mirroring real traffic to the Twin. | **Control Plane** (Mechanics) |
| **Mutation Application** | Applying specific Twin overrides. | **Fabrication Dimension** (Config) |

### Phenomenon 5: Resonance Activation
*Establishing the link to the Origin.*

| Term | Definition within Zone 2 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Sync Subscription** | Listening for Origin updates. | **Interaction Plane** (Boundary) |
| **Diff Calculator** | Runtime measurement of drift. | **Control Plane** (Policy) |
| **Origin Proxying** | Fallback to Origin for missing data. | **Data Plane** (Skillset) |

### Phenomenon 6: Semiotic Indexing (Agent Onboarding)
*Ingesting the documentation into the Agent brain.*

| Term | Definition within Zone 2 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Vector Embedding** | Converting docs to vector coordinates. | **Cognitive Plane** (Meaning) |
| **RAG Ingestion** | Storing knowledge in Agent memory. | **Data Plane** (Schema) |
| **Tool Registration** | Registering capabilities with the Orchestrator. | **Interaction Plane** (API) |

### Phenomenon 7: Membrane Construction
*Establishing boundaries and filters.*

| Term | Definition within Zone 2 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Sidecar Injection** | Attaching service mesh proxies. | **Interaction Plane** (Boundary) |
| **Policy Enforcement** | Applying firewall/network rules. | **Control Plane** (Policy) |
| **Egress Filtering** | Limiting outbound access. | **Scoping Factor** (Exposure) |

### Phenomenon 8: The Ignition Event
*The start of time and telemetry.*

| Term | Definition within Zone 2 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Health Probing** | Liveness/Readiness checks. | **Temporal Factor** (State) |
| **Boot Sequence** | Execution of entrypoint command. | **Control Plane** (Mechanics) |
| **Telemetry Hook** | First emission of logs/metrics. | **Interaction Plane** (Visibility) |
---
## Zone 3: Operation (The Bridge)

**Objective:** Execution, Adaptation, and Service.

**Context:** Zone 3 is where the entity lives, breathes, and works. It is the domain of runtime dynamics, where the "Plan" meets "Reality."

### Phenomenon 1: Metabolic Homeostasis
*The struggle to stay alive and self-correct.*

| Term | Definition within Zone 3 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Heartbeat** | Signal of liveness to the control plane. | **Temporal Factor** (State) |
| **Reconciliation Loop** | Restarts processes and fixes drift. | **Control Plane** (Mechanics) |
| **Circuit Breaking** | Stops damage propagation to dependencies. | **Interaction Plane** (Boundary) |

### Phenomenon 2: Elastic Morphology
*Changing shape (scaling) under pressure.*

| Term | Definition within Zone 3 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Replica Expansion** | Horizontal scaling (Spawning clones). | **Fabrication Dimension** (Instance) |
| **Throttling** | Refusing work to survive. | **Control Plane** (Policy) |
| **Load Shedding** | Dropping low-priority tasks. | **Cognitive Plane** (Role) |

### Phenomenon 3: Resource Combustion
*The active consumption of economic value.*

| Term | Definition within Zone 3 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Metering Pulse** | Periodic recording of usage. | **Data Plane** (Substance) |
| **Saturation Point** | Measure of resource fullness (%). | **Control Plane** (Orchestration) |
| **Budget Alarm** | Trigger when cost exceeds limits. | **Control Plane** (Policy) |

### Phenomenon 4: Kinetic Transduction
*Transforming requests into work.*

| Term | Definition within Zone 3 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Ingress Event** | Arrival of a request. | **Interaction Plane** (Boundary) |
| **Latency Span** | Duration of processing. | **Temporal Factor** (Flow) |
| **Payload Processing** | Execution of business logic. | **Data Plane** (Skillset) |

### Phenomenon 5: State Transmutation
*The evolution of internal truth.*

| Term | Definition within Zone 3 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Transaction Commit** | Locking new truth to storage. | **Data Plane** (Substance) |
| **Cache Invalidation** | Purging obsolete data. | **Temporal Factor** (State) |
| **Event Emission** | Broadcasting state changes. | **Interaction Plane** (API) |

### Phenomenon 6: Signal Emission (Observability)
*The narrative of the self.*

| Term | Definition within Zone 3 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Log Stream** | Narrative diary of events. | **Cognitive Plane** (Meaning) |
| **Metric Aggregation** | Numerical summary of health. | **Data Plane** (Properties) |
| **Trace Propagation** | Context linking across boundaries. | **Interaction Plane** (Boundary) |

### Phenomenon 7: Quantum Resonance Maintenance
*The active flow between Twin and Origin.*

| Term | Definition within Zone 3 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Replay Stream** | Applying Origin events to Twin. | **Interaction Plane** (Protocol) |
| **Drift Correction** | Overwriting Twin state to match Origin. | **Control Plane** (Mechanics) |
| **Conflict Detection** | Spotting divergent writes. | **Control Plane** (Policy) |

### Phenomenon 8: Semiotic Engagement (Agent Usage)
*The active use by AI Agents.*

| Term | Definition within Zone 3 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Tool Invocation** | Agent executing a command. | **Interaction Plane** (API) |
| **Context Injection** | Feeding runtime state to the Agent. | **Cognitive Plane** (Meaning) |
| **Reasoning Feedback** | Output returning to the Agent's brain. | **Cognitive Plane** (Role) |
---

## Zone 4: Evolution (The Wisdom Refinery)

**Objective:** Synthesis, Sedimentation, and Selection.

**Context:** Zone 4 processes the raw experience of Zone 3 into permanent *Knowledge*. It maintains the "Multi-Fact Documentation," ensuring that the system learns from every success and failure. It turns *Data* into *Wisdom*.

---
### Phenomenon 1: Reality Calibration (The Truth Delta)
*Quantifying the gap between Zone 1 promises and Zone 3 behavior.*

| Term | Definition within Zone 4 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Divergence Vector** | The calculated distance between Spec and Reality (e.g., "Latency +300%"). | **Data Plane** (Properties) |
| **Specimen Categorization** | Re-labeling the entity based on actual behavior (e.g., "Batch" vs "Real-time"). | **Cognitive Plane** (Identity) |
| **Expectation Erosion** | Reducing confidence in the Spec if Reality contradicts it constantly. | **Control Plane** (Policy) |

### Phenomenon 2: Causal Attribution
*Identifying the physics behind the variance.*

| Term | Definition within Zone 4 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Factor Isolation** | Pinpointing the single variable responsible for a change. | **Data Plane** (Schema) |
| **Dependency Mapping** | Tracing internal failures to external neighbor changes. | **Interaction Plane** (Boundary) |
| **Exogenous Impact** | Attributing events to forces outside the system (e.g., Cloud Outage). | **Scoping Factor** (Exposure) |

### Phenomenon 3: Economic Crystallization
*Turning raw expense data into unit economics wisdom.*

| Term | Definition within Zone 4 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Efficiency Ratio** | Derived constant of "Resource per Outcome." | **Data Plane** (Skillset) |
| **Waste Pattern** | Identifying structural inefficiencies in logic loops. | **Control Plane** (Mechanics) |
| **Yield Calculation** | The final ROI score of the entity. | **Cognitive Plane** (Meaning) |

### Phenomenon 4: Epistemic Sedimentation (Truth Patching)
*Overlaying "Runtime Reality" onto "Design Spec."*

| Term | Definition within Zone 4 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Truth Patch** | Append-only override of Zone 1 Spec fields (e.g., "Note: Timeout is actually 8s"). | **Data Plane** (Properties) |
| **Heuristic Injection** | Creating "Rules of Thumb" for future Agents based on past patterns. | **Cognitive Plane** (Meaning) |
| **Divergence Warning** | Marking "Minefields" in the documentation where Spec is unreliable. | **Interaction Plane** (Boundary) |

### Phenomenon 5: Semiotic Refinement (Prompt Evolution)
*Optimizing the language used to control the entity.*

| Term | Definition within Zone 4 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Ambiguity Detection** | Finding Spec descriptions that caused Agent hallucinations. | **Cognitive Plane** (Identity) |
| **Instruction Hardening** | Converting "Suggestions" into "Constraints" in System Prompts. | **Control Plane** (Policy) |
| **Vocabulary Expansion** | Adding synonyms to vector indexes to improve tool discovery. | **Data Plane** (Schema) |

### Phenomenon 6: Teleological Selection (Survival of the Fittest)
*Deciding if a Twin should replace the Origin.*

| Term | Definition within Zone 4 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Fitness Score** | Composite metric: Is the Twin "Better" than Origin? | **Cognitive Plane** (Role) |
| **Promotion Decree** | Atomic command to swap Twin into Origin slot. | **Control Plane** (Lifecycle) |
| **Regression Block** | Blocking promotion due to violation of new Truths. | **Control Plane** (Mechanics) |

### Phenomenon 7: Entropic Recycling (Clean Death)
*Ensuring lessons survive the death of the entity.*

| Term | Definition within Zone 4 | Corresponding Axiom |
| :--- | :--- | :--- |
| **Wisdom Extraction** | Saving "Patches" to the Zone 0 Library before deletion. | **Data Plane** (Substance) |
| **State Fossilization** | Archiving final state for future forensics. | **Temporal Factor** (State) |
| **Tombstone Marker** | Permanent record of *why* the entity died. | **Cognitive Plane** (Identity) |
