# Problem Statement & Success Metrics

## Problem Statement

The clinic operates a high-volume intake workflow without a reliable mechanism to ensure all required administrative checks are completed before the visit.

As a result:
- intake defects are discovered during the visit
- physicians are interrupted by administrative issues
- staff must perform reactive rework

This creates operational inefficiency and workflow disruption.

## Context

- ~180 patients per day  
- 4 front-desk staff  
- ~45 patients per staff member  
- multiple intake steps per patient  

## Design Goal

Ensure intake completeness before the visit while reducing manual administrative effort.

## Success Metrics

### Reliability
- % of visits with complete intake before visit
- reduction in visit-time intake defects
- reduction in late discovery of prior auth issues

### Efficiency
- reduction in manual intake effort
- reduction in repeated administrative checks
- reduction in follow-up workload

### Safety and Control
- 0 clinical decisions made by the agent
- 100% escalation of sensitive inputs
- full audit coverage of all actions