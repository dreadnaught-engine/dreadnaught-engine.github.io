---
layout: default
title: Engineering Notes
permalink: /notes
---

<style>
  /* Carmack-Style Terminal Override */
  .notes-terminal {
    background-color: #02040a;
    border: 1px solid #14203d;
    border-top: 4px solid #00ff66;
    padding: 30px;
    font-family: monospace;
    color: #00ff66; /* Phosphor Green */
    min-height: 60vh;
    box-shadow: inset 0 0 30px rgba(0, 255, 102, 0.05);
  }
  .notes-terminal h1 {
    font-family: 'Rajdhani', sans-serif;
    color: #fff;
    margin-top: 0;
    border-bottom: 1px dashed #14203d;
    padding-bottom: 10px;
  }
  .notes-terminal p {
    margin-bottom: 15px;
    line-height: 1.6;
    font-size: 0.95rem;
  }
  
  /* Syntax Highlighting for Tags */
  .timestamp { color: #8ab4f8; font-weight: bold; }
  .tag-sys { color: #d600ff; }
  .tag-warn { color: #ff3333; background-color: rgba(255,51,51,0.1); padding: 0 4px; }
  
  .notes-terminal hr {
    border: none;
    border-top: 1px dashed #14203d;
    margin: 25px 0;
  }
  .notes-terminal a {
    color: #8ab4f8;
    text-decoration: underline;
  }
</style>

<div class="notes-terminal">
  <h1>SYS_LOG // RAW_MEMORY_DUMP</h1>
  <p style="color: #555; margin-bottom: 40px;">> This is an unformatted engineering ledger. Chronological order (newest top). Zero friction.</p>

  <p><span class="timestamp">[2026-06-25 14:30]</span> <span class="tag-sys">[RHI]</span> Figured out the PCIe bus saturation issue. Moving the voxel debris generation entirely to a compute shader. Needs indirect dispatch.</p>

  <hr>

  <p><span class="timestamp">[2026-06-24 09:15]</span> <span class="tag-sys">[ECS]</span> RESOURCE: Read up on EA's Frostbite task scheduler.<br>
  Link: <a href="#">https://example.com/frostbite-scheduler</a><br>
  Need to adapt their ring-buffer approach for our Wasm Deferred Mutation Queue.</p>

  <hr>

  <p><span class="timestamp">[2026-06-23 22:45]</span> <span class="tag-warn">[BUG]</span> Jolt Physics is crashing on Linux when compiling with GCC 13. Alignment fault. Might need to force alignas(16) on the root Entity container, not just the Transform component.</p>

</div>
