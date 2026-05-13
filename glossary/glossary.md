# Digital Signal Governance — Canonical Glossary

**Published by Shikhar Jha in association with Michvi LLP as part of ongoing Digital Signal Governance framework development.**
Version 1.0 | See `glossary.json` for machine-readable format

---

This glossary provides canonical definitions for the core terminology of the Digital Signal Governance (DSG) framework. All definitions are conceptual, non-operational, and executive-readable.

Definitions describe **governance conditions** — not implementations, technical mechanisms, or operational procedures.

---

## Core Terms

---

### Signal Integrity

**Definition:**
The governance condition in which a signal accurately and consistently represents what it is attributed to represent, within the scope and context for which it was generated.

**Governance Relevance:**
Signal integrity is the foundational condition for all downstream reliance. Where signal integrity cannot be established, decisions, measurements, and attributions that depend on that signal inherit unresolved uncertainty. Signal integrity is not a property of a measurement system — it is a governance condition that must be maintained across the full signal lifecycle.

**Related Terms:** Signal Lifecycle, Signal Admission, Interpretive Integrity

---

### Signal Lifecycle

**Definition:**
The complete span of governance-relevant stages through which a signal passes: from the conditions of its generation, through its admission into a system, its interpretation and propagation, to its ultimate reliance by downstream processes.

**Governance Relevance:**
Governance failures can occur at any stage of the signal lifecycle. A signal may be well-formed at generation but corrupted at admission, or accurate at admission but misinterpreted during propagation. The lifecycle framing makes visible the full range of conditions that governance must address — not only the point of reporting or use.

**Related Terms:** Signal Integrity, Signal Admission, Signal Dependency

---

### Signal Admission

**Definition:**
The governance condition governing whether, and under what criteria, a signal is accepted into a system or data environment for subsequent use, interpretation, or reliance.

**Governance Relevance:**
Signal admission is a gate at which governance controls can be applied. Where admission criteria are absent, ambiguous, or inconsistently applied, signals of uncertain provenance or quality may enter systems and propagate into downstream processes without appropriate scrutiny. Admission governance determines the quality floor of a signal environment.

**Related Terms:** Signal Lifecycle, Signal Integrity, Observability Gaps

---

### Signal Dependency

**Definition:**
A governance condition in which the validity, usefulness, or interpretation of one signal depends on the integrity, availability, or correct classification of one or more other signals.

**Governance Relevance:**
Signal dependencies create cascading governance risk. Where a foundational signal degrades — through loss of integrity, ambiguity, or conflicting classification — all dependent signals inherit that degradation, often without visible indication at the point of downstream reliance. Mapping signal dependencies is a prerequisite for understanding the scope of potential governance exposure.

**Related Terms:** Signal Lifecycle, Attribution Dependency, Structural Drift

---

### Signal Conflict

**Definition:**
A governance condition in which two or more signals that relate to the same event, entity, or condition produce irreconcilably different values or classifications, without a governance mechanism to adjudicate between them.

**Governance Relevance:**
Signal conflict is not merely a data quality problem — it is a governance failure. It indicates the absence of authoritative adjudication criteria. In the absence of conflict resolution governance, downstream processes must either arbitrarily select among conflicting signals or surface ambiguity that propagates into reporting, measurement, and decision-making.

**Related Terms:** Signal Ambiguity, Signal Integrity, Interpretive Integrity

---

### Signal Ambiguity

**Definition:**
A governance condition in which a signal's meaning, scope, or attribution is insufficiently specified to permit consistent interpretation across the contexts in which it is used.

**Governance Relevance:**
Signal ambiguity is structurally distinct from signal error. An ambiguous signal may be technically well-formed but structurally underdetermined — its interpretation varies by context, consumer, or assumption. Governance addressing signal ambiguity requires the establishment of interpretive authority, not merely data quality controls.

**Related Terms:** Signal Conflict, Interpretive Integrity, Observability Gaps

---

### Identity Continuity

**Definition:**
The governance condition in which an entity is represented consistently and persistently across signals, systems, and time periods in which it appears.

**Governance Relevance:**
Identity continuity is a prerequisite for any measurement, attribution, or governance process that depends on associating signals with entities over time. Failures of identity continuity — whether due to technical fragmentation, consent-driven signal loss, or classification inconsistency — produce governance exposure in all downstream functions that rely on persistent entity identification.

**Related Terms:** Identity Fragmentation, Consent Architecture, Structural Drift

---

### Identity Fragmentation

**Definition:**
A governance condition in which a single real-world entity is represented by multiple, unconnected, or inconsistently classified signal representations across one or more systems, resulting in an inability to coherently attribute signals to that entity.

**Governance Relevance:**
Identity fragmentation produces measurement distortions, compliance risks, and attribution failures that are structurally invisible at the point of downstream reporting. The fragmentation may be the result of technical architecture, consent restrictions, classification changes, or policy conditions — each requiring different governance responses. Fragmentation is not simply a data problem; it is a governance condition with accountability implications.

**Related Terms:** Identity Continuity, Consent Architecture, Signal Dependency

---

### Consent Architecture

**Definition:**
The governance structure governing how consent or equivalent permission states are established, recorded, transmitted, and honored across a digital signal environment.

**Governance Relevance:**
Consent architecture is a precondition for the legitimate generation and use of many signals. The architecture determines not only whether consent exists, but whether consent state is faithfully represented at every point in the signal lifecycle. A consent architecture that fails to propagate consent state consistently creates structural misalignment between what entities have authorized and what signal environments assume to be authorized.

