# AI Resume Reviewer (Team Pioneers, PE-B49-47)

SCSE4041 Prompt Engineering – Mini Project, Milestone 2

## What it does
A shared Gemini Gem that compares a resume with a job description and returns a match score out of 100 (fixed rubric), matching and missing skills, rewritten bullet points that never invent facts, and tips.

## Prototype (open and try)
https://gemini.google.com/gem/1x_poArLSXmTtevzxS66_U2mGqBoJMAH7?usp=sharing

How to use: open the link, start a new chat, and paste:
RESUME:
(resume text)

JOB DESCRIPTION:
(job description text)
Use made-up or anonymised data only.

## Team
| Name | Enrollment no. |
|---|---|
| Vansh Gupta (leader) | S24CSEU0144 |
| Peeyush Tomar | S24CSEU0202 |
| Varun Panwar | S24CSEU1735 |

Faculty: Ankit Vijay Bansal | Batch: B49-64 | Problem source: Problem Pool, ID C9

## Repository structure
- prompts/v1, prompts/v2: older prompt versions
- prompts/final: the final prompt used in the Gem
- test-data: the 12 test inputs and saved screenshots
- docs: Milestone 2 PDF and Technical Report
- CHANGELOG.md: dated changes since Milestone 1

## Notes
No API keys or passwords are stored in this repository. If the Gem link stops working (Google is migrating Gems to skills), the full prompt is in prompts/final/.
