<div align="center">

<sub><b>English</b> · <a href="README_FR.md">Français</a></sub>

# NeoMundi — AI Act & GDPR

### From measurement to technical evidence for AI governance.

**Measure behaviour, document observation conditions and verify technical artefacts that can support AI governance and compliance work.**

**Measurement → Station → Evidence**

[![Measurement](https://img.shields.io/badge/Measurement-Measure-2563eb?style=flat-square)](https://github.com/neomundi-io/neomundi-runtime-measurement)
[![Station](https://img.shields.io/badge/Station-Observe-0f766e?style=flat-square)](https://github.com/neomundi-io/neomundi-station-public)
[![Evidence](https://img.shields.io/badge/Evidence-Verify-D4A545?style=flat-square)](https://github.com/neomundi-io/neomundi-evidence-public)
[![Use cases](https://img.shields.io/badge/Use_cases-Explore-64748b?style=flat-square)](https://github.com/neomundi-io/neomundi-use-cases)

**[API](https://github.com/neomundi-io/neomundi-runtime-measurement/blob/main/QUICKSTART.md)** · **[Create an account](https://controltower.neomundi.io/welcome)**

</div>

---

## What NeoMundi contributes

Organisations need to explain what their AI produced, under what conditions, which signals were measured and what records can be inspected. NeoMundi supplies the technical building blocks to answer those questions.

| Product | Operational contribution | Start here |
|---|---|---|
| **[Measurement](https://github.com/neomundi-io/neomundi-runtime-measurement)** | Versioned response measurements, status, evaluator coverage and bounded risk signals. | [API quickstart](https://github.com/neomundi-io/neomundi-runtime-measurement/blob/main/QUICKSTART.md) |
| **[Station](https://github.com/neomundi-io/neomundi-station-public)** | Observation campaigns, execution context, records, provenance and export. | [Overview](https://github.com/neomundi-io/neomundi-station-public) |
| **[Evidence](https://github.com/neomundi-io/neomundi-evidence-public)** | Archive-integrity verification, artefact traceability and Ed25519 attestation checks. | [User guide](https://github.com/neomundi-io/neomundi-evidence-public/blob/main/docs/EVIDENCE_USER_GUIDE.md) · [Demo](https://github.com/neomundi-io/neomundi-evidence-public/blob/main/docs/EVIDENCE_TECHNICAL_DEMO.md) |

**Demonstrated:** a real experimental Q-2 qualification traversed Measurement → Station → Evidence, including a verified Ed25519 attestation. Technical checks passed in their tested scope; **overall Q-2 verdict PARTIAL**. Its source dossier is private. See the [Evidence validation report](https://github.com/neomundi-io/neomundi-evidence-public/blob/main/docs/EVIDENCE_VALIDATION_REPORT.md).

## Where this evidence may help

| Governance need | Potential contribution | To confirm per deployment |
|---|---|---|
| **Traceability and logging** | IDs, measurements, campaign records, hashes, verifiable archives | Capture, completeness, exports, retention and access |
| **Human oversight** | Signals to inform designated reviewers and escalation | Alerts and routing actually configured in the consuming system |
| **Quality and drift monitoring** | Longitudinal comparison of compatible instrumented measurements | Protocol, frequency, coverage and validated thresholds |
| **Incident investigation and audit** | Traceable technical dossiers, verification results and attestations | Chain of custody, available records and limits of evidence |
| **Data protection** | Minimisation options and content-limited exports for selected paths | Actual flows, evaluators, processors and retention |

This matrix describes a **potential technical contribution**, not certification of compliance or a claim that all mechanisms are available in every integration. The API route, integration and deployment determine what operates. Authorization, blocking and compliance decisions remain with the organisation.

## EU AI Act timeline — checked 7 November 2026

[Regulation (EU) 2024/1689](https://eur-lex.europa.eu/eli/reg/2024/1689/oj), as amended notably by [Regulation (EU) 2026/1744](https://eur-lex.europa.eu/eli/reg/2026/1744/oj), applies progressively:

| Date | Main provisions |
|---|---|
| **2 February 2025** | Initial definitions, AI literacy and prohibited practices |
| **2 August 2025** | General-purpose AI model rules |
| **2 August 2026** | Majority of other provisions, including several transparency obligations |
| **2 December 2026** | Additional specified prohibitions and certain Article 50(2) transitional requirements |
| **2 December 2027** | High-risk AI rules for Annex III systems |
| **2 August 2028** | High-risk AI rules for Annex I product-embedded systems |

**Primary references:** [European Commission implementation timeline](https://ai-act-service-desk.ec.europa.eu/en/ai-act/eu-ai-act-implementation-timeline) and [amending regulation in the Official Journal](https://eur-lex.europa.eu/eli/reg/2026/1744/oj). The applicable obligations depend on the organisation's role, system purpose and relevant provisions.

## Detailed operational reference

The sections below retain the existing AI Act/GDPR mappings, data flows and possible control mechanisms. Configurable capabilities must be checked per integration; a measurement score does not independently grant authority to act.

---

# 1. What NeoMundi actually covers

## 1.1. Operational traceability of observed AI responses

NeoMundi associates observed events related to AI responses with technical and operational artifacts that may include:

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

## 1.2. Monitoring AI-response behavior

NeoMundi continuously observes signals associated with the behavior of AI systems during operation.

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

NeoMundi can help identify measurable changes in the behavior of an AI system over time.

A behavioral change may appear even when:

* no public provider update has been announced;
* no visible production incident has yet been reported;
* a point-in-time benchmark remains broadly reassuring;
* conventional quality snapshots do not reveal the change.

These observations may concern changes in factual-risk signals, semantic variation, stability or other monitored indicators.

NeoMundi does not attribute the cause of a detected behavioral change unless an independent investigation establishes it.

A detected signal is an operational observation. By itself, it is not proof of a provider change, system failure, legal breach or root cause.

### Covered capability

**Detection and traceability of measurable behavioral drift and silent regime changes in production.**

---

## 1.4. Configurable governance and control mechanisms

NeoMundi can support configurable governance mechanisms applied in real time or near real time, depending on the selected integration.

These mechanisms may include:

* risk thresholds;
* alerts;
* escalation paths;
* routing to human review;
* differentiated treatment of higher-risk responses;
* configurable blocking or hold mechanisms where supported by the selected integration;
* observation and decision logs;
* auditing of rule application and measurement history.

NeoMundi does not silently turn an observed signal into an authorized action.

A measurement signal may justify information, review or escalation, but the authority to act remains defined by the organization’s governance rules, accountable roles and selected integration.

### Covered capability

**Continuous monitoring and configurable mechanisms for controlling risks associated with AI responses.**

---

## 1.5. Support for human oversight

NeoMundi can support human oversight by making relevant runtime signals visible and actionable.

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

NeoMundi produces measurable and verifiable technical elements that may include:

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

NeoMundi does not rely solely on declarative claims about the reliability of an AI system.

It provides measured, traceable and configurable signals that can help organizations make their governance processes more explicit.

For example, an organization can use NeoMundi to document that:

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

NeoMundi is designed to support data minimization, but NeoMundi has several distinct data flows. No organization-wide claim of zero transmission, zero storage or zero retention is made here.

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

# 3. How NeoMundi can contribute to an EU AI Act compliance process

NeoMundi does not replace legal analysis, conformity assessment, organizational governance or regulatory certification.

It nevertheless provides technical capabilities and runtime evidence that can contribute to several operational areas relevant to an EU AI Act compliance process.

The applicability of these areas depends on the AI system, its intended purpose, the organization’s role, the system’s risk classification and the specific use case.

| Operational area | NeoMundi contribution | Coverage level |
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

A central contribution of NeoMundi is its ability to create a longitudinal history of the observed behavior of an AI system during operation.

This can help organizations identify:

* unexpected variation;
* an increase in factual-risk signals;
* changes in semantic behavior;
* degradation in observed stability;
* changes in the distribution of risk;
* silent regime changes;
* patterns requiring review before they become visible through traditional incident-reporting processes.

NeoMundi does not replace an incident investigation.

It helps establish that an operational signal was observed, measured and documented at a given time within a defined measurement and governance context.

## 3.2. The distinction between measurement and authorization

NeoMundi is built around an essential governance distinction:

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

# 4. How NeoMundi can contribute to a GDPR compliance process

NeoMundi is designed to support privacy-first data-processing principles.

It does not replace a complete GDPR analysis, a record of processing activities, a data protection impact assessment, or the legal responsibility of a controller or processor.

Its architecture can nevertheless provide technical support for several GDPR-related operational principles.

| GDPR-related area | NeoMundi contribution | Coverage level |
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
| Management of data-subject rights | Requires organizational procedures and systems beyond NeoMundi | Out of scope |

---

# 5. What NeoMundi does not cover

NeoMundi does not replace an organization’s legal, organizational, security or governance responsibilities.

NeoMundi does not provide:

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

**NeoMundi NeoMundi is a runtime evidence, continuous monitoring and traceability layer for responses generated by AI systems.**

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

NeoMundi can be integrated:

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

This document describes NeoMundi NeoMundi’s technical capabilities and intended operational contribution.

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
