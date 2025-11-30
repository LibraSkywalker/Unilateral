# Unilateral

Phase-Oriented World-Building Specification in Cuelang

---

## Zone 0: Meta

**Purpose:** Integration, platform entity discovery, twin worlds for different purposes.

### Specification

- **Platform Integration**
  - Define connection points between external systems and the world specification
  - Establish authentication and authorization boundaries
  - Configure environment-specific adapters (development, staging, production)

- **Entity Discovery**
  - Catalog available platform entities (services, resources, agents)
  - Map entity capabilities and constraints
  - Maintain entity lifecycle states and health indicators

- **Twin Worlds**
  - Support parallel world instances for different purposes (testing, simulation, production)
  - Enable world forking and merging strategies
  - Define synchronization rules between twin instances

---

## Zone 1: Declaration

**Purpose:** Project intent, requirements, architecture sketch.

### Specification

- **Project Intent**
  - Define the core objectives and success criteria
  - Establish scope boundaries and non-goals
  - Document stakeholder expectations and priorities

- **Requirements**
  - Specify functional requirements with acceptance criteria
  - Define non-functional requirements (performance, security, reliability)
  - Capture constraints and dependencies

- **Architecture Sketch**
  - Outline high-level system components and their relationships
  - Define data flow patterns and communication protocols
  - Establish architectural decision records (ADRs)

---

## Zone 2: Construction

**Purpose:** Turn scaffolds into artifact, add observability, wire agents.

### Specification

- **Scaffold to Artifact**
  - Transform declarative specifications into deployable artifacts
  - Generate configuration files, manifests, and infrastructure code
  - Validate artifact integrity and completeness

- **Observability**
  - Instrument artifacts with logging, metrics, and tracing
  - Define alerting rules and thresholds
  - Establish dashboards and visualization templates

- **Agent Wiring**
  - Connect autonomous agents to their designated roles
  - Configure agent communication channels and protocols
  - Define agent permissions and operational boundaries

---

## Zone 3: Execution

**Purpose:** Operate with real resources; model requests to metric.

### Specification

- **Resource Operation**
  - Deploy artifacts to target environments
  - Manage resource provisioning and deprovisioning
  - Handle scaling, failover, and recovery procedures

- **Request Modeling**
  - Capture incoming requests and their characteristics
  - Route requests through appropriate processing pipelines
  - Track request lifecycle from ingestion to completion

- **Metric Generation**
  - Convert operational events into measurable metrics
  - Aggregate and store metric data for analysis
  - Expose metrics through standardized interfaces

---

## Zone 4: Evaluation

**Purpose:** Analyze data, assess goals, feed the next cycle.

### Specification

- **Data Analysis**
  - Process collected metrics and logs for insights
  - Identify patterns, anomalies, and trends
  - Generate reports and summaries

- **Goal Assessment**
  - Compare actual outcomes against declared objectives
  - Calculate success metrics and key performance indicators
  - Identify gaps and areas for improvement

- **Cycle Feedback**
  - Synthesize learnings into actionable recommendations
  - Update declarations and requirements based on findings
  - Trigger the next iteration of the world-building cycle
