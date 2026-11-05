# Verification and known limitations

**Security update:** Supporting dependency pins, the local viewer launcher, and evaluation error classification were updated after the live runs described below. Those historical live results do not constitute a new live test of this archive. The security update is verified with fresh installations, offline SDK checks, recorded-result replay, and local viewer tests. Models, scoring criteria, reference datasets, and unfinished exercises are preserved.

Historical API-backed baseline: the learner configuration and separate reference configuration each ran all 11 rows against `gpt-5` on 2026-09-01, with no runtime/grader errors. They produced 6/11 and 7/11 passing rows respectively; this illustrates grading variability, not a required pass count. The current Lab 01 configuration instead uses Codex SDK with `gpt-6-luna` as the rubric judge; it has not yet received a live end-to-end run in this bundle.

The Academy lesson is written for API-key-backed OpenAI rubric graders. This bundle keeps the same prewritten-answer `echo` target, rubrics, thresholds, and deterministic equality check, but configures Codex SDK as the rubric judge so Lab 01 can use an existing Codex sign-in. The screenshot shows an earlier illustrative run.

All starter TODOs remain. Generated answers, evaluation histories, credentials, prior resource IDs, and unrelated labs are excluded. Windows and Linux instructions were reviewed, not runtime-tested on those systems. The verification host was macOS with Python 3.13.0 and Node 24.19.0; Python 3.12 was not executed.

The standard [MIT license](LICENSE) was added at the packaging requester’s direction; original source attribution is retained in [ATTRIBUTION.md](ATTRIBUTION.md).
