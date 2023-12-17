try to create program which prints something like

```
===============================
01.02.2023 Monday
-------------------------------
01.02.2023 Tuesday
-------------------------------
01.02.2023 Wednesday
-------------------------------
01.02.2023 Thursday
-------------------------------
01.02.2023 Friday
-------------------------------
01.02.2023 Saturday						##
-------------------------------
01.02.2023 Sunday							##
===============================
```

New things I have learned:

- constants declare constant values. These represent a value, not a memory address. This is the most common thing one would reach for and would replace static as we know it today in almost all cases.
- statics declare global variables. These represent a memory address. They would be rarely used: the primary use cases are global locks, global atomic counters, and interfacing with legacy C libraries.


https://www.reddit.com/r/rust/comments/u4wedx/when_to_pass_in_self_vs_self_in_rust/
& -> a borrow. Gets returned to owner at the end of scope
&mut -> An exclusive borrow. Guarantees that holder is the only one with a reference
Self -> Move. Unless you return it explicitly, it is dropped at the end of scope


git remote set-url origin git@github.com:aldehydkrotonowy/rust-playground.git