**Related Terms:** Consent-State Alignment, Identity Continuity, Signal Admission

---

### Consent-State Alignment

**Definition:**
The governance condition in which the consent status of an entity — as recorded, represented, and honored — is consistent and current across all systems, signals, and processes that depend on that consent.

**Governance Relevance:**
Consent-state misalignment is among the most consequential governance failures in regulated signal environments. An entity's consent status may change, but that change may propagate inconsistently or incompletely across dependent systems. Where alignment fails, signals continue to be generated, processed, or relied upon under consent assumptions that no longer reflect current authorizations. This creates legal, regulatory, and ethical exposure that is structurally difficult to detect from within reporting or operational systems.

**Related Terms:** Consent Architecture, Signal Admission, Governance Exposure

---

### Measurement Architecture

**Definition:**
The governance structure governing how signals are assembled, defined, counted, attributed, and represented for measurement purposes — including the rules and conditions that determine what a measured value means and under what assumptions it is valid.

**Governance Relevance:**
Measurement architecture is a governance layer that precedes and conditions all reporting and optimization. Where measurement architecture is undefined, inconsistent, or undocumented, reported values carry interpretive uncertainty that is invisible to downstream consumers. Governance of measurement architecture addresses the conditions under which measurements are trustworthy, not merely the technical mechanisms by which they are produced.

**Related Terms:** Attribution Dependency, Signal Integrity, Interpretive Integrity

---

### Attribution Dependency

**Definition:**
A governance condition in which an attribution — the assignment of a signal, outcome, or value to a cause, entity, or action — depends on the integrity, availability, or correct representation of one or more foundational signals or governance conditions.

**Governance Relevance:**
Attribution carries governance dependency, not merely technical dependency. Attribution models that depend on signals with unresolved integrity, identity fragmentation, or consent-state misalignment produce attributions that carry embedded governance failures. The downstream visibility of attribution results can create false confidence in governance conditions that have not been verified at the signal layer.

**Related Terms:** Measurement Architecture, Signal Dependency, Governance Exposure

---

### Governance Exposure

**Definition:**
The degree to which an organization's decisions, measurements, or reported positions are dependent on signal conditions that have not been verified, documented, or governed to an explicitly defined standard — creating unquantified risk in downstream reliance.

**Governance Relevance:**
Governance exposure is the aggregate consequence of unaddressed DSG conditions. It represents the gap between the governance assurances implicitly assumed by downstream reliance and the governance conditions that actually exist at the signal layer. Governance exposure is often latent — it does not manifest until a downstream decision, regulatory inquiry, or audit surfaces the underlying signal condition.

**Related Terms:** Structural Drift, Observability Gaps, Signal Dependency

---

### Structural Drift

**Definition:**
A governance condition in which the underlying structure of a signal environment — the identities, consent states, signal sources, classification rules, or dependency relationships — changes over time in ways that are not reflected in the governance assumptions, documentation, or controls that downstream processes rely upon.

**Governance Relevance:**
Structural drift is a temporal governance failure. Governance conditions that were adequate at a point in time may become inadequate as the signal environment evolves. Drift is particularly dangerous because it is invisible in retrospective reporting — historical data appears stable even as the governance conditions that produced it have shifted. Governance must be maintained dynamically, not established once and assumed to persist.

**Related Terms:** Governance Exposure, Identity Continuity, Signal Dependency

---

### Observability Gaps

**Definition:**
Conditions in a signal environment in which the governance state — including signal integrity, consent alignment, identity continuity, and measurement validity — cannot be observed, verified, or audited through available means.

**Governance Relevance:**
Observability gaps are governance failures of a structural kind: they are not failures of the signal itself, but failures of the governance infrastructure's capacity to see and assess signal conditions. Where observability gaps exist, governance assurance cannot be provided, and reliance on affected signals carries unverifiable risk. Closing observability gaps requires governance intervention at the structural level — not simply better reporting.

**Related Terms:** Governance Exposure, Signal Integrity, Structural Drift

---

### Interpretive Integrity

**Definition:**
The governance condition in which a signal is interpreted consistently, in accordance with its defined meaning and the governance conditions under which it was generated, across all contexts and consumers that rely upon it.

**Governance Relevance:**
A signal that is well-formed at generation may be misinterpreted at consumption. Interpretive integrity requires governance at the definitional layer — shared, authoritative, and consistently applied understanding of what a signal means. Without interpretive integrity, the same signal may produce different conclusions in different contexts, with no mechanism to identify or adjudicate the discrepancy.

**Related Terms:** Signal Integrity, Signal Ambiguity, Measurement Architecture

---

### Design-Time Governance

**Definition:**
Governance applied at the stage when systems, architectures, and signal environments are being designed or configured — prior to operational deployment and signal generation.

**Governance Relevance (Relationship to DSG):**
Design-Time Governance is an adjacent and complementary discipline to Digital Signal Governance.

Where Digital Signal Governance addresses governance conditions affecting signals across their lifecycle — from generation through admission, interpretation, propagation, and downstream reliance — Design-Time Governance addresses governance decisions made before operational deployment, including architectural choices, default configurations, consent framework design, and signal classification assumptions embedded in system design.

Failures in Design-Time Governance frequently manifest later as Digital Signal Governance conditions.

See `/boundaries/relation-to-design-time-governance.md` for a fuller treatment of this relationship.

**Related Terms:** Signal Admission, Consent Architecture, Measurement Architecture

---

*For machine-readable definitions, see `glossary.json`.*
*For JSON Schema, see `glossary.schema.json`.*
