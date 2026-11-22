# AI Resume Reviewer

**Team Pioneers (PE-B49-47)** | SCSE4041 Prompt Engineering, Mini Project, Milestone 2

## What this project does
When you apply for an internship, it is hard to know which skills the job wants and what your resume is missing. Our tool is a shared Gemini Gem. You paste a resume and a job description, and it gives you:
- a match score out of 100, with the reasons for each part of the score
- the skills that match and the ones that are missing
- better versions of your bullet points, using only facts you already wrote
- up to three tips

## Try it
Prototype (Gemini Gem): https://gemini.google.com/gem/1x_poArLSXmTtevzxS66_U2mGqBoJMAH7?usp=sharing

Reel (109 seconds): https://www.youtube.com/watch?v=U-Dy9-W0rBs

How to use the Gem:
1. Open the link and start a new chat.
2. Paste your text in this format:

```
RESUME:
(resume text)

JOB DESCRIPTION:
(job description text)
```

3. Read the reply. Please use made-up or anonymised data only.

## How it works
There is no code. The Gem has one long instruction (one prompt) that makes Gemini work in three steps: check and read the input, score it with a fixed rubric (required skills 60, preferred skills 20, relevance 20), and rewrite the bullet points. If the job lists no preferred skills, the score is worked out of 80 and scaled to 100.

## Results so far
- 12 tests: 4 normal, 5 edge, 3 invalid
- First Gem version (v2): 5 passed, 7 failed
- Final version (v3): 11 passed, 1 failed (Test 3, because its score changes between runs)

## Repository structure
| Folder or file | What is inside |
|---|---|
| prompts/v1 | Baseline prompt from Milestone 1 |
| prompts/v2 | First Gem instructions |
| prompts/v3 | Second round with three extra rules (same as final) |
| prompts/final | The prompt used in the Gem now |
| test-data | The 12 test inputs and screenshots of real runs |
| docs | Milestone 2 PDF and Technical Report |
| code | Empty on purpose, because the project has no code |
| CHANGELOG.md | Dated list of what changed since Milestone 1 |

## Team
| Name | Enrollment no. | Main task |
|---|---|---|
| Vansh Gupta (leader) | S24CSEU0144 | Prompt design, testing, repository |
| Peeyush Tomar | S24CSEU0202 | Proofreading and link checks |
| Varun Panwar | S24CSEU1735 | Reel |

Faculty: Ankit Vijay Bansal | Batch: B49-64 | Problem source: Problem Pool, ID C9

## Notes
- No API keys or passwords are stored in this repository.
- Google is moving Gems to "skills". If the Gem link stops working, the full prompt is in `prompts/final/`.
