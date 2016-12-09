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
  -iplc_sim_trap_address - Get the index and tag we are looking for, then go through our cache and see if any of our indices match our tag. If so, run update on hit (since we hit). If not, run replace on miss (since we missed). Return hit (0 or 1) at the end.
  -Step 3: See if we've hit. If we miss, add our delay. If it's an R-type, write to the writeback register and clear the main register
- Will:
  -Implemented the store word, load word, and branch instruction type functions. Structs with member variables for each instruction were provided, so I just pushed another instruction to the pipeline and inserted the correct values into the member variables. Then implemented steps 2, 4, and 6 of the iplc_sim_push_pipeline_stage, handling the branch prediction whether it be correct or incorrect and pushing the data to the next stage if necesssary, checking for data misses, and pushing the pipeline data at the end of the function.
