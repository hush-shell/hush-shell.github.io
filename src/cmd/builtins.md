# Builtins

Some commands must be implemented as shell builtins, so that they can mutate the shell state, a thing that would not be possible for an external program. A good example of such kind is the `cd` command, which must change the shell's working directory.

*Hush* currently provides the following builtin commands:

- `cd TARGET_DIR`: change the working directory to *TARGET_DIR*.
- `exec PROGRAM [ARG1, ARG2, ARG3...]`: replace hush process with *PROGRAM* (argument 0 = *PROGRAM*).
- `exec0 PROGRAM ARG0 [ARG1, ARG2, ARG3...]`: replace hush process with *PROGRAM* (argument 0 = *ARG0*).
- `spawn0 PROGRAM ARG0 [ARG1, ARG2, ARG3...]`: spawn *PROGRAM* (argument 0 = *ARG0*).

As *Hush* has no such thing as subshells, builtin commands may not be used in pipes, redirections, or capture blocks.
