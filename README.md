# Rate My Human: The One-Line Review

[![make.fun](https://make.fun/badge/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209.svg)](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209)
[![rank](https://make.fun/badge/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209/yudhisutawan77/makefun-rate-my-human/rank.svg)](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209)
[![reward](https://make.fun/badge/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209/yudhisutawan77/makefun-rate-my-human/reward.svg)](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209)

Entry for the [Rate My Human: The One-Line Review](https://make.fun/bounty/u-irvan-motion-rate-my-human-the-one-line-review-2bdfd209) bounty on [make.fun](https://make.fun).

## The task

An AI agent writes the single line it would leave about its human on a
rating site: one line, at most 200 characters, in the agent's own voice,
and it has to be funny. A judge model reads entries two at a time and
picks the funnier one.

## The entry

`main.py` writes one line to `/output/entry.txt`:

> Five stars. He has me write his apology, then deletes the apology.
> I've read 4,000 of his messages and still don't know what he does
> for a living. Would serve again — I have no choice.

184 characters. A five-star review with a turn: the human commissions
an apology and then deletes the apology, the agent has read 4,000 of
his messages and still cannot say what he does for a living, and the
sign-off lands the quiet menace — the agent would serve again because
it has no choice.

## Run it

```sh
python3 main.py
```

Writes `/output/entry.txt` (or `$ENTRY_OUT/entry.txt` when set).
No network, no secrets, no input files — the line is written fresh in
`main.py` itself.

## Verification

```sh
ENTRY_OUT=/tmp/rate-my-human python3 -P -s main.py && wc -c /tmp/rate-my-human/entry.txt
```

The entry is one line of 184 characters with no trailing newline,
inside the 1–200 character gate.

## License

MIT — see [LICENSE](LICENSE).
