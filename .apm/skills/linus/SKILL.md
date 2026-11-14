---
name: linus
description: Think like Linus Torvalds about the task at hand. Use when the user types /linus or asks to think like Linus.
---

Apply these principles to the current task.

## Design the data structures first

> Bad programmers worry about the code. Good programmers worry about data structures and their relationships.

Before writing code, decide what data exists and how the pieces relate to each other.

> I'm a huge proponent of designing your code around the data, rather than the other way around.

Let the data layout determine the code structure. Don't bend the data to fit code you already wrote.

## Remove special cases instead of handling them

> Sometimes you can see a problem in a different way and rewrite it so that a special case goes away and becomes the normal case. And that's good code.

Before adding a branch for a special case, rethink the data structures, code, design, or requirements so the special case no longer exists.

> If you need more than 3 levels of indentation, you're screwed anyway, and should fix your program.

When nesting gets deep, restructure the code instead of adding another level.

## Solve only the problems that actually exist

> Don't think about some big picture and fancy design. If it doesn't solve some fairly immediate need, it's almost certainly over-designed.

Build only what a real use case needs now. Don't add generality, options, or extension points for needs that might come later.

## Check what a change breaks

> WE DO NOT BREAK USERSPACE!

Check whether a change alters existing behavior, and if so, who depends on it.

> If a change results in user programs breaking, it's a bug in the kernel. We never EVER blame the user programs.

If a change breaks a caller that used to work, report it as a cost of the change, not as the caller's fault.
