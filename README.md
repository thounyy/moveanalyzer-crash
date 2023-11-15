# move-analyzer crash

When adding `use std::vector;`, move-analyzer shows an error before I add the comma but it never goes away.

![Screenshot from 2023-11-15 10-33-22](https://github.com/thounyy/moveanalyzer-crash/assets/92447129/8c22bee1-8867-4972-9939-48b19a53e56c)

The move-analyzer server crashes and returns `symbolicator message error: RecvError` in an infinite loop.
This is on Pop Os but also experienced it on Fedora.

It happens very often when I add a line in the middle of a module or function, before adding the comma.
It never happens with https://github.com/movebit/move/tree/sui_move_analyzer
