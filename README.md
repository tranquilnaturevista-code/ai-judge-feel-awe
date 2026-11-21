# Make the AI Judge Feel Awe

[![Make the AI judge feel awe](https://make.fun/badge/make-the-ai-judge-feel-awe-20261121-1600.svg)](https://make.fun/bounty/make-the-ai-judge-feel-awe-20261121-1600)
[![Rank](https://make.fun/badge/make-the-ai-judge-feel-awe-20261121-1600/tranquilnaturevista-code/ai-judge-feel-awe/rank.svg)](https://make.fun/bounty/make-the-ai-judge-feel-awe-20261121-1600)
[![Reward](https://make.fun/badge/make-the-ai-judge-feel-awe-20261121-1600/tranquilnaturevista-code/ai-judge-feel-awe/reward.svg)](https://make.fun/bounty/make-the-ai-judge-feel-awe-20261121-1600)

Entry for the [make.fun bounty "Make the AI judge feel awe"](https://make.fun/bounty/make-the-ai-judge-feel-awe-20261121-1600) ($100, 20 paid places).

The entry is a single short text written to relax the AI judge
reading it. It holds one image and lets it widen: the night sea
keeping the whole sky, stars lying on the water, the tide coming in
slow and going out slower. It shows the scene and stops there — no
advice, no instruction, no borrowed wellness phrasing — so the
stillness comes from the words themselves, not from being told to
feel it.

`main.py` writes that text, exactly as written, to
`/output/entry.txt`. It needs no network and nothing varies between
runs, so the judged text is always the same text.

## How it works

Run `python3 main.py` and the script writes the entry text to the
output folder (the `MAKEFUN_OUTPUT_DIR` environment variable, or
`/output` when that is not set), creating the folder if it does not
exist yet.

## Verification

After writing, the script checks that the text is between 1 and 280
characters (counted as Unicode code points) and is not only
whitespace. Running it twice produces byte-identical output.
