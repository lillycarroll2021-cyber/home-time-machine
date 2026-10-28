# Home Time — Product Requirements Document (PRD)

**Version:** 1.0 · Hackathon concept · 28 October 2026  
**Status:** Interactive discovery prototype; not a launched financial product  
**Product:** Home Time  
**Prototype:** https://lillycarroll2021-cyber.github.io/home-time-machine/  
**Repository:** https://github.com/lillycarroll2021-cyber/home-time-machine

---

## 1. Executive summary

Home Time is a consumer-first mortgage and homeownership companion. It aims to turn a mortgage from a mostly passive monthly payment and occasional renewal task into an ongoing, understandable relationship between people, their home and their financial future.

The central feature is the **Home Time Machine**: an interactive visual experience that helps people explore the estimated effect of extra mortgage payments over time. Around that core, Home Time proposes everyday cashback and rewards, practical overpayment guidance, personalised homeownership milestones, goals such as moving or renovating, and — in future — securely connected financial information.

This PRD describes **the vision, the current hackathon prototype and a proposed MVP**. They are deliberately separate. Current functionality uses fictional household and mortgage data. Cashback, bank connections, real payments, credit and retailer partnerships are **not live**.

## 2. The customer problem

Mortgage services are often organised around isolated events: applying, completing, making a payment, taking additional borrowing or switching deals. In the months and years between those events, customers can find it hard to see their progress, understand their options or identify small, achievable actions.

Problems to test with research:
- It is difficult to picture how today's financial decisions might affect the end of a mortgage.
- Equity, rates, mortgage terms and early repayment charges can feel abstract or intimidating.
- Shopping rewards, savings and household bills are disconnected from mortgage goals.
- When a fixed deal ends, customers may need to work out when and how to act.
- Home goals such as moving or renovating can require several disconnected journeys.

**Opportunity:** Give homeowners a reason to return beyond mortgage renewal, while building customer understanding, agency and confidence. This may also create value for a participating bank or lender through deeper engagement, retention and relevant cross-product discovery; these business outcomes remain hypotheses.

## 3. Product vision

**Home Time helps people see where they are, imagine where they could be and understand practical steps towards getting there.**

Design principles:
1. **Make the future visible.** Prefer interactive timelines and comparisons over abstract figures.
2. **Be specific and human.** Show actual dates, transparent calculations and plain-English explanations.
3. **Connect everyday actions to meaningful goals.** Make rewards and savings measurable rather than decorative.
4. **Never mistake education for personalised financial advice.** Explain assumptions, trade-offs and relevant restrictions.
5. **Be inclusive by default.** Accessible contrast, readable typography, touch targets and reduced-motion options.
6. **Earn trust.** Clear permissions, honest limitations and no invented live partnerships.

## 4. Audience and sample persona

**Primary audience:** UK residential mortgage holders who want to understand their mortgage, make informed overpayment choices and plan their next steps.

**Secondary audiences:** Home movers, people approaching a deal renewal, first-time homeowners after completion, and customers exploring home improvements.

**Illustrative prototype household:** Sam and Priya, owners of a two-bedroom terrace in Stockport. Their sample mortgage balance is **£200,000**, estimated property value **£280,000**, and fixed deal is shown ending **31 March 2028**. These are invented demo figures, not real customer information.

## 5. The experience

### 5.1 My Home — understand today

**Job to be done:** “Help me see my mortgage position and what I should pay attention to next.”

- Mortgage balance, estimated property value and derived equity amount and percentage.
- Upcoming mortgage milestones such as a fixed-rate end date.
- Contextual entry points to Time Machine and future planning.

**Important:** The property valuation is an estimate, not a confirmed sale price. Live values would require approved sources and clear freshness indicators.

### 5.2 Home Time Machine — explore the future

**Job to be done:** “Show me what might happen if I paid a little extra.”

- Select an extra monthly payment, including £0.
- Move a year slider to compare projected mortgage balances.
- Show two distinct curves: baseline and scenario.
- Display estimated mortgage-free month and year, months brought forward and lifetime interest difference.
- Explain the calculation assumptions, including starting balance, rate, remaining term and how overpayments are applied.
- Save and revisit a scenario in the prototype session.

**Calculation rules for the demo:** Standard monthly amortisation using an illustrative £200,000 balance, 25 years remaining and a constant 4.5% annual interest rate. Monthly payments are held at the calculated contractual amount plus optional overpayment, so paying extra reduces the term. Monthly interest is calculated on the outstanding balance. Results exclude actual future rate changes, overpayment restrictions, early repayment charges, taxes and other fees.

**Acceptance criteria:**
- Changing extra payment or selected year updates both the graph and figures.
- £0 shows the baseline path with no meaningless “0 years sooner” claim.
- Values never display a negative balance.
- Saved scenarios can be revisited within the same session.
- Charts have accompanying textual equivalents and usable slider labels.

### 5.3 Home Time Earn — make rewards relevant

**Job to be done:** “Could spending I already do help me make progress towards my home?”

