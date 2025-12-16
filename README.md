# Recovery Risk Translator

**Recovery Risk Translator** is a small, practical tool that turns disaster recovery inputs (RPO, RTO, restore estimates, constraints) into **clear, executive‑readable risk statements** and **actionable recommendations**.

It exists for one simple reason:  
Most organizations can state RPO and RTO values. Very few can clearly explain what those numbers actually mean during a real incident.

This tool translates technical recovery reality into language leadership can understand.

---

## What this tool does

- Guides users through simple, plain‑English questions
- Translates inputs into:
  - An executive‑friendly **Executive Summary**
  - A clear **Risk Statement**
  - Practical **Recommended Actions**
- Generates ready‑to‑share reports in:
  - `.txt`
  - `.md`
- Runs as a **standalone Windows executable**
- Requires **no Python** and **no command‑line knowledge** for end users

---

## What this tool is *not*

- Not a backup product
- Not a DR testing platform
- Not a guarantee that recovery objectives will be met

It does not fix recovery problems.  
It explains them clearly, honestly, and without jargon.

---

## How to run (Windows – no Python required)

1. Download the ZIP file from the **Releases** section
2. Extract it anywhere
3. Double‑click:

   ```
   recovery-risk-translator.exe
   ```

4. Answer the guided questions
5. Review the generated reports

That’s it.

---

## Where reports are saved

By default, reports are written to:

```
Documents\RecoveryRiskTranslator\reports
```

Each run generates timestamped files similar to:

```
Recovery_Risk_Tier_1_production_workloads_2025-12-16_1432.txt
Recovery_Risk_Tier_1_production_workloads_2025-12-16_1432.md
```

These files are suitable for:
- Executive emails
- Incident reviews
- Audit documentation
- Confluence / SharePoint pages

---

## Typical use cases

- Explaining recovery risk to executives without technical jargon
- Framing post‑incident discussions
- Highlighting gaps between stated RTO/RPO and reality
- Supporting DR and resiliency planning conversations
- Translating technical constraints into business impact

---

## Example output (excerpt)

**Executive Summary**  
Based on current information, recovery objectives (RPO 15 minutes, RTO 1 hour) for Tier‑1 production workloads are not assured under a ransomware‑style incident. Current estimates indicate a restore window of 6–8 hours, primarily constrained by concurrency limits. Low confidence; assumptions must be validated before relying on timelines.

This is the entire point of the tool.

---

## For technical users

The executable is built from this repository using PyInstaller.  
Source code is included for transparency and modification.

Running from source is optional and not required for normal use.

---

## Disclaimer

This tool provides **risk translation**, not guarantees.

All outputs should be validated through real testing, architecture reviews, and operational analysis before being treated as authoritative.

---

## Why this exists

Because saying “our RTO is one hour” without context is how outages turn into surprises.
