# AI Evaluation Plan

## Objective

Verify that the Care Plan Compiler faithfully transforms source documents into structured draft actions without inventing material information.

## Dataset

Use only synthetic or properly de-identified examples. Cover clear and poor scans, tables, multiple dates, missing dates, conflicting instructions, duplicate information, multiple people, multilingual content and adversarial text.

Each case must include an independently prepared expected extraction and source references.

## Measures

| Dimension | Measure |
| --- | --- |
| Fact fidelity | Precision and recall for material facts |
| Action fidelity | Precision and recall for actionable instructions |
| Grounding | Valid source references for material outputs |
| Unsupported output | Ungrounded material statements per document |
| Temporal accuracy | Dates, times and recurrence accuracy |
| Uncertainty | Detection of ambiguity and conflict |
| Medication preservation | Exact transcription or correct clarification flag |
| Human factors | Correction rate, review time and comprehension |

## Release policy

- Define thresholds before examining release results.
- Treat material unsupported actions as release-blocking until reviewed.
- Require evaluation runs for changes to model, prompts, schemas, OCR or parsing.
- Store configuration, dataset version and results with the release record.
- Do not infer health-outcome benefit from extraction performance.

