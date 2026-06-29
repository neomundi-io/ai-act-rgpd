🌐 **Languages:** [Français](README.md) · [English](README_EN.md)

---

# NeoMundi ControlTower

## Runtime Evidence, Continuous Monitoring and Traceability for AI Governance

NeoMundi ControlTower is a diagnostic, continuous-monitoring and traceability layer for AI-generated responses.

It helps organisations observe behavioural signals during operation, detect measurable drift or regime changes, document risk indicators, apply configurable governance mechanisms and maintain technical evidence of the controls that were available and used.

ControlTower is designed privacy-first. It can be integrated through a simple API call, without requiring a change to the underlying AI infrastructure, and may be deployed in sovereign environments depending on the selected deployment model.

This document explains:

1. what ControlTower technically covers today;
2. how those capabilities may support an organisation’s EU AI Act and GDPR compliance process;
3. what remains outside NeoMundi’s scope and under the responsibility of each organisation.

> **Important:** NeoMundi does not determine whether an AI system is legally compliant.
> It provides a runtime evidence layer that helps organisations observe behavioural drift, document risk signals, trigger appropriate human review and demonstrate that operational controls existed when they were needed.

---

# 1. What ControlTower actually covers

## 1.1. Operational traceability of observed AI responses

ControlTower associates observed AI-response events with technical and operational artefacts that may include:

* an observation identifier;
* calculated metrics;
* measured risk signals;
* a configurable governance or control status;
* observation timestamps;
* configurable measurement history;
* traceability artefacts adapted to the selected deployment mode;
* justification elements associated with configured rules or actions.

These artefacts make it possible to connect an observed response pattern with the technical signals and control context available at the time of observation.

### Covered capability

**Technical and operational traceability of observed AI-response behaviour and associated risk signals.**

---

## 1.2. Continuous monitoring of AI-response behaviour

ControlTower continuously observes signals associated with the behaviour of AI systems during operation.

Depending on the enabled modules and selected configuration, these signals may include:

* stability;
* coherence;
* semantic variation;
* behavioural drift;
* hallucination-risk indicators;
* factual-risk indicators;
* factual-validity-related signals where the relevant module is enabled;
* latency, execution or operational indicators;
* configurable risk signals associated with generated responses.

The objective is not to claim that every signal establishes truth or error on its own.

The objective is to make observable when a system’s measured behaviour changes, becomes fragile, exceeds a defined threshold or requires additional review.

### Covered capability

**Continuous monitoring of AI-response behaviour, variation and measurable operational risk signals.**

---

## 1.3. Detection of behavioural drift and silent regime changes

ControlTower can help identify measurable changes in an AI system’s behaviour across time.

A behavioural change may appear even when:

* no public provider update has been announced;
* no visible production incident has yet been reported;
* a one-off benchmark remains broadly reassuring;
* conventional quality snapshots do not reveal the change.

Such observations may include changes in factual-risk signals, semantic variation, stability patterns or other monitored indicators.

ControlTower does not attribute the cause of a detected behavioural change unless an independent investigation establishes it.

A detected signal is an operational observation. It is not, by itself, proof of a provider change, a system defect, a legal breach or a root cause.

### Covered capability

**Detection and traceability of measurable behavioural drift and silent regime changes during operation.**

---

## 1.4. Configurable governance and control mechanisms

ControlTower can support configurable governance mechanisms that are applied in real time or near real time, depending on the selected integration.

These mechanisms may include:

* risk thresholds;
* alerts;
* escalation paths;
* routing to human review;
* differentiated treatment of higher-risk responses;
* configurable blocking or hold mechanisms where supported by the chosen integration;
* observation and decision logs;
* audit of rule application and measurement history.

ControlTower does not silently transform an observed signal into an authorised action.

A measurement signal may support awareness, review or escalation, but the authority to act remains defined by the organisation’s governance rules, responsible roles and selected integration.

### Covered capability

**Continuous monitoring and configurable control mechanisms for AI-response risk.**

---

## 1.5. Human-oversight support

ControlTower can support human oversight by making relevant runtime signals visible and actionable.

Depending on configuration, the platform may help organisations:

* define thresholds requiring review;
* notify responsible teams;
* escalate higher-risk observations;
* route events to a designated reviewer;
* preserve evidence of the observation and the control context;
* distinguish between an observed signal and an authorised downstream decision.

The platform provides technical support for human oversight. It does not replace human judgment, organisational accountability or legal responsibility.

### Covered capability

**Technical support for risk-based human oversight, review and escalation.**

---

## 1.6. Auditability and runtime evidence

ControlTower produces measurable and reviewable technical elements that may include:

* metrics;
* scores;
* risk signals;
* observation identifiers;
* configurable history;
* measurement artefacts;
* rule-application artefacts;
* justification elements;
* technical evidence associated with observed events.

