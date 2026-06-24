---
tracker: [Bug, Physics, Pending]
date: 2026-06-25 14:30:00
---
Jolt Physics is throwing a fatal hardware fault on Linux when compiled with GCC 13. 

The issue is unaligned memory access into the 128-bit CPU registers. I need to force `alignas(16)` on the root Entity container, not just the Transform component. Will test this tomorrow.
