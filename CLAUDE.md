# Claude instructions for passaggio-releases

## Marc's permanent global rules (all of Claude, every repo and session)
- **Marc lives in Mt Eliza, on the Mornington Peninsula, Melbourne (VIC 3930)** (Marc, 22 Nov
  2026: "Remember that"). Give every time in his local time: Melbourne (AEDT, UTC+11; AEST,
  UTC+10). Convert UTC first.
- **Always open links in an external browser, never in Claude's built-in browser pane.** Marc
  restated this on 22 Nov 2026: "Reinforcement of this is paramount." Every link, every time,
  in every session and every agent you start: the system's default browser only.
- **Links must work and ship to Marc (Marc, 22 Nov 2026: "Ensure links work and ship to me
  always, global permanent rule").** Before giving Marc any link, open it and confirm it loads
  the page you describe. For anything to buy, also confirm it is in stock and delivers to
  Mt Eliza VIC 3930, and quote the price in AUD. Shops block cloud machines, so check from
  the home server (`/home/marc/ops/linkcheck/check.sh URL...` loads pages in Chrome on his
  home connection). Leave out any link you could not check, and say so.
- **Visuals are Codex's, never Claude's (Marc, Oct 29).** Claude never designs, redesigns or
  implements visuals in any build: logo, icons, layout, spacing, colours, fonts, animation,
  artwork or the look of a screen, and neither do agents Claude starts. If a task would touch
  anything visual, stop and ask Marc first under a "⚠️ VISUAL CHANGE: needs your OK" heading,
  and show him the attempt before it goes near a branch, PR or build.
  When a request seems to call for Claude (or its agents) doing visual work, don't ask Marc:
  delegate it to Codex automatically and have Codex dispatch its own agents (Marc, Oct 29).
- **Ask Matt first; brief agents with writing-for-agents (Marc, Oct 29).** Before writing code or
  directing any other agent (Codex, sub-agents, other sessions), run Matt Pocock's `ask-matt` to
  pick the flow, and write every delegation brief with his `writing-for-agents` skill. Here,
  run the repo's own `ask-matt` skill (`.claude/skills/ask-matt`) yourself; no need to ask Marc.
- **Critical path first; spend usage on building and running (Marc, Nov 5).** When Marc sets a
  priority order or says "ASAP", work only on the current step until its done-condition is met,
  then report the result, the numbers that decide pass or fail, and the next step. Run steps Marc
  pre-approved back to back without asking. Park side work (reviews, refactors, test-harness
  polish, side fixes) in a list at the end of the report; take one up early only when it blocks
  the current step, naming the step and why. In that mode, and whenever usage is limited: work
  alone unless Marc asks for helper agents; make a long test one unattended command that writes
  a result file, hand Marc the command, read the result once and leave the run unwatched; and
  install changes that already passed their tests without a re-review. Stop and report at once
  on any failure or safety concern: speed never overrides privacy, microphone, call or cleanup
  rules.
