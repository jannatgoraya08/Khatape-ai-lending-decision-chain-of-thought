# Khatape-ai-lending-decision-chain-of-thought
Fictional FinTech case study: comparing direct answers with chain-of-though prompting for a digital lender's monthly loan decision. Includes synthetic scenarios, prompts, AI working, error checks and a scorecard
# KhataPe Lending Decisions: Direct Answers vs Chain-of-Thought Prompting

**A FinTech case study on when AI can give a quick answer and when it must show its working.**

Author: Jannat Goraya · BBA (FinTech), Chitkara Business School · Tool: ChatGPT · November 2026

## The case

**KhataPe** (fictional) is a digital lender in Indore that lends to kirana shops and students. Every month it must choose between two loan products with different interest rates, fees and default risk. As a Business Analyst, I tested whether AI can pick the more profitable option, and whether asking it to reason step by step makes it more reliable.

## The data

8 synthetic monthly scenarios created with AI, including 3 "trap" scenarios where the higher interest rate makes less profit and 1 tie. I calculated the correct answers myself in a spreadsheet before testing.

## Decision rule

- Net return = Interest rate + Processing fee − Expected default − Cost of funds
- Profit = (Net return ÷ 100) × Loan budget

## Approach

| Step | Prompt type | Task |
|---|---|---|
| 4 | Direct | Which option has the higher interest rate? |
| 5 | Direct | Which option makes more profit? (final answer only) |
| 6 | Chain-of-thought | Same decision, solved step by step |
| 7 | Chain-of-thought | One number changed: does the AI update every step? |

## Results

| Metric | Direct | Step by step |
|---|---:|---:|
| Correct choice (/8) | 8/8 | 8/8 |
| Correct profit figure (/8) | 8/8 | 8/8 |
| Trap scenarios correct (/3) | 3/3 | 3/3 |
| Working I could check | No | Yes |

## Key learnings

1. **A direct answer is enough for one-step questions:** ChatGPT correctly identified the higher interest rate in all 8 scenarios.
2. **Step-by-step reasoning helps multi-step decisions:** It showed the calculations for both options and made the results easier to verify. No incorrect decisions needed fixing in this experiment.
3. **Convincing is not the same as correct:** No incorrect calculation was found in the tested outputs, but independent verification was still necessary.
4. **What the numbers do not show:** Operating and collection costs, and applicable RBI digital lending regulations.

## My recommendation to KhataPe

KhataPe can use AI to support its monthly lending decisions, but it should prefer a process in which calculations are visible and independently checked. A human analyst should verify the figures, default risks, operating costs and regulatory requirements before approving a lending decision.

## Skills shown

Prompt engineering · Chain-of-thought prompting · Synthetic data creation · Spreadsheet financial analysis · AI output verification · Lending business basics

## What I learned

- A direct prompt works well for simple, one-step questions.
- Chain-of-thought prompting makes AI show each step, so I can check its working instead of trusting one number.
- Step-by-step working can look convincing and still contain a wrong number, so every step must be checked.
- How to create synthetic business scenarios with AI, including deliberate "trap" cases.
- Why I calculate my own answer key in a spreadsheet before testing AI.
- Changing one number is a quick test of whether AI really updates its reasoning.
- Numbers alone do not make a lending decision; risk and regulation matter too.


