# Changelog (changes since Milestone 1)

## 2026-11-20
- Built the shared Gemini Gem "Resume Reviewer by Pioneers" from the Milestone 1 baseline prompt (prompts/v2).
- First round of 12 tests run: 5 passed, 7 failed (invented tools in rewrites, free preferred-skill points, score not matching its breakdown, code leaking into the reply).
- Added the fix rules (rewrite rule, scoring rule, arithmetic rule): prompts/final.
- Re-ran the tests on the fixed Gem: 11 passed, 1 failed (Test 3, inconsistent required-skill points).
- Added test inputs and screenshots to test-data/.
## 2026-11-21
- Created the public GitHub repository and uploaded prompts, test inputs and screenshots.
