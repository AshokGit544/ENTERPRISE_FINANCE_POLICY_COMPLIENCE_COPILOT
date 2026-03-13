# Enterprise Finance Policy Compliance Copilot

This project checks finance transactions against policy rules.

It uses finance data like:
- vendors
- cost centers
- profit centers
- GL accounts
- approval details
- invoice details

The goal is to find records that break the rules and show why they were flagged.

## What this project does

- creates finance sample data
- creates policy rules
- checks each transaction against those rules
- finds non-compliant records
- matches records to the closest policy
- gives a simple explanation for each flagged case
- creates output files for review

## Examples of checks

This project checks things like:

- high consulting spend without proper approval
- emergency repair spend without higher approval
- non-preferred vendor transactions without justification
- late invoice submission
- weekend posting review
- high-risk vendor transactions needing controls review

## Main outputs

After running the notebook, it creates files like:

- `vendors.csv`
- `cost_centers.csv`
- `profit_centers.csv`
- `gl_accounts.csv`
- `policy_library.csv`
- `finance_transactions.csv`
- `top_non_compliant_cases.csv`
- `compliance_summary.csv`
- `violation_type_summary.csv`
- `policy_hit_summary.csv`
- `compliance_cases.csv`

## What can be checked

This project can answer questions like:

- Which transactions broke the rules?
- Which vendors need more review?
- Which records are missing approval?
- Which policy is most relevant for a flagged case?
- What are the top compliance issues?

## Tools used

- Python
- pandas
- NumPy
- matplotlib
- scikit-learn
- Google Colab / Jupyter Notebook

## What this project shows

- finance data handling
- policy rule checking
- compliance reporting
- search across policy text
- simple case explanation

## How to run

1. Open the notebook in Google Colab
2. Install the required libraries
3. Run all cells
4. Check the output files
5. Upload the notebook and outputs to GitHub