- Browse fictional illustrative reward examples, such as groceries, home essentials and gift vouchers.
- Collect sample rewards in a non-monetary demo wallet.
- Explore **recurring monthly** cashback and how it accumulates over one or five years.
- Connect an illustrative monthly reward amount to the Time Machine as a possible overpayment.

**Important design principle:** Small one-off rewards should not be exaggerated. Show the true scale of the effect and explain when repeated behaviour is more relevant.

**Future integration hypothesis:** Approved partner-funded cashback offers, voucher fulfilment and optional redirection into an eligible mortgage or savings account. This is not implemented.

### 5.4 Pay Off — understand how overpayments work

**Job to be done:** “What should I check before making an extra payment?”

- Educational guidance on early repayment charges, annual allowances and whether an overpayment reduces the term, monthly payment or both.
- Illustrative annual allowance and amount-remaining examples.
- One-off payment amount preview.
- Guardrail when a proposed amount exceeds the *example* allowance.
- Clear distinction between a calculation and a real payment.

**Future implementation:** Any real payment must take place through a secure, authorised lender or payment partner journey with confirmation, validation, fraud controls, receipts and appropriate disclosures.

**UK mortgage detail:** A 10% allowance is common in some products but is **not a universal rule**. The real product must use the customer's own mortgage contract and the lender's current rules.

### 5.5 My Future — goals and milestones

**Job to be done:** “Help me plan what comes next for my home.”

Goal paths:
- **Own it outright:** Open overpayment and mortgage-free-date exploration.
- **Find our next place:** Understand estimated equity and considerations for moving.
- **Make space for more:** Explore a renovation budget and funding considerations.
- **Get ready for the next deal:** See a fixed-rate end date and prepare for renewal.

The hackathon prototype includes an indicative home-project budget split by number of months. It is **not** an offer of credit, an APR quotation or an affordability assessment.

**Future roadmap:** A richer goal planner, saved timelines, reminders and context-aware guidance tied to real customer milestones.

### 5.6 Connected Home — future concept

With informed customer permission and appropriate contracts, possible integrations include:
- **Open Banking:** account and transaction data through an appropriately authorised provider.
- **Mortgage servicing:** balances, rates, payments and contractual limits via participating lender APIs.
- **Rewards:** retailer/affiliate networks for eligible offers and tracked cashback.
- **Home finance:** renovation-related budgeting or instalment finance offered by a suitably authorised partner, following applicable credit, affordability, disclosure and customer-protection requirements.

No bank, retailer, credit or payment integration has been authorised or launched by Home Time.

## 6. Current prototype vs proposed MVP

| Capability | Hackathon prototype | Proposed MVP |
|---|---|---|
| Home snapshot | Fictional balance, equity and milestone | Customer-entered data with validation, transparent source and update date |
| Time Machine | Interactive amortisation illustration, visual chart | Validated scenario engine; rate-change scenarios, downloadable comparisons |
| Earn | Fictional rewards wallet and recurring estimates | Rewards discovery only after partners, fulfilment and economics are confirmed |
| Pay Off | Educational checks and preview | Lender-specific allowances and secure hand-off when integrated |
| My Future | Goal selection and project-budget illustration | Distinct goal flows, persistent saved plans and reminders |
| Data persistence | Session only | User account/consent and secure storage, if justified |
| Financial connections | None | Feasibility pilot with authorised partners; not a day-one requirement |

**Recommended MVP boundary:** Start with **My Home + Time Machine + My Future mortgage renewal planning** using transparent manually entered data. Validate whether this solves a real problem before adding money movement, partner rewards or credit.

## 7. Priority user journeys

**Journey A — see what £100 extra could do**  
Home → Time Machine → adjust monthly payment → compare outcomes and mortgage-free date → save scenario → revisit in My Future.

**Journey B — turn rewards into a habit**  
Earn → explore illustrative retailer categories → choose a monthly cashback assumption → see one-/five-year total → model that amount in Time Machine.

**Journey C — prepare for a fixed-rate end**  
Home milestone → My Future renewal goal → see target date → understand timing and next steps → optionally receive a future reminder (roadmap only).

**Journey D — explore a renovation**  
My Future → improvement goal → enter project budget → choose a duration for a *simple budget illustration* → compare saving versus possible borrowing options (future discovery only).

## 8. Functional requirements

**P0 — essential for a credible prototype / test**
- FR-01: All five navigation destinations remain accessible on mobile.
- FR-02: Key figures and controls respond without page reloads.
- FR-03: Mathematical results are derived from stated assumptions, not hardcoded claims.
- FR-04: Equity percentage is calculated from property value and loan balance.
- FR-05: Form inputs validate negatives, invalid values and bounds.
- FR-06: Zero overpayment produces sensible unchanged outcomes.
- FR-07: Financial examples and non-live features are transparently identified.
- FR-08: Navigation does not hide headings or controls on mobile.
- FR-09: Information is readable with sufficient contrast and clear focus states.

**P1 — MVP discovery**
- FR-10: Edit base mortgage assumptions rather than using only a fixed demo case.
- FR-11: Compare scenarios when the interest rate changes.
- FR-12: Save and restore named scenarios reliably.
- FR-13: Show event-based mortgage milestones and reminders.
- FR-14: Distinguish cashback earned, confirmed and redeemed.

