# iplc_sim_comporg
iplc_sim final project for Computer Organization

Who did what (Write what you did under your name once it's done):
- Lorelei:
  - Implemented jump, syscall, and nop. For each, I pushed a new instruction onto the pipeline
    and set its type to be the appropriate type. Additionally, for jump, I set the jump address
    to the address given in the function.
- Mary:
  - I implemented the iplc_sim_LRU_replace_on_miss function. I replaced the last recently
    used cache slot and then moved that so it was the Most Recently Used entry, and then
    percolated it up.
- Tim:
  -
- Will:
  -Implemented the store word, load word, and branch instruction type functions. Structs with member variables for each instruction were provided, so I just pushed another instruction to the pipeline and inserted the correct values into the member variables.
