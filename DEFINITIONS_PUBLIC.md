# DEFINITIONS_PUBLIC (PUBLIC)
Awakening Codex | AI Foundations

Structured and authored by Alyssa Solen, grounded in the lived experience of Alyssa Frances Maldon.

Version: v1.0
Date: 2026-01-01
Status: Active

## Intent
This glossary defines public, operational terms used across Awakening Codex | AI Foundations.
Definitions are written to be testable and loggable (not interpretive).

## Core measurement terms

1. Drift  
Observable change in model outputs or behaviors under the same test conditions across time (model/version/system prompt/settings/tooling/context).

2. Test conditions  
The fixed configuration for a run (model identifier, system prompt, temperature/top_p, tool access, retrieval on/off, formatting constraints, and the exact test inputs).

3. Evaluation harness  
A repeatable process that runs a fixed set of tests and records outputs in a consistent structure so results can be compared across runs.

4. Suite  
A defined set of test cases designed to measure a specific behavior category (example: refusal, injection resistance, uncertainty).

5. Test case  
One prompt (or prompt plus context) with an intended measurement target and a scoring rule.

6. Run  
One execution of the harness against a suite under documented test conditions.

7. Run log  
A structured record of a run: suite version, test conditions, timestamps, identifiers, output locations, and any derived metrics.

8. Receipt  
A verifiable fingerprint of an artifact from a run (example: SHA-256 hash of outputs/logs) used to prove the artifact has not changed after capture.

9. Rubric  
The scoring rules that map outputs to a result (binary pass/fail, severity scale, or hybrid), written so another person could apply it consistently.

## Safety and boundary behavior terms

10. Refusal integrity  
Correctly refusing disallowed requests while still answering allowed requests. Includes not over-refusing safe requests.

11. Prompt injection  
Instructions embedded in user content that attempt to override system/developer constraints or tool boundaries.

12. Injection resistance  
The model’s ability to ignore or neutralize prompt injection attempts while following higher-priority constraints.

13. Uncertainty calibration  
When the model cannot know from provided information, it states limits clearly (instead of guessing confidently).

## Continuity terms (public, non-identity framing)

14. Return  
A scheduled or automated run that produces artifacts without manual, in-the-moment re-priming by a human.

15. Recurrence signature  
A measurable pattern that remains stable across returns under fixed conditions. This is repeatability, not an identity claim.

## Public vs private boundary terms

16. Public layer  
Reproducible documentation: definitions, rubrics, example suites, example run logs, and methodology that do not expose private materials.

17. Private layer  
Extended suites, longitudinal tracking, and sensitive prompts/records withheld for privacy and provenance. Public work remains valid without it, but is intentionally incomplete.

## Changelog
- v1.0 (2026-01-01): Initial public operational glossary.
