================================================================================
STUDENT DROPOUT RISK 2026 — COMPLETE ANALYSIS PACKAGE
================================================================================

WHAT'S INSIDE
-------------

student_dropout_risk_2026_readout.pptx
    5-slide presentation (Clean Academic style) for the read-out session.
    Slides: 1) Cover  2) Headline numbers  3) Academic signals
            4) Financial signals  5) Risk ranking & recommended actions.
    Each slide carries short speaker-note hints (View > Notes in PowerPoint).

presentation_script.md
    The read-out script: talking-point cues per slide (~5-7 minutes total),
    a Q&A cheat sheet for likely questions, and a one-page numbers cheat card.
    Open this next to the PPT while presenting.

charts/  (8 PNG files, 300 DPI, presentation-ready)
    01_dropout_overview.png ....... headline donut: 32.0% dropped out
    02_gpa_cliff.png .............. dropout rate by semester-2 GPA band
                                    (83.5% at <1.0 down to 2.4% at 3-4)
    03_academic_gap.png ........... attendance / assignments / deadlines,
                                    dropouts vs retained
    04_engagement_gap.png ......... library visits and LMS logins by outcome
    05_income_gap.png ............. dropout rate by family income level
    06_financial_pressure.png ..... work-hours dose-response + tuition status
    07_risk_ranking.png ........... standardized logistic regression ranking
                                    (red = raises risk, indigo = protective)
    08_corr_heatmap.png ........... correlation map of 13 key variables

data_summary.txt
    Dataset inspection: shape, 34-column inventory, data-quality checks
    (0 missing values, 0 duplicates, all ranges valid), cohort composition,
    and the average student profile.

key_facts.txt
    33 presentation-ready facts in 7 groups (headline, academic, financial,
    engagement & wellbeing, null results, model ranking, practical
    implications). Every number is computed from the full dataset.

statistical_tests.txt
    Full test results for a data-literate audience: Welch t-tests with
    Cohen's d and point-biserial r, chi-square tests with Cramer's V, and
    the standardized logistic regression table with odds ratios and 95% CIs.
    Includes the "with n = 100,000, read effect sizes not p-values" caveat.

HEADLINE FINDINGS (for the impatient)
-------------------------------------
- 32.0% of 100,000 students dropped out (32,004).
- Semester-2 GPA is a cliff: <1.0 -> 83.5% dropout; 3.0-4.0 -> 2.4% (35x).
- Family income is the strongest demographic factor: Low 42.9% vs High 20.0%.
- Work hours show a dose-response: 24.7% (no job) -> 46.0% (21-40 h/week).
- Overdue tuition: 44.2% vs 28.7% dropout.
- Nulls: gender, nationality, course type, international status, age.
- Recommended early-warning flag: semester-1 GPA < 2.0 AND attendance < 75%.

METHOD NOTES
------------
All statistics computed on the complete 100,000-record dataset (no sampling).
Analysis pipeline: pandas + SciPy (t-tests, chi-square, point-biserial),
statsmodels (standardized logistic regression), matplotlib/seaborn (charts).
Observational data — findings are associations, not causal estimates.
