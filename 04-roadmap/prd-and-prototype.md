# PRD & Prototype Sprint (Module 4)

## Pick & scope with MoSCoW
- **The “Now” feature I’m scoping (name + one-line core description):** Installment Agreement Summary: Gives customers one clear view of who pays, what is financed, monthly payment, duration, and remaining balance.
- **My finalized Must-Haves (after overriding the AI):** After reviewing the AI output, I reduced the Must-Have scope to the minimum set required to solve the Responsible Payer's core problem.

Display payer information – clearly identify who is financially responsible for the agreement.
Display financed amount – show the exact amount covered by the installment agreement.
Display monthly payment – provide clear visibility into the current payment obligation.
Display agreement duration / remaining installments – show how long the commitment will continue.
Display remaining balance – show the outstanding amount still to be repaid.

I moved items such as payment date details, agreement change history, payment progress indicators, document access, and contextual explanations into Should-Have because the persona can still achieve the primary goal without them in the first release.
- **What I demoted from Must → Should/Won’t, and why:** I demoted several items from Must-Have because they support convenience rather than solve the core customer problem. I moved Next Payment Date, Payment Progress Indicator, Agreement Change History, Document Access, and Contextual Explanations from Must to Should. While these features improve the overall experience, the Responsible Payer can still achieve the primary goal without them.

I also kept servicing functions such as installment changes, payment deferrals, bank account updates, returned direct debit resolution, and status tracking out of scope for the first release. These capabilities are valuable but do not directly solve the core Moment of Misery: understanding who pays, what is financed, how much is owed each month, how long the agreement runs, and what balance remains outstanding.

The resulting Must-Have scope focuses exclusively on five questions: Who pays? What is financed? What is my monthly payment? How long does the agreement run? What do I still owe?

## Generate your Simplified PRD
- **One thing my PRD makes explicit that a vague brief would have missed:** One thing my PRD makes explicit that a vague brief would have missed is the distinction between understanding an installment agreement and servicing an installment agreement. The PRD clearly limits scope to helping the Responsible Payer understand five key facts (who pays, what is financed, monthly payment, remaining installments, and remaining balance) and explicitly excludes actions such as changing installments, updating bank details, or resolving payment issues. This prevents the project from expanding into a broader self-service portal before validating the core transparency hypothesis.

## Prompt-to-prototype sprint
- **Where did the prototype reveal a gap in my PRD logic? (what I had to update):** The prototype revealed that showing the core agreement details alone was not sufficient to solve the customer’s moment of misery. While the original PRD focused on who pays, what is financed, monthly payment, remaining installments, and remaining balance, the prototype made it clear that customers also need contextual information about what the agreement actually relates to. As a result, I extended the design with the “What is this installment agreement for?” section, including invoice reference, healthcare provider, and service description.

The prototype also highlighted the need for repayment progress and contextual guidance (“Good to Know”) to help users understand their obligation over time. These additions improved clarity without expanding into servicing functionality, keeping the solution aligned with the original transparency-focused scope
- **My prototype, as a link or a screenshot (publish or share from your tool; in Lovable that is Share → Share Preview, in Bolt Publish → Web. No share URL? Screenshot the working flow):** see word document: promt to prototype sprint