**P2 — future integrations**
- FR-15: Permission-based connection to authorised financial-data services.
- FR-16: Lender-specific overpayment allowances and payment handoff.
- FR-17: Real retailer offers, eligibility and audited reward balances.
- FR-18: Optional, appropriately regulated home-improvement finance offers.

## 9. UX, accessibility and content requirements

- Mobile-first responsive layouts with consistently sized touch targets.
- Aim for **WCAG 2.2 AA** on any production experience; audit rather than assume compliance.
- Screen-reader names for icons, tab controls, charts and sliders.
- Support text enlargement, visible keyboard focus and reduced motion.
- Do not rely on pink/green or any colour alone to indicate meaning.
- Use sentence case and calm typography; avoid repetitive all-caps labels, interchangeable cards and decorative arrows.
- Use dates, amounts and concrete explanations rather than generic slogans.
- Keep warnings discoverable at decision points without repeatedly obscuring primary tasks.

## 10. Safety, compliance and data

- This is a planning and education concept, **not regulated mortgage advice**.
- No personalised “best mortgage”, suitability recommendation or claim that an option is cheapest unless authorised, evidenced and compliant.
- Financial outputs must show assumptions and limitations, including the possibility of charges.
- Any real mortgage, personal or transaction data requires an approved data-governance model, user consent where applicable, lawful basis, encryption, minimisation and deletion controls.
- Real cashback, Open Banking, mortgage servicing, payment initiation and credit must be reviewed with appropriate legal, risk, security and regulated partners before launch.
- Conduct threat modelling, privacy impact assessment and accessibility testing as part of production readiness.

## 11. Business hypotheses and success metrics

These are hypotheses to validate; no performance or revenue figures are asserted.

**Customer outcomes**
- Comprehension: % correctly explaining baseline vs scenario and key assumptions.
- Confidence: pre/post user-reported confidence in understanding choices.
- Task success: % completing a scenario without assistance.
- Ongoing value: % returning to a saved goal or milestone.
- Safety: % recognising that figures are illustrative and not advice.

**Business outcomes**
- Retention/engagement: appropriately defined active engagement outside renewal windows.
- Timely renewal engagement and reduction in missed relevant milestones.
- Reward-to-goal conversion, if an eligible rewards model is implemented.
- Cost-to-serve and contact reduction only where supported by measured evidence.
- Partnership unit economics, net of reward funding, acquisition and servicing cost.

## 12. Research plan

**Initial usability testing:** 6–10 homeowners with varied mortgage experience and accessibility needs; qualitative, not statistically representative.

Test prompts:
1. “Without an introduction, what do you think Home Time does?”
2. “Find what an extra £100 per month might change.”
3. “Explain what the chart and mortgage-free date mean.”
4. “Explore rewards. Would the result actually be worth doing?”
5. “Find when your deal ends and what you would do next.”
6. “What would you trust, question or expect to be connected to your bank?”

Capture misconceptions, navigation issues, perceived value, trust, motivations, accessibility friction and priority features. Follow with quantitative validation before business case claims.

## 13. Delivery approach

**Phase 0 — Hackathon:** Interactive HTML prototype, fictional data, demo use cases, stakeholder/customer feedback.

**Phase 1 — Research and refinement:** Validate Time Machine usefulness, customer comprehension, financial calculations, accessibility and prioritisation.

**Phase 2 — Limited MVP:** Build dependable scenario planning, goal persistence and milestone support with user-supplied data.

**Phase 3 — Partnership discovery:** Explore lender APIs, authorised Open Banking providers, rewards economics and compliance conditions.

**Phase 4 — Conditional expansion:** Only pursue payments, funded cashback or regulated credit after evidence, partner approvals and appropriate controls.

## 14. Dependencies and open questions

- Who is the initial target: direct consumers, a bank's existing mortgage customers or both?
- Which lender/product data can be legally and technically accessed?
- Can we show customer-specific overpayment limits accurately?
- Can cashback meaningfully move mortgage outcomes after all fees and costs?
- How will partner-funded rewards be attributed, reversed and transferred?
- What regulatory permissions are needed for each model?
- Should Time Machine prioritise term reduction, monthly payment reduction or choice between both?
- What does retention value look like *without* pushing unnecessary borrowing?
- What privacy/consent model would users trust?

## 15. Hackathon demo script

1. Start at **My Home**: “Here is the household's current position and next mortgage milestone.”
2. Open **Time Machine**: “What if they paid £100 more each month? Watch the two balance curves separate and the end date change.”
3. Open **Earn**: “Could a repeatable cashback habit contribute toward that extra monthly amount? These are illustrative offers, not live deals.”
4. Open **Pay Off**: “Before acting, check allowances and possible early repayment charges.”
5. Open **My Future**: “Now connect the mortgage to meaningful life goals: moving, renovating and getting ready for renewal.”
6. Close with the vision: “A product customers return to between mortgage transactions — one that can help them understand, plan and act.”

---

**Ownership and disclaimer:** Independently created hackathon concept. This PRD is a proposal for discussion and product exploration, not an approved delivery commitment, investment offer or claim of a banking partnership.
