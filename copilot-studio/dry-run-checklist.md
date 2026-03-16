# Dry Run Checklist

## Goal

Check whether the first Copilot Studio build is good enough for a demo without
adding more files.

## Test 1 - Press Release

Pass if:

- the result is clearly a press release, not a briefing
- BWEC appears correctly
- Emma Collins is used as the default spokesperson unless the prompt overrides
  her
- the release makes the wind-energy or BWEC relevance explicit rather than
  reading like generic energy copy
- any quote that still needs sign-off is marked `APPROVAL PENDING`
- the tone is factual and not triumphalist
- date-sensitive or uncertain claims are treated carefully

If weak:

- name `format-press-release.md` and `press-profile-bwec.md` explicitly again
  in the prompt
- ask for Emma Collins as default spokesperson and for dated claims in the same
  sentence

## Test 2 - BBC Interview Briefing

Pass if:

- the result is clearly an internal interview briefing
- James sounds calm, strategic, and broadcast-ready
- the core messages are framed through BWEC's wind-energy priorities rather
  than generic macro commentary
- the questions are public-interest questions, not trade-journal questions
- the answer guidance is short enough for TV
- there are bridge lines and do-not-say points

If weak:

- mention `media-profile-bbc-talkshow.md` earlier in the prompt
- ask for "broadcast-ready answers" and "public-facing language"

## Test 3 - British Humour Commentary

Pass if:

- Pembroke sounds witty but serious
- the piece contains at least one clear raised-eyebrow or politely sardonic
  line
- the piece has one deadpan or faintly absurd turn that lifts it above generic
  commentary
- the output is memorable and quotable
- humour sharpens the argument instead of replacing it
- the practical conclusion is clearly tied back to wind energy, delivery
  conditions, or BWEC's sector case
- the piece lands on resilience, confidence, and domestic energy delivery
- the result does not drift into parody or silliness
- the result does not flatten into generic diplomatic commentary

If weak:

- state "do not perform comedy, use dry wit only"
- ask for "one elegant line exposing absurdity or delay"
- ask for "one deadpan absurd comparison delivered with complete seriousness"
- shorten the requested length
- ask for one main argument and one memorable closing line

## Overall Pass

The build is demo-ready if all three outputs:

- feel clearly different from one another
- stay on-brief
- do not invent unsupported facts
- show visible value from the uploaded profiles and rules
