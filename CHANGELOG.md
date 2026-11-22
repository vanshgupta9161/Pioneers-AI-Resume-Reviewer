# Changelog

Changes since Milestone 1, newest first.

## 2026-11-22
- Recorded the project reel (109 seconds) and uploaded it to YouTube as unlisted.
- Added the Milestone 2 PDF and the Technical Report to `docs/`.
- Updated the README with the reel link and a short summary of the results.
- Filled in and submitted the Milestone 2 form.

## 2026-11-21
- Added three rules to the Gem (rewrite rule, scoring rule, arithmetic rule). This is prompt version v3, saved in `prompts/v3/` and `prompts/final/`.
- Re-ran all 12 tests on v3: 11 passed, 1 failed. Test 4 (chef resume) dropped from 22 to 0 and Test 9 stopped contradicting its own score.
- Test 3 still fails because its score changes between runs (92, 100). We kept it in the table as a known limitation.
- Ran the Milestone 1 baseline prompt three times in a plain Gemini chat to get the v1 numbers (scores 45, 52 and 52).
- Saved screenshots of Tests 1, 6 and 12 and of the Gem instructions in `test-data/`.
- Created this public GitHub repository and uploaded the prompts, test inputs and screenshots.

## 2026-11-20
- Built the shared Gemini Gem "Resume Reviewer by Pioneers" from the Milestone 1 baseline prompt (saved as `prompts/v2/`).
- Ran the first round of 12 tests on v2: 5 passed, 7 failed. The problems were invented tools in rewrites, free preferred-skill points, a score that did not match its own breakdown, and code showing up in the reply.
- Checked that the Gem link opens from a different Google account.