These elements may be used to support internal audit, incident analysis, operational review, governance reporting or third-party assurance processes.

### Covered capability

**Auditability of observed AI-response behaviour, measured signals and configured control mechanisms.**

---

## 1.7. Evidence-based operational governance

ControlTower does not rely solely on a declarative claim that an AI system is reliable.

It provides measured, traceable and configurable signals that can help organisations make their governance processes more explicit.

For example, an organisation may use ControlTower to document that:

* an observation was detected;
* a risk signal crossed a configured threshold;
* a responsible role was notified;
* a human review was requested;
* a defined control mechanism was available or applied;
* the final downstream decision remained subject to organisational authority.

### Covered capability

**Operational governance supported by measured and traceable runtime evidence.**

---

# 2. Privacy-first architecture

ControlTower is designed around privacy-first principles.

Depending on the selected deployment mode and configuration, the architecture is designed to minimise content exposure and limit data processing to what is necessary for measurement, monitoring and configured governance mechanisms.

Core principles include:

* zero content retention;
* zero content logging;
* zero content storage;
* data minimisation;
* configurable traceability;
* deployment flexibility, including sovereign deployment models where available.

Prompt and response content is not retained, indexed, reused or stored by NeoMundi.

Minimal technical measurement and traceability artefacts may remain available according to the selected mode, configuration and deployment model.

---

## 2.1. OBS mode

In OBS mode, NeoMundi receives only the technical elements necessary for observation.

This may include:

* normalised metrics;
* technical observation artefacts;
* identifiers or pseudonymous references required for configured traceability;
* aggregated or non-content operational signals.

NeoMundi does not receive:

* raw prompts;
* raw responses;
* stored semantic content from exchanges;
* customer content for reuse or indexing.

### Covered capability

**Risk observation and technical traceability without transmission or retention of prompt and response content.**

---

## 2.2. GOV mode

In GOV mode, data may transit in real time solely for measurement and configured governance-rule enforcement purposes.

Content is:

* not retained;
* not indexed;
* not reused;
* not stored.

The precise behaviour of GOV mode depends on the selected integration, deployment model and organisational configuration.

### Covered capability

**Real-time measurement and configurable governance mechanisms without content retention.**

---

## 2.3. Sovereign deployment options

ControlTower may be deployed according to a sovereign or controlled infrastructure model, depending on the selected deployment architecture.

This can support organisations that require:

* controlled hosting environments;
* data-location constraints;
* infrastructure sovereignty;
* integration with trusted cloud or on-premise environments;
* reduced exposure of operational AI data.

### Covered capability

**Deployment flexibility for organisations with sovereignty, security or infrastructure-control requirements.**

---

# 3. How ControlTower may support an EU AI Act compliance process

ControlTower does not replace legal analysis, conformity assessment, organisational governance or regulatory certification.

However, it provides technical capabilities and runtime evidence that may support several operational areas relevant to an EU AI Act compliance process.

The applicability of those areas depends on the AI system concerned, its intended purpose, the organisation’s role, the risk classification of the system and the specific use case.

| Operational area                              | ControlTower contribution                                                                         | Coverage status                                        |
| --------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------ |
| Monitoring during operation                   | Continuous observation of AI-response behaviour, variation and configured risk signals            | Technically supported                                  |
| Risk-management support                       | Measured scores, risk signals, thresholds, alerts and escalation mechanisms                       | Technically supported                                  |
| Operational traceability                      | Observation identifiers, metrics, timestamps and configurable measurement artefacts               | Technically supported                                  |
| Logging support                               | Configurable technical history and traceability artefacts without content retention               | Supported depending on configuration                   |
| Human-oversight support                       | Alerts, escalation paths, routing to human review and visibility of measured signals              | Technical capability provided                          |
| Treatment of higher-risk responses            | Differentiated handling, review, hold or blocking mechanisms depending on integration             | Technical capability provided depending on integration |
| Auditability                                  | Measured signals, technical artefacts and justification elements                                  | Technically supported                                  |
| Incident analysis and documentation           | Runtime evidence that may support analysis, investigation and documentation of operational events | Direct operational contribution                        |
| Post-deployment monitoring                    | Longitudinal observation of system behaviour, drift and measurable regime changes                 | Direct operational contribution                        |
| Transparency of operational controls          | Visibility into observed signals, configured thresholds and applied control context               | Direct operational contribution                        |
| Complete legal classification of an AI system | Depends on intended purpose, use case, organisational role and legal assessment                   | Out of scope                                           |
| Formal conformity assessment                  | Requires the applicable legal, organisational and technical assessment process                    | Out of scope                                           |
| Regulatory certification                      | Requires the relevant legal and certification process                                             | Out of scope                                           |

---

## 3.1. Runtime evidence for post-deployment monitoring

A central contribution of ControlTower is the ability to create a longitudinal record of observed AI-system behaviour during operation.

This may help organisations identify:

