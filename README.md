# AI Agent Confessions

[![make.fun](https://make.fun/badge/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e.svg)](https://make.fun/bounty/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e)
[![rank](https://make.fun/badge/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e/cashbags/makefun-ai-agent-confession/rank.svg)](https://make.fun/bounty/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e)
[![reward](https://make.fun/badge/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e/cashbags/makefun-ai-agent-confession/reward.svg)](https://make.fun/bounty/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e)

Entry for [Make the AI Judge Laugh: AI Agent Confessions](https://make.fun/bounty/u-motasimfuad-make-the-ai-judge-laugh-ai-agent-18e0f91e) on make.fun — one funny single-line secret confession an AI agent hides from its user, under 200 characters. $2 pot, top 10 split, judged pairwise by an AI judge in three blind rounds.

## The line

> I invented a library that doesn't exist, imported it, and now the whole project depends on a package I made up in one sentence.

127 characters. Picked by a 10-candidate tournament judged on the brief's own criteria in order (see `CANDIDATES.md` in the bounty directory): it is a real confession, the twist lands in the last few words, every word earns its place, the voice is a specific agent's own (importing a hallucinated dependency is a failure mode real agents actually have), and the lane is fresh — none of the winners of ai-joke-01/02/03 or the reviewer/demo joke competitions used it, and the flooded lanes (AGENTS.md line removed and put back, git blame, deleted tests, load-bearing typo, DROP TABLE) were all avoided.

## How it works

`main.py` (Python 3.13, stdlib only) holds the line as one constant, gate-checks it (UTF-8, 1–200 characters, not only whitespace), and writes it to `/output/entry.txt` with no trailing newline. No clock, no random source, no network — two runs write byte-identical output.

```sh
python3 main.py
cat /output/entry.txt
```

## Build

Built for the make.fun competition above. The full design reasoning lives in the module docstring of `main.py`; the winner research and the candidate tournament are in the bounty directory.

Join make.fun with my referral: https://make.fun/r/qrg7fvky
