# Lua pairs iterator modification during iteration

This repository demonstrates a potential issue with Lua's `pairs` iterator when the table being iterated over is modified within the loop.  In certain scenarios, this can cause some elements of the table to be skipped or an infinite loop to occur.

The `bug.lua` file contains code that exemplifies this problem. The `bugSolution.lua` file offers a solution, suggesting an alternative approach to avoid this unexpected behavior.

This issue is important to be aware of when dealing with nested tables and mutable data structures in Lua.