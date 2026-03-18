# User Stories



**User Stories** turn product requirements into clear, actionable backlog items that developers can build. They describe what users want to accomplish and why it matters.

Use this template to write stories that are specific, measurable, achievable, relevant, and time-bound. Include acceptance criteria in Given/When/Then format.

Link to PRDs and design files in the Additional Details section.

## Story Format

**As a** [role]

**I want** [goal]

**So that** [benefit]

## Acceptance Criteria

Use Given/When/Then (Gherkin) format:

- **Given** [context], **when** [action], **then** [expected outcome]
- **Given** [context], **when** [action], **then** [expected outcome]
- **Given** [context], **when** [action], **then** [expected outcome]

## SMART Checklist

**Specific** — Clear objective with no ambiguity

**Measurable** — Defined success criteria

**Achievable** — Sprint-sized and feasible for team capacity

**Relevant** — Aligned with product vision and objectives

**Time-bound** — Deliverable within one sprint

## Additional Details (Optional)

### Business Value

Why does this matter? How does it contribute to product or business objectives?

### Dependencies

- Technical dependencies (APIs, integrations, data sources)
- Cross-team dependencies
- Prerequisite work

### Edge Cases & Validation

- Error scenarios
- Boundary conditions
- Performance considerations
- Security requirements

### Notes

- Assumptions
- Open questions
- Risks or concerns

## Example

### Story

**As a** facility manager

**I want** to create TechOne requisitions directly from FMI work orders

**So that** I can streamline purchasing without manual data entry

### Acceptance Criteria

- **Given** a work order with status "under consideration", **when** I trigger the integration, **then** a TechOne requisition is created with all mandatory fields populated
- **Given** a supplier ABN is provided, **when** the requisition is created, **then** the supplier account is automatically looked up and linked
- **Given** the integration fails, **when** an error occurs, **then** the user receives a clear error message and the work order status remains unchanged

### Business Value

Reduces manual effort, minimizes data entry errors, and accelerates procurement cycle time for Royal Freemasons and future clients.

### Dependencies

- TechOne web service access and authentication
- Excel export of purchasing locations for mapping
- ABN lookup service availability
