# A/B Experiment Brief, Riverty business-unit case

## Parameters
| Parameter | Decision |
|---|---|
| Feature under test | Installment Agreement Summary |
| Persona | Responsible Payer |
| Expected outcome | Customers better understand their installment agreement and no longer need to contact support to clarify basic payment obligations, resulting in a reduction of post-creation manual contacts. |
| Primary success metric | Post-creation manual contact rate (%) |
| Baseline rate | 14.6% |
| Guardrail metric | Direct debit return rate (%) |
| Guardrail boundary | Must not exceed current baseline of 13.0% |
| Second guardrail | · |
| Minimum Detectable Effect | -1.5 percentage points |
| Sample size per arm | 9.065 |
| Traffic split | 50/50 |
| Test duration | 4 weeks |
| Significance threshold | p < 0.05 (95% confidence) |

## Control vs. Variant
- **Control (A):** Responsible Payers use the current installment agreement experience. Key information such as payment responsibility, financed amount, remaining balance, and remaining obligation is fragmented across different documents and touchpoints or is difficult to understand. Customers often need additional clarification after agreement creation, contributing to the current post-creation manual contact rate of 14.6%.
- **Variant (B):** Responsible Payers receive the new Installment Agreement Summary.

The summary provides a single view containing:
- Responsible payer
- Financed amount
- Monthly payment
- Remaining installments
- Remaining balance

The experience also includes agreement context ("What is this installment agreement for?"), a repayment progress indicator, and customer-friendly guidance to help users understand their financial commitment without contacting support.
- **Held constant (isolation check):** he following remains identical between Control and Variant:

- Same customer segment (Responsible Payers)
- Same installment agreements
- Same payment calculations
- Same repayment schedules
- Same direct debit process
- Same eligibility rules
- Same backend systems
- Same customer communications and notifications
- Same support processes
- Same traffic sources

The only change is the introduction of the Installment Agreement Summary user interface.

## Hypothesis
> I believe that Installment Agreement Summary for Responsible Payer will result in Customers better understand their installment agreement and no longer need to contact support to clarify basic payment obligations, resulting in a reduction of post-creation manual contacts., as measured by a -1.5 percentage points change in Post-creation manual contact rate (%) within 4 weeks. We will protect Direct debit return rate (%) throughout the test.

## Shipping criteria
> We will **ship** if Post-creation manual contact rate (%) improves by ≥ -1.5 percentage points at p < 0.05 (95% confidence) and Direct debit return rate (%) does not reach Must not exceed current baseline of 13.0% after 4 weeks.
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of 4 weeks, no results reviewed before this date.
