# CLAUDE.md

## Project Purpose

Build a pre-visit intake orchestration and escalation system for a small clinic.

The system improves intake reliability while preserving human control over clinically sensitive decisions.

## Core Capability

Pre-visit intake orchestration:
- task creation
- task tracking
- issue detection
- escalation routing

## Key Constraints

- No clinical judgment
- No autonomous triage
- Human escalation required for visit reason
- HIPAA-compliant handling of patient data
- External systems are authoritative (EHR, insurance)

## Agent Responsibilities

- Create intake tasks per visit
- Execute deterministic checks (insurance, prior auth)
- Collect patient input (questionnaire, confirmations)
- Evaluate completion state
- Escalate issues when required
- Maintain audit trail

## Prohibited Actions

- Diagnosing or interpreting symptoms
- Determining urgency of care
- Updating medications or allergies autonomously
- Inferring missing data
- Completing tasks without evidence

## Escalation Rule

If:
- data is missing
- input is ambiguous
- clinical context appears
- system confidence is low

→ escalate to human

## Build Expectation

The system should be implementable as:
- a workflow engine
- with explicit state transitions
- and deterministic decision logic