# Eden

**Pwn · 500 points**

A walled garden for small colonies. Plant one, step it forward, watch the
viewport. A colony that survives long enough earns the right to be
transplanted, dropped in at coordinates of your choosing. The garden grants
that privilege a little too freely.

### Where it is

**The brief and a live viewport:**

    http://bin.syriactf.com

**The service itself, which is what you attack:**

```
nc bin.syriactf.com 5000
```

### What you are working against

- x86-64
- A bounded grid, 64 × 32, running Conway's Life under B3/S23
- Patterns go in as **RLE**: `b` dead, `o` alive, `$` end of row, `!` end of
  pattern, each optionally prefixed with a count

### Sessions, and how to not waste them

**A session lasts about fifteen minutes.** That is not much when you are
iterating.

Run it locally in Docker instead: work out your approach against your own copy
with no clock on it, and come back to the live host only when you have
something ready to fire.

### AI

**This is the one challenge where AI is fully allowed.** Use whatever you like,
as much as you like. Everywhere else it is out.
