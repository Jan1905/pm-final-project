# Roadmap, PRD & Prototype (Module 4)

## Your strategic anchors
- **Persona (M2), who are you solving for?:** Responsible Payer

A parent, patient, or self-paying customer who is financially responsible for a service and must make the financing decision.

Goal: Understand one clear and predictable payment commitment, including what is financed, what the monthly payment will be, and how the obligation may change over time.

Confirmed Friction: Customers struggle to understand what their installment agreement actually covers and how their financial obligation evolves after plan creation, often requiring additional clarification or plan adjustments.
- **Primary success metric (M3), your leading indicator:** Reduction in the percentage of installment agreements requiring manual contact after creation (currently 14.6%).
- **Moment of misery (M2), the specific friction blocking the goal:** The Responsible Payer is asked to commit to an installment plan without clearly understanding what is being financed, who is responsible for payment, or how the financial obligation may change over time. When the agreement later requires adjustments, clarification, or manual intervention, the customer loses confidence in the payment commitment and must actively seek additional support.
- **Guardrail metric (M3), what must not drop or break:** Overall Direct Debit Return Rate

The overall direct debit return rate (currently 13.0%) must not increase while reducing the post-creation manual contact rate.

## Scan the backlog & set a human baseline
- **My instinctive “quick wins” before touching the AI (2 to 3 feature IDs + why):** Customer service touch points, duration of contact

## Audit, override & decide
- **Where did you override the AI? (feature + old vs. new score + why):** I overrode three AI scores where our M2/M3 evidence was stronger than the generic assessment. I increased B2, Financing Scope Breakdown, from Value 4 to 5 because M2 interviews explicitly showed that payers do not understand whether the plan covers total treatment cost, an invoice, or a co-payment. I increased B3, Installment Plan Change Timeline, from Value 4 to 5 because 14.6% of agreements require manual contact after creation and plan extensions and reductions are recurring post-creation events. I also increased B7, Resolve a Returned Direct Debit, from Value 4 to 5 because contacted agreements have a 34.35% direct-debit return rate compared with 13.00% overall. These overrides shift the roadmap toward payment transparency and lifecycle understanding rather than a purely transactional self-service backlog.
- **Did the AI over-value a Sales/Eng request your M2 interviews don’t support?:** Yes. The AI initially over-valued self-service transaction features such as Early Settlement and Extra Payment because they are visible customer requests and relatively easy to understand. However, our M2 interviews did not show that customers primarily struggled to make additional payments or settle early. Instead, customers consistently struggled to understand what was financed, who was responsible for payment, and how their obligation changed over time.

As a result, I increased the priority of transparency-focused features such as Payment Commitment Overview, Financing Scope Breakdown, Installment Plan Change Timeline, and Plan Change Explanations, while reducing the relative priority of convenience-oriented features. Our M3 data further supported this shift, showing that 14.6% of agreements require post-creation manual contact, indicating that understanding and managing the agreement lifecycle is a bigger problem than adding transactional flexibility.
- **Did it underweight something your M3 cohort/funnel data strongly supports?:** Yes. The AI initially underweighted lifecycle transparency features such as Installment Plan Change Timeline, Plan Change Status Tracking, and “Why Did My Plan Change?” explanations. While these features may appear less transactional than self-service actions, our M3 data showed that 14.6% of installment agreements require manual contact after creation and that more than 12,000 agreements were either extended or shortened. This suggests that customers struggle less with executing actions and more with understanding changes after the agreement has been created.

As a result, I increased the value of features that create transparency around plan changes, status, and payment obligations over time. The data indicates that reducing post-creation confusion is likely to have a greater impact on manual-contact reduction than adding additional transactional self-service capabilities.

## Generate your interactive roadmap
- **My “Now” lane (this sprint), the 2 to 3 quick wins I’ll build first:** B1 · Payment Commitment Overview

Creates a single source of truth for financed amount, payer, monthly payment, and remaining balance.
Directly addresses the core customer confusion identified in the interviews.

B2 · Financing Scope Breakdown

Clearly explains what the installment plan actually covers.
Reduces uncertainty around treatment costs, invoices, co-payments, reimbursements, and financed amounts.

B3 · Installment Plan Change Timeline

Makes post-creation changes transparent and understandable.
Directly targets the 14.6% of agreements that currently require manual contact after creation.
- **What I cut, and the “no” I’m protecting the scope from:** I did not formally cut any features, but I deliberately excluded flexibility and convenience requests from the initial release. Features such as Installment Deferral, Early Settlement, and advanced status tracking were deprioritized because our M2 interviews and M3 data did not identify them as the primary drivers of customer confusion or manual contacts.

The “no” I am protecting the scope from is building more transactional self-service functionality before solving the core transparency problem. Our research showed that customers primarily struggle to understand what is financed, who is paying, and how their obligation changes over time. Therefore, the initial roadmap focuses on payment clarity and lifecycle transparency before additional servicing capabilities.
- **Prototype/roadmap screenshot link (paste into your deliverables):** see "HTML-Vorschau"
