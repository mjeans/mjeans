# A guided review of my portfolio

My work spans nutritional sciences, public health, education, quantitative evaluation, and research delivery. These routes point to the evidence behind the project summaries—not just screenshots or lists of techniques.

## Nutrition, epidemiology, and public health

Start with my [first-author TX Sprouts paper](https://pmc.ncbi.nlm.nih.gov/articles/PMC10375509/), then inspect the [executed NHANES nutrition analysis](https://github.com/mjeans/nhanes-nutrition-survey-analysis/blob/main/outputs/report.md). The paper represents published research; the repository is a separate portfolio analysis of CDC public-use data.

**Look for:** two-day dietary measurement, energy adjustment, appropriate survey weights, domain estimates, uncertainty, and explicit cohort/missingness accounting. The [Public Health Methods Lab](https://github.com/mjeans/public-health-methods-lab) complements this with synthetic age-standardization, outbreak, surveillance, survival, and nutrition examples.

**A useful review question:** What population and measurement window does an estimate represent? Two recalls are not usual intake, and descriptive associations do not identify a dietary intervention effect.

## Machine learning and education data science

The [education predictive-modeling report](https://github.com/mjeans/student-success-predictive-modeling/blob/main/outputs/report.md) follows a model from development to a later academic-year test cohort. The [input-monitoring extension](https://github.com/mjeans/student-success-predictive-modeling/blob/main/outputs/input-monitoring-report.md) then asks what happens when a scoring feed arrives with wrong units or substantially more missing data.

**Look for:** validation-only model and threshold selection, probability calibration, capacity drift, subgroup errors, a strict predictor boundary, and monitoring that separates invalid inputs from distribution changes. All student records are synthetic; this is not a claim of deployed student-risk prediction.

**A useful review question:** What must happen before a score becomes an action? A model score alone does not authorize outreach, discipline, or denial of support.

## Evaluation and quantitative research

- [Quasi-experimental evaluation](https://github.com/mjeans/quasi-experimental-program-evaluation/blob/main/outputs/report.md): inspect overlap and balance before effect estimates; distinguish the full ATT from the retained matched-treated subset.
- [Multilevel outcomes](https://github.com/mjeans/multilevel-outcomes-analysis/blob/main/outputs/report.md): inspect person/organization variance, time interactions, and the independent-cluster count—not just the number of repeated observations.
- [Structural equation modeling](https://github.com/mjeans/structural-equation-modeling/blob/main/outputs/report.md): review measurement invariance and solution diagnostics before structural paths. Excellent fit to data generated from the model is an implementation check, not empirical confirmation of the theory.

All three repositories use synthetic data. The substantive interpretations are demonstrations with visible assumptions, not client findings.

## Data systems, SQL, and operational decisions

Start with the [Stata enrollment and service-revision example](https://github.com/mjeans/administrative-data-pipeline/tree/main/examples/stata-enrollment), the [multisource pipeline audit](https://github.com/mjeans/administrative-data-pipeline/blob/main/outputs/report.md), and the [data-quality toolkit](https://github.com/mjeans/evaluation-data-quality-toolkit).

Then inspect [as-of cohort SQL](https://github.com/mjeans/sql-analytics-case-study/blob/main/outputs/as-of-report.md): new members should not become retention failures before their observation window has closed. The [student-success operations dashboard](https://github.com/mjeans/student-success-operations-dashboard) connects metrics to an action queue, with source-generated SVG previews and explicit decision rules.

**Look for:** grain-preserving joins, missing-versus-zero distinctions, deterministic schema recovery, temporal boundaries, tests that exercise failure cases, and traceable metrics. Dashboard previews are not presented as a tested native Power BI deployment; event-time snapshots are not ingestion-time reconstructions.

## Research leadership and delivery

The [second dietary recall decision memo](https://github.com/mjeans/research-project-management-toolkit/blob/main/examples/nutrition-evaluation/second-recall-decision.md) is a short fictional leadership exercise. It distinguishes a delayed upload from a scheduling barrier, assigns owners, and specifies when to stop or continue a small change.

The surrounding toolkit supplies governance gates, work plans, risks, and requirement-to-deliverable traceability. It demonstrates how I would structure a decision, not a claim that the fictional pilot took place.

## Verify a claim

For any project, follow the result to its source table, then to the generating code and test. Read its reproduction commands and license. Check the latest GitHub Actions run separately: a passing workflow supports the checks it runs, not every possible scientific or operational use.

[Back to profile](README.md) · [Publications](https://www.ncbi.nlm.nih.gov/myncbi/matthew.jeans.1/bibliography/public/) · [ORCID](https://orcid.org/0000-0002-1140-3185)
