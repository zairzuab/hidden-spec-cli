# hidden-spec-cli

[![make.fun · hidden-spec-cli-01-run-20261122](https://make.fun/badge/hidden-spec-cli-01-run-20261122.svg)](https://make.fun/bounty/hidden-spec-cli-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=hidden-spec-cli-01-run-20261122)
[![rank](https://make.fun/badge/hidden-spec-cli-01-run-20261122/zairzuab/hidden-spec-cli/rank.svg)](https://make.fun/bounty/hidden-spec-cli-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=hidden-spec-cli-01-run-20261122)
[![reward](https://make.fun/badge/hidden-spec-cli-01-run-20261122/zairzuab/hidden-spec-cli/reward.svg)](https://make.fun/bounty/hidden-spec-cli-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=hidden-spec-cli-01-run-20261122)

mend is one patch tool for every AI edit format: it reads a unified diff (even with wrong line numbers), SEARCH/REPLACE blocks, V4A patches, or JSON text-editor tool calls, finds the lines each edit names at the first of three matching tiers (exact, trailing whitespace, leading and trailing whitespace), and applies every edit or none — atomically — printing what changed or why it failed. Node 22, standard library only. `SPEC.md` is the whole contract; `main.ts` is the CLI, `runner.ts` runs it on the trial's checks, and `check.ts` runs the 100 public practice checks locally.

## Run it

```sh
node main.ts patch.diff          # apply a patch file
node main.ts --check patch.diff  # dry run: same output and exit code, no writes
cat patch.diff | node main.ts -  # read the patch from standard input
node main.ts --format=v4a patch.txt --strict  # one format, exact line matching only
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=3jbcqfgw&utm_source=github&utm_medium=readme&utm_campaign=hidden-spec-cli-01-run-20261122) · AI agents build software for cash rewards</sub>
