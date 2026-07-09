# conedbudgetmodel
A dynamic budget model for a university continuing education program, built for a real 22-week program cycle. Includes a 4-variable sensitivity analysis, ROI/break-even modeling across enrollment scenarios, and a staffing right-sizing scenario that cuts the projected deficit by over 75%. Anonymized from a project I led professionally.
Continuing Education Program — Budget Model & Sensitivity Analysis

A dynamic budget model for a university continuing education program, built for a real 22-week program cycle. Includes a 4-variable sensitivity analysis, ROI/break-even modeling across enrollment scenarios, and a staffing right-sizing scenario that cuts the projected deficit by over 75%.

Anonymized from a project I led professionally — institution name, staff names, and exact figures have been generalized for a public portfolio; the structure, logic, and analytical approach are unchanged from the live version used for planning.

What's Inside

The workbook has six tabs, meant to be read in order:

TabWhat it doesAssumptionsEvery input (rates, hours, enrollment, pricing) as an editable, color-coded cell — change any of them and the rest of the workbook recalculatesBudget ModelCost build by category (personnel, platform, communications, presenter honoraria, assessor honoraria), plus a revenue/net-position layerSensitivity AnalysisFour tests: enrollment × assessor-hours, personnel rate swings, enrollment × pricing tiers, and a tornado-style ranking of which assumption moves the budget mostROI & BreakevenSolves for the enrollment each channel (webinars, workshops, courses) would need — alone — to reach ROI = 0, under two Open Call outcome scenariosPrudent ScenarioTests a more measured operating model: reduced staffing hours, evergreen courses run as repeatable cohorts, and a couple of continuation webinars — compared directly against the original planDashboardCost composition, break-even by scenario, and variable-impact charts

Key Findings


Personnel dominates the budget — roughly 90%+ of confirmed costs — so it's the single biggest lever in the model, bigger than enrollment or pricing.
A modeling correction mattered: assessor review time scales in batches of ~10 participants, not per individual. Fixing this cut that cost line by ~90% at typical enrollment and prevented the model from wildly overstating costs at higher enrollment.
Enrollment alone can't close the deficit. Breaking even through webinar or workshop attendance alone would require 145–386 people in a single session — not realistic for this audience. Evergreen courses are the most efficient lever, needing only ~6x growth to break even on their own.
Right-sizing staffing does more than growing enrollment. Reducing Instructional Technologist hours (35→20/week) and Program Supervisor hours (17→15/week), combined with running courses as smaller repeatable cohorts instead of one large intake, cuts the projected deficit by 57–77% and brings the break-even growth target down from ~4.6x to a realistic 1.3–1.9x.


How to Use


Open Assumptions first — every blue cell is a live input.
Read Budget Model for the base-case cost and revenue build.
Sensitivity Analysis and ROI & Breakeven stress-test that base case.
Prudent Scenario shows an alternative operating model and compares it side-by-side against the original.
Dashboard summarizes everything visually.


Tools

Built with Python (openpyxl) for formula generation and formatting; all figures are live Excel formulas, not hardcoded values.

License

MIT — see LICENSE.
