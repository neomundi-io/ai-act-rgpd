# NeoMundi ControlTower

## Control, Traceability and Contribution to EU AI Act and GDPR Compliance Efforts

NeoMundi has developed **ControlTower**, a diagnostic, continuous-control and traceability layer designed to manage the risk of AI-generated responses.

Privacy-first by design, ControlTower integrates through a simple API call, without requiring infrastructure changes. The platform can also be deployed in sovereign mode.

This document clearly presents:

1. what ControlTower technically covers today;
2. what the platform helps demonstrate as part of an EU AI Act or GDPR compliance process;
3. what remains the responsibility of each organisation.

---

# 1. What ControlTower actually covers

## 1.1. Operational traceability of AI responses

ControlTower associates observed responses with:

* an observation identifier;
* calculated metrics;
* a governance score;
* actionable risk signals;
* configurable measurement history;
* traceability artefacts adapted to the selected deployment mode.

### Covered capability

**Technical and operational traceability of observed AI responses.**

---

## 1.2. Continuous risk monitoring

ControlTower continuously observes different signals related to the behaviour of AI systems:

* stability;
* coherence;
* drift;
* hallucination risk;
* factual validity when the relevant module is enabled;
* risk signals associated with generated responses.

### Covered capability

**Continuous monitoring of AI-response behaviour and risk.**

---

## 1.3. Continuous control

ControlTower makes it possible to configure governance rules that can be applied in real time:

* risk thresholds;
* alerts;
* supervision;
* escalation to human review;
* blocking or specific handling of higher-risk responses, depending on the selected integration;
* audit of observations.

### Covered capability

**Continuous control of AI-response risk.**

---

## 1.4. Auditability

ControlTower produces measurable and verifiable elements:

* metrics;
* scores;
* signals;
* configurable history;
* justification elements;
* measurement and traceability artefacts.

### Covered capability

**Auditability of observed responses and associated risk signals.**

---

## 1.5. Evidence-based governance

ControlTower does not rely solely on a declarative promise of reliability.

The platform provides measured, traceable and actionable signals that can be used to document control decisions.

### Covered capability

**Operational governance based on evidence.**

---

# 2. A privacy-first architecture

ControlTower is designed around the following principles:

* **zero content retention**;
* **zero content logging**;
* **zero content storage**.

In other words, prompt and response content is neither retained, logged nor stored by NeoMundi.

Minimal measurement and traceability artefacts may remain available depending on the selected mode and configuration.

---

## 2.1. OBS mode

In OBS mode, NeoMundi receives only:

* normalised metrics;
* technical observation artefacts.

NeoMundi does not receive:

* prompts;
* responses;
* semantic content from exchanges.

### Covered capability

**Risk observation without content transmission.**

---

## 2.2. GOV mode

In GOV mode, data transits in real time solely for measurement and governance-rule enforcement purposes.

Content is:

* not retained;
* not indexed;
* not reused;
* not stored.

### Covered capability

**Real-time control without content retention.**

---

# 3. What ControlTower helps demonstrate in an EU AI Act compliance process

ControlTower does not replace a complete legal analysis and does not provide regulatory certification.

However, the platform provides technical capabilities and evidence that are directly useful for several operational requirements expected in an EU AI Act compliance process.

| Area                                            | ControlTower contribution                                           | Coverage level                                 |
| ----------------------------------------------- | ------------------------------------------------------------------- | ---------------------------------------------- |
| Monitoring during operation                     | Continuous monitoring of AI-response behaviour and risk             | Technically covered                            |
| Risk management                                 | Actionable scores, signals, thresholds and alerts                   | Technically covered                            |
| Operational traceability                        | Observation identifiers, metrics and measurement artefacts          | Technically covered                            |
| Risk-adapted logging                            | Configurable history without content retention                      | Technically covered depending on configuration |
| Human oversight                                 | Thresholds, alerts and escalation to human review                   | Technical capability provided                  |
| Control of higher-risk responses                | Blocking or specific handling depending on the selected integration | Technical capability provided                  |
| Auditability                                    | Measured signals and justification elements                         | Technically covered                            |
| Incident documentation                          | Evidence that can be used to analyse and document incidents         | Direct contribution                            |
| Post-deployment monitoring                      | Data supporting system monitoring during operation                  | Direct contribution                            |
| Complete EU AI Act classification of the system | Analysis depending on the use case and the organisation’s role      | Out of scope                                   |

---

# 4. What ControlTower helps demonstrate in a GDPR compliance process

ControlTower’s privacy-first architecture directly contributes to several GDPR principles.

| Principle                                | ControlTower contribution                                                         | Coverage level          |
| ---------------------------------------- | --------------------------------------------------------------------------------- | ----------------------- |
| Data minimisation                        | Transmission limited to what is strictly necessary depending on the selected mode | Covered by architecture |
| Data protection by design                | OBS and GOV modes designed to limit content exposure                              | Covered by architecture |
| Storage limitation                       | Zero content retention, zero content logging, zero content storage                | Covered by architecture |
| Accountability                           | Technical artefacts supporting demonstration of implemented controls              | Direct contribution     |
| Control traceability                     | Signals, scores and configurable history                                          | Technically covered     |
| Processing documentation                 | Technical elements that can be used by the organisation                           | Partial contribution    |
| Record of processing activities          | Organisational document maintained by the data controller                         | Out of scope            |
| Data Protection Impact Assessment — DPIA | Legal and organisational assessment performed by the client where required        | Out of scope            |

---

# 5. What NeoMundi does not cover

NeoMundi does not replace an organisation’s legal, organisational or security functions.

ControlTower does not cover:

* the complete legal classification of a system under the EU AI Act;
* legal analysis of the use case;
* preparation of the GDPR record of processing activities;
* completion of a DPIA;
* the organisation’s internal AI policy;
* HR governance;
* contractual compliance;
* complete supplier qualification;
* Shadow AI mapping;
* a global cybersecurity audit;
* regulatory certification;
* formal conformity assessment.

---

# 6. Summary positioning

**NeoMundi ControlTower is a diagnostic, continuous-control and traceability layer for AI-generated responses.**

By architecture, the platform provides monitoring, auditability, human-oversight capabilities, evidence-based governance and privacy-first data protection.

It directly contributes to several operational requirements expected in EU AI Act and GDPR compliance processes, notably in the areas of monitoring, risk management, traceability and demonstration of controls.

---

# 7. Integration

ControlTower can be integrated:

* through a simple API call;
* without infrastructure changes;
* in OBS mode;
* in GOV mode;
* in sovereign deployment mode depending on the selected deployment model.

---

# 8. Disclaimer

This document presents the technical capabilities of NeoMundi ControlTower.

It does not constitute:

* legal advice;
* regulatory certification;
* an automatic guarantee of compliance;
* a complete assessment applicable to a specific organisation or use case.

Compliance depends notably on the system concerned, its intended purpose, the context of use, the organisation’s role and the technical and organisational measures implemented.
