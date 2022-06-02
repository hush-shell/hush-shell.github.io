# Overview

In order to attain it's goals, *Hush* takes great inspiration from *Lua*, the industry proven embedded scripting language. If you're familiar with *Lua*, you'll notice that, except for the shell capabilities, *Hush* feels a lot like a simplified version of it.

As such, *Hush* provides:

- Static scoping
- Strong dynamic typing
- Garbage collection
- First class functions
- Good support for functional programming
- Basic support for object oriented programming
- First class shell capabilities

While being somewhat similar to scripting languages like *Lua*, *Python* and *Ruby*, even though it is much simpler than those, *Hush* strives to feel pretty much like *Bash* when it comes to shell capabilities. There are only minor syntactical differences regarding invoking and interconnecting external programs, and therefore you won't have to learn all the shell syntax again.

But while most shell and even general purpose script languages focus a lot on **flexibility**, *Hush* favors **robustness**, which may come at the cost of some flexibility. As such, the language does it's best to empower the programmer to write robust scripts that work in diverse scenarios. It does so by preventing, by design, entire classes of bugs that often occur in shell scripts.

Being a shell scripting language, the typical use cases for *Hush* are operating systems instrumenting and infrastructure programming. In practice, *Hush* should be a good fit in any scenario where the heavy lifting is done by external programs, and you just need to make them to work together.
