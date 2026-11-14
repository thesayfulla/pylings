# PyLings 🐍

Python interview practice, like [rustlings](https://github.com/rust-lang/rustlings): from easy to hard. 

Python 3.14 with no dependencies.

## Start

With [uv](https://docs.astral.sh/uv/getting-started/installation/) (it fetches Python 3.14 for you if you don't have it):

```bash
uv run pylings
```

No uv? Any Python 3.14 works: `python3 -m pylings`

It opens the next exercise and re-runs its tests every time you save.

## Keys: 
- `n` next
- `h` hint
- `r` re-run
- `l` list
- `c` check all
- `x` reset
- `s` solution
- `q` quit

## Exercises

| Level | Folder | What's inside |
|-------|--------|---------------|
| Warm-up | `exercises/0_warmups/` | 35 short "fix this" tasks: strings, collections, functions, classes, iterators, decorators, asyncio… |
| Middle | `exercises/1_middle/` | 01–06: iterator utils, LRU cache, retry decorator, bug hunt, KV transactions, log report |
| Middle+ | `exercises/2_middle_plus/` | 07–10: Money, rate limiter, event bus, task graph |
| Senior | `exercises/3_senior/` | 11–17: contextmanager, single-flight cache, circuit breaker, external sort, async map, worker pool, bug hunt |
| Staff | `exercises/4_staff/` | 18–20: generator event loop, mini pydantic, DI container |

Solutions are in `solutions/` (same layout). Interview questions are in `questions/middle.md` and `questions/senior.md`.

## Tips

1. Don't open `solutions/` until the tests pass.
2. Name the edge cases before you write code.
3. When the tests pass, answer the **Discussion** questions at the end of the exercise. That's what interviewers ask.

## Without pylings

```bash
uv run -m unittest discover -s tests -p "test_ex05*" -v
```

Check the reference solutions:

```bash
SOLUTIONS=1 uv run -m unittest discover -s tests
```
