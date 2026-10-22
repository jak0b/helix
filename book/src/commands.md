# Commands

- [Typable commands](#typable-commands)
- [Static commands](#static-commands)

## Typable commands

Typable commands are used from command mode and may take arguments. Command mode can be activated by pressing `:`. The built-in typable commands are:

{{#include ./generated/typable-cmd.md}}

With a tracked file open, `:stage-chunk` stages the Git diff chunks touched by the current selection, including unsaved buffer changes. `:unstage-chunk` removes selected staged chunks from the index without changing the buffer. `:stage-buffer` stages the entire current buffer, including unsaved changes. `:unstage-buffer` removes all staged changes for the current file from the index. Neither unstage command changes the buffer. Staged chunks retain their diff gutter color and symbol, but appear dimmed. Reload the buffer to refresh the gutter after changing the Git index outside Helix.

## Static Commands

Static commands take no arguments and can be bound to keys. Static commands can also be executed from the command picker (`<space>?`). The built-in static commands are:

{{#include ./generated/static-cmd.md}}