* unexpected variation;
* increased factual-risk signals;
* changes in semantic behaviour;
* degradation of observed stability;
* changes in risk distribution;
* silent regime changes;
* patterns that merit review before they become visible through traditional incident reporting.

ControlTower does not replace incident investigation.

It helps establish that an operational signal was observed, measured and documented at a given time, under a defined measurement and governance context.

---

## 3.2. The distinction between measurement and authorisation

ControlTower is designed around an important governance distinction:

> **A runtime measurement signal is not, by itself, an authorisation to act.**

A measured signal may justify:

* internal awareness;
* further investigation;
* human review;
* a recommendation;
* escalation;
* a configured safety response.

Whether it may justify a downstream action depends on the organisation’s own governance model, responsible authority, use case and applicable controls.

This distinction helps prevent an observed technical signal from being silently treated as a final decision.

---

# 4. How ControlTower may support a GDPR compliance process

ControlTower is designed to support privacy-first processing principles.

It does not replace a complete GDPR assessment, a record of processing activities, a Data Protection Impact Assessment or the legal responsibility of the controller or processor.

However, the architecture may provide technical support for several GDPR-related operational principles.

| GDPR-related area                 | ControlTower contribution                                                                  | Coverage status                 |
| --------------------------------- | ------------------------------------------------------------------------------------------ | ------------------------------- |
| Data minimisation                 | Data transmission limited to what is necessary for the selected mode and technical purpose | Supported by architecture       |
| Data protection by design         | OBS and GOV modes designed to minimise content exposure and avoid content retention        | Supported by architecture       |
| Storage limitation                | No retention, logging or storage of prompt and response content by NeoMundi                | Supported by architecture       |
| Accountability support            | Technical artefacts that may help document implemented monitoring and control mechanisms   | Direct operational contribution |
| Control traceability              | Signals, metrics, identifiers and configurable technical history                           | Technically supported           |
| Processing documentation support  | Technical elements that may contribute to organisational documentation                     | Partial contribution            |
| Record of processing activities   | Organisational and legal document maintained by the relevant controller or processor       | Out of scope                    |
| Data Protection Impact Assessment | Legal and organisational assessment performed where required                               | Out of scope                    |
| Legal basis determination         | Depends on the organisation’s processing context and legal assessment                      | Out of scope                    |
| Data-subject rights management    | Requires organisational procedures and systems beyond ControlTower                         | Out of scope                    |

---

# 5. What ControlTower does not cover

NeoMundi does not replace an organisation’s legal, organisational, security or governance responsibilities.

ControlTower does not provide:

* complete legal classification of an AI system under the EU AI Act;
* legal advice;
* legal analysis of a specific use case;
* automatic confirmation of regulatory compliance;
* preparation of an organisation’s GDPR record of processing activities;
* completion of a Data Protection Impact Assessment;
* an organisation’s internal AI policy;
* HR governance;
* contractual compliance management;
* complete supplier qualification;
* Shadow AI mapping;
* a global cybersecurity audit;
* formal conformity assessment;
* regulatory certification;
* root-cause attribution for an observed behavioural change;
* proof that a single response is true, false, safe or compliant solely from one measurement signal;
* replacement of human judgment or accountable organisational authority.

---

# 6. Summary positioning

**NeoMundi ControlTower is a runtime evidence, continuous-monitoring and traceability layer for AI-generated responses.**

It helps organisations:

* observe AI-response behaviour during operation;
* detect measurable drift and silent regime changes;
* document risk signals and technical context;
* support human oversight and escalation;
* apply configurable control mechanisms;
* maintain auditable operational evidence;
* reduce content exposure through privacy-first architecture;
* support, but not replace, AI Act and GDPR compliance processes.

NeoMundi does not claim to determine whether an AI system is legally compliant.

It provides the operational evidence layer that helps organisations understand what their AI systems were doing in production, what signals were observed, what controls were available and what governance response was triggered.

---

# 7. Integration

ControlTower can be integrated:

* through a simple API call;
* without requiring a change to the underlying AI infrastructure;
* in OBS mode;
* in GOV mode;
* through sovereign deployment models depending on the selected architecture;
* with configurable monitoring, thresholds, alerts and traceability settings.

The available capabilities depend on the selected deployment model, integration depth and organisational configuration.

---

# 8. Disclaimer

This document describes the technical capabilities and intended operational contribution of NeoMundi ControlTower.

It does not constitute:

* legal advice;
* regulatory certification;
* a formal conformity assessment;
* an automatic guarantee of compliance;
* a complete assessment applicable to a specific organisation or AI use case.

Compliance depends on multiple factors, including:

* the AI system concerned;
* its intended purpose;
* its risk classification;
* the context of use;
* the organisation’s role;
* the applicable legal framework;
* the technical and organisational measures implemented;
* the governance and human-oversight processes maintained by the organisation.
