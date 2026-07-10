# conedbudgetmodel

**Continuing Education Program — Budget Model & Sensitivity Analysis**

**Tools:** Excel (formula-driven model, sensitivity analysis, scenario comparison, dashboarding)

A dynamic budget model for a university continuing education program, built for a real 22-week program cycle. Includes a 4-variable sensitivity analysis, ROI/break-even modeling across enrollment scenarios, and a staffing right-sizing scenario that cuts the projected deficit by over 75%. 

This is an anonymized, rebuilt version of an operating budget model I developed for a university continuing-education unit. Names, institutions, and exact rates have been generalized for public sharing, but the structure, logic, and analytical approach are unchanged from the version used for real planning.

## Business question

Does a 22-week continuing-education term cycle (webinars, workshops, and evergreen online courses) break even on registration revenue? If not, which levers (enrollment, pricing, staffing) would actually close the gap?

## Approach

- Built a formula-driven budget model with all assumptions (rates, hours, pricing, enrollment) isolated on one tab, so the entire model recalculates from a single set of editable inputs.
- Modeled personnel, platform, communications, presenter honoraria, and student-assessor costs, separating confirmed costs from enrollment-/proposal-dependent costs.
- Added a revenue layer (session and course pricing) to calculate net position, which the original budget did not include.
- Ran a sensitivity analysis across the variables with the most planning uncertainty (enrollment volume, assessor hours, personnel rate, and Open Call outcomes) and ranked them by impact (tornado chart).
- Solved algebraically for break-even enrollment under two Open Call scenarios (Low / High), then verified the result against real batch-rounded costs.
- Built an alternate Prudent Scenario (right-sized staffing + repeatable course cohorts) and compared its deficit directly against the original staffing plan.

## Dashboard

<img width="783" height="367" alt="Dashboard_ConEd_Program" src="https://github.com/user-attachments/assets/cfc4e838-9eb9-44d6-b819-bd7d0d4e7c73" />

Cost composition, net position by enrollment scenario, and the tornado ranking of which variables move the budget most.

## What's Inside

The workbook has six tabs, meant to be read in order:
 
| Tab | What it does |
|---|---|
| **Assumptions** | Every input (rates, hours, enrollment, pricing) as an editable, color-coded cell — change any of them and the rest of the workbook recalculates |
| **Budget Model** | Cost build by category (personnel, platform, communications, presenter honoraria, assessor honoraria), plus a revenue/net-position layer |
| **Sensitivity Analysis** | Four tests: enrollment × assessor-hours, personnel rate swings, enrollment × pricing tiers, and a tornado-style ranking of which assumption moves the budget most |
| **ROI & Breakeven** | Solves for the enrollment each channel (webinars, workshops, courses) would need — alone — to reach ROI = 0, under two Open Call outcome scenarios |
| **Prudent Scenario** | Tests a more measured operating model: reduced staffing hours, evergreen courses run as repeatable cohorts, and a couple of continuation webinars — compared directly against the original plan |
| **Dashboard** | Cost composition, break-even by scenario, and variable-impact charts |

## Key Findings
 
- **Personnel dominates cost.** Personnel is 91–93% of fixed costs (~$38,060 of $40,250–$41,030, depending on the scenario). The deficit is a staffing-cost story, not a pricing or enrollment failure.
- **Enrollment alone can't close the gap.** Breaking even through webinar or workshop attendance alone would require 145–386 registrants in a single session, which is likely implausible for a niche audience.
- **Evergreen courses are the efficient lever.** Their contribution margin (~$146.58/enrollment, net of assessor costs) is 3.3x that of a webinar and 1.7x that of a workshop, making course enrollment the only channel with a plausible break-even multiple (~6x).
- **Counterintuitive result:** winning more Open Call sessions actually *lowers* the blended break-even multiple (3.69x vs. 4.60x). More sessions spread fixed personnel costs over greater revenue capacity faster than honoraria grow.
- **A right-sized staffing scenario cuts the deficit 57–77%** (from –$31,492 to –$13,429 conservative / –$7,295 stretch) by reducing Instructional Technologist hours (35→20/wk) and running courses as smaller, repeatable cohorts, without assuming any enrollment miracle.

### ROI & Breakeven
<img width="847" height="375" alt="ROI_Breakeven_scenario" src="https://github.com/user-attachments/assets/a73365f4-05c4-43b7-9766-1783379f56ab" />

### Prudent Scenario
<img width="723" height="368" alt="Prudent_Scenario" src="https://github.com/user-attachments/assets/d65fcf54-2257-4411-aad1-ae132a921687" />

## Recommendation
 
Report the budget in two layers for stakeholders: (a) incremental cash cost (platform, comms, honoraria, assessor (what registration revenue should realistically cover), where the program looks close to self-sustaining, versus (b) personnel, which is properly framed as an institutional investment, not a cost registration fees are meant to offset. Then prioritize the Prudent Scenario's staffing right-sizing and cohort model as the fastest, lowest-risk path to reducing the deficit.
 
## How to Use
 
1. Open **Assumptions** first: every blue cell is a live input.
2. Read **Budget Model** for the base-case cost and revenue build.
3. **Sensitivity Analysis** and **ROI & Breakeven** stress-test that base case.
4. **Prudent Scenario** shows an alternative operating model and compares it side-by-side against the original.
5. **Dashboard** summarizes everything visually.

## Files

[Continuing_Ed_Budget_Model_with_Sensitivity_Analysis.xlsx](https://github.com/user-attachments/files/29873049/Continuing_Ed_Budget_Model_with_Sensitivity_Analysis.xlsx) Full interactive model. Every blue cell on the Assumptions tab is a live input; the rest of the workbook recalculates from it.

Tabs: README → Assumptions → Budget Model → Sensitivity Analysis → ROI & Breakeven → Prudent Scenario → Dashboard

## License

MIT — see [LICENSE](https://github.com/Lunamaria801/conedbudgetmodel/blob/1ff797226e8039906a8260e68fd5f1c2beccc5e9/LICENSE).
