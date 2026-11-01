# NeoMundi ControlTower

[🇬🇧 English](./README.md) · [🇫🇷 Français](./README_FR.md) ·
[NeoMundi](https://neomundi.io) ·
[Create an account](https://controltower.neomundi.io/welcome)

## Runtime evidence, continuous monitoring and traceability for AI governance

NeoMundi ControlTower helps organizations observe the behavior of AI-generated responses in production, detect measurable drift and regime changes, document risk signals, apply configurable governance mechanisms and retain auditable technical evidence.

**One API integration · Continuous runtime signals · Configurable governance · Auditable evidence**

ControlTower is designed with a privacy-first approach. It can be integrated through a simple API call without replacing the underlying AI infrastructure and can support sovereign deployment models depending on the selected architecture.

### Start using ControlTower

1. **Create your account and API key**  
   [Open NeoMundi ControlTower →](https://controltower.neomundi.io/welcome)

2. **Connect your AI system**  
   Integrate through the NeoMundi API using the documentation and the deployment mode suited to your environment.

3. **Observe and govern**  
   Receive runtime measurements, configure monitoring and escalation rules, and retain traceable evidence of the controls available and applied.

This document explains:

1. what ControlTower technically covers today;
2. how these capabilities can contribute to an organization’s compliance processes under the European AI Act and the GDPR;
3. what remains outside NeoMundi’s scope and under each organization’s responsibility.

> **Important:** NeoMundi does not determine whether an AI system is legally compliant. It provides a runtime evidence layer that helps organizations observe behavioral drift, document risk signals, trigger appropriate human review and demonstrate that operational controls existed when required.

---

# 1. What ControlTower actually covers

## 1.1. Operational traceability of observed AI responses

ControlTower associates observed events related to AI responses with technical and operational artifacts that may include:

* an observation identifier;
* calculated metrics;
* measured risk signals;
* a configurable governance or control status;
* observation timestamps;
* configurable measurement history;
* traceability artifacts suited to the selected deployment mode;
* justification elements associated with configured rules or actions.

These artifacts make it possible to connect an observed behavior with the technical signals and control context available at the time of observation.

### Covered capability

**Technical and operational traceability of observed AI-response behavior and associated risk signals.**

---

## 1.2. Continuous monitoring of AI-response behavior

ControlTower continuously observes signals associated with the behavior of AI systems during operation.

Depending on the enabled modules and selected configuration, these signals may include:

* stability;
* coherence;
* semantic variation;
* behavioral drift;
* hallucination-risk indicators;
* factual-risk indicators;
* factual-validity signals when the relevant module is enabled;
* latency, execution or operational indicators;
* configurable risk signals associated with generated responses.

The objective is not to claim that a signal, by itself, establishes the truth or error of a response.

The objective is to make observable the moment when the measured behavior of a system changes, becomes fragile, crosses a defined threshold or requires additional review.

### Covered capability

**Continuous monitoring of AI-response behavior, variability and measurable operational risk signals.**

---

## 1.3. Detection of behavioral drift and silent regime changes

ControlTower can help identify measurable changes in the behavior of an AI system over time.

A behavioral change may appear even when:

* no public provider update has been announced;
* no visible production incident has yet been reported;
* a point-in-time benchmark remains broadly reassuring;
* conventional quality snapshots do not reveal the change.

These observations may concern changes in factual-risk signals, semantic variation, stability or other monitored indicators.

ControlTower does not attribute the cause of a detected behavioral change unless an independent investigation establishes it.

A detected signal is an operational observation. By itself, it is not proof of a provider change, system failure, legal breach or root cause.

### Covered capability

**Detection and traceability of measurable behavioral drift and silent regime changes in production.**

---

## 1.4. Configurable governance and control mechanisms

ControlTower can support configurable governance mechanisms applied in real time or near real time, depending on the selected integration.

These mechanisms may include:

* risk thresholds;
* alerts;
* escalation paths;
* routing to human review;
* differentiated treatment of higher-risk responses;
* configurable blocking or hold mechanisms where supported by the selected integration;
* observation and decision logs;
* auditing of rule application and measurement history.

ControlTower does not silently turn an observed signal into an authorized action.

A measurement signal may justify information, review or escalation, but the authority to act remains defined by the organization’s governance rules, accountable roles and selected integration.

### Covered capability

**Continuous monitoring and configurable mechanisms for controlling risks associated with AI responses.**

---

## 1.5. Support for human oversight

ControlTower can support human oversight by making relevant runtime signals visible and actionable.

Depending on the configuration, the platform can help organizations:

* define thresholds that require review;
* notify responsible teams;
* escalate observations presenting higher risk;
* route events to a designated reviewer;
* retain evidence of the observation and its control context;
* distinguish an observed signal from an authorized downstream decision.

The platform provides technical support for human oversight. It does not replace human judgment, organizational accountability or legal responsibility.

### Covered capability

**Technical support for risk-based human oversight, review and escalation.**

---

## 1.6. Auditability and runtime evidence

ControlTower produces measurable and verifiable technical elements that may include:

* metrics;
* scores;
* risk signals;
* observation identifiers;
* configurable history;
* measurement artifacts;
* rule-application artifacts;
* justification elements;
* technical evidence associated with observed events.

These elements can support an internal audit, incident analysis, operational review, governance reporting or third-party assurance activities.

### Covered capability

**Auditability of observed AI-response behavior, measured signals and configured control mechanisms.**

---

## 1.7. Evidence-based operational governance

ControlTower does not rely solely on declarative claims about the reliability of an AI system.

It provides measured, traceable and configurable signals that can help organizations make their governance processes more explicit.

For example, an organization can use ControlTower to document that:

* an observation was detected;
* a risk signal crossed a configured threshold;
* an accountable role was notified;
* a human review was requested;
* a defined control mechanism was available or applied;
* the final downstream decision remained under the organization’s authority.

### Covered capability

**Operational governance supported by measured and traceable runtime evidence.**

---

# 2. Data protection boundaries

ControlTower is designed to support data minimization, but NeoMundi has several distinct data flows. No organization-wide claim of zero transmission, zero storage or zero retention is made here.

The currently reviewed technical boundaries are:

* a REST measurement request may include prompt and response text when the caller supplies them;
* an SSE generation path sends generation arguments and the configured provider credential upstream;
* submitted text may be processed by enabled evaluators and services;
* Station documents an internal ledger containing answers and measurement context, while its read-only interface returns fingerprints and lengths instead of raw text;
* the interoperability export excludes raw prompts, responses and provider/model identifiers by schema design.

Transmission, processing, disclosure and retention are different questions. Retention and deletion guarantees must be established for each deployment, service, evaluator, log, backup and store. An export or read-only interface without raw text does not prove that raw text was never processed or stored upstream.

[**Review the canonical Data Protection & Confidentiality documentation →**](https://github.com/neomundi-io/neomundi-io-data-protection)

## 2.1. OBS paths

OBS is a measurement-layer label, not a guarantee that the payload is metrics-only. The reviewed REST path can receive llm_prompt and llm_response when supplied by the caller. Other integrations may submit reduced execution objects, but the measurements that remain available and their provenance depend on the actual payload and deployment.

## 2.2. GOV and generation paths

In GOV or generation paths, content and provider parameters may transit through NeoMundi and configured upstream services for measurement, generation or enabled controls. The exact destinations, evaluators, available governance mechanisms, storage and retention depend on the selected route, integration and deployment.

A measurement signal does not itself authorize an action. Blocking, holding, routing or human-review mechanisms exist only where the consuming integration explicitly implements and authorizes them.

## 2.3. Sovereign deployment options

Sovereign or controlled deployment models may be available depending on the selected architecture. Their data location, operators, subprocessors, access controls and retention rules must be documented for the actual deployment; they are not inferred from the deployment label.

# 3. How ControlTower can contribute to an EU AI Act compliance process

ControlTower does not replace legal analysis, conformity assessment, organizational governance or regulatory certification.

It nevertheless provides technical capabilities and runtime evidence that can contribute to several operational areas relevant to an EU AI Act compliance process.

The applicability of these areas depends on the AI system, its intended purpose, the organization’s role, the system’s risk classification and the specific use case.

| Operational area | ControlTower contribution | Coverage level |
|---|---|---|
| Monitoring during operation | Continuous observation of AI-response behavior, variability and configured risk signals | Technically supported |
| Risk-management support | Measured scores, risk signals, thresholds, alerts and escalation mechanisms | Technically supported |
| Operational traceability | Observation identifiers, metrics, timestamps and configurable measurement artifacts | Technically supported |
| Logging support | Configurable technical history and traceability artifacts; content retention depends on the deployment | Supported depending on configuration |
| Human-oversight support | Alerts, escalation paths, routing to human review and visibility of measured signals | Technical capability provided |
| Treatment of higher-risk responses | Differentiated treatment, review, hold or blocking depending on the integration | Technical capability provided depending on integration |
| Auditability | Measured signals, technical artifacts and justification elements | Technically supported |
| Incident analysis and documentation | Runtime evidence supporting the analysis, investigation and documentation of events | Direct operational contribution |
| Post-deployment monitoring | Longitudinal observation of behavior, drift and measurable regime changes | Direct operational contribution |
| Transparency of operational controls | Visibility into observed signals, configured thresholds and applied control context | Direct operational contribution |
| Complete legal classification of an AI system | Depends on intended purpose, use case, organizational role and legal analysis | Out of scope |
| Formal conformity assessment | Requires the applicable legal, organizational and technical process | Out of scope |
| Regulatory certification | Requires the appropriate certification and assessment process | Out of scope |

## 3.1. Runtime evidence for post-deployment monitoring

A central contribution of ControlTower is its ability to create a longitudinal history of the observed behavior of an AI system during operation.

This can help organizations identify:

* unexpected variation;
* an increase in factual-risk signals;
* changes in semantic behavior;
* degradation in observed stability;
* changes in the distribution of risk;
* silent regime changes;
* patterns requiring review before they become visible through traditional incident-reporting processes.

ControlTower does not replace an incident investigation.

It helps establish that an operational signal was observed, measured and documented at a given time within a defined measurement and governance context.

## 3.2. The distinction between measurement and authorization

ControlTower is built around an essential governance distinction:

> **A runtime measurement signal does not, by itself, constitute authorization to act.**

A measured signal may justify:

* internal information;
* further investigation;
* human review;
* a recommendation;
* an escalation;
* a configured safety response.

The ability to justify a downstream action depends on the organization’s governance model, accountable authority, use case and applicable controls.

This distinction prevents an observed technical signal from being silently treated as a final decision.

---

# 4. How ControlTower can contribute to a GDPR compliance process

ControlTower is designed to support privacy-first data-processing principles.

It does not replace a complete GDPR analysis, a record of processing activities, a data protection impact assessment, or the legal responsibility of a controller or processor.

Its architecture can nevertheless provide technical support for several GDPR-related operational principles.

| GDPR-related area | ControlTower contribution | Coverage level |
|---|---|---|
| Data minimization | Transmission limited to the data required by the selected mode and technical purpose | Supported by design |
| Data protection by design | Selected paths may minimize content exposure; actual processing and retention remain deployment-specific | Supported by design |
| Storage limitation | No universal guarantee established; rules must be verified per service, evaluator, log, backup and store | Supported by design |
| Accountability support | Technical artifacts that can help document implemented monitoring and control mechanisms | Direct operational contribution |
| Traceability of controls | Signals, metrics, identifiers and configurable technical history | Technically supported |
| Support for processing documentation | Technical elements that can contribute to organizational documentation | Partial contribution |
| Record of processing activities | Organizational and legal document maintained by the relevant controller or processor | Out of scope |
| Data protection impact assessment | Legal and organizational assessment performed when required | Out of scope |
| Determination of the legal basis | Depends on the processing context and the organization’s legal analysis | Out of scope |
| Management of data-subject rights | Requires organizational procedures and systems beyond ControlTower | Out of scope |

---

# 5. What ControlTower does not cover

NeoMundi does not replace an organization’s legal, organizational, security or governance responsibilities.

ControlTower does not provide:

* the complete legal classification of an AI system under the EU AI Act;
* legal advice;
* a legal analysis of a specific use case;
* automatic confirmation of regulatory compliance;
* preparation of an organization’s record of processing activities;
* performance of a data protection impact assessment;
* an organization’s internal AI policy;
* HR governance;
* contractual-compliance management;
* complete supplier qualification;
* Shadow AI mapping;
* a comprehensive cybersecurity audit;
* a formal conformity assessment;
* regulatory certification;
* attribution of a root cause to an observed behavioral change;
* proof that an isolated response is true, false, safe or compliant based on a single measurement signal;
* replacement of human judgment or the responsible organizational authority.

---

# 6. Positioning summary

**NeoMundi ControlTower is a runtime evidence, continuous monitoring and traceability layer for responses generated by AI systems.**

It helps organizations:

* observe AI-response behavior during operation;
* detect measurable drift and silent regime changes;
* document risk signals and their technical context;
* support human oversight and escalation mechanisms;
* apply configurable control mechanisms;
* retain auditable operational evidence;
* reduce content exposure through a privacy-first architecture;
* contribute to, without replacing, EU AI Act and GDPR compliance processes.

NeoMundi does not claim to determine whether an AI system is legally compliant.

It provides the operational evidence layer that helps organizations understand what their AI systems were doing in production, which signals were observed, which controls were available and which governance response was triggered.

---

# 7. Integration

ControlTower can be integrated:

* through a simple API call;
* without requiring replacement of the underlying AI infrastructure;
* in OBS mode;
* in GOV mode;
* through sovereign deployment models depending on the selected architecture;
* with configurable monitoring, threshold, alert and traceability parameters.

Available capabilities depend on the selected deployment model, depth of integration and organizational configuration.

### Access the platform

[**Create your account and API key →**](https://controltower.neomundi.io/welcome)

---

# 8. Disclaimer

This document describes NeoMundi ControlTower’s technical capabilities and intended operational contribution.

It does not constitute:

* legal advice;
* regulatory certification;
* a formal conformity assessment;
* an automatic guarantee of compliance;
* a complete assessment applicable to a specific organization or AI use case.

Compliance depends on several factors, including:

* the AI system concerned;
* its intended purpose;
* its risk classification;
* the context of use;
* the organization’s role;
* the applicable legal framework;
* the implemented technical and organizational measures;
* the governance and human-oversight processes maintained by the organization.

---

## NeoMundi

**Independent runtime measurement for AI systems.**

One measurement primitive. Multiple applications. Multiple infrastructures.

**NeoMundi provides the signal. Your organization retains authority.**
