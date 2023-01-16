# MinecraftComputer
My process of creating a computer in Minecraft. Currently hasn't advanced past a weak calculator. The implementation of each opcode is inefficient because the multiplexers (MUXes) to select which operation (i.e. add, shift, etc) to perform are ill-formed and use AND gates on the opcode bits instead of working efficiently by default due to smartly designing the wiring. Can be fixed by vertically stacking every possible operation and running MUXes from each operation's output. Note that MineCraft has a vertical height block limit.

Note that subtraction is possible by using 2's complement on a positive number to turn it into its negative counterpart; vice versa also works. Don't forget to discard any extra bits (e.g. if starting with 8 bits and end up with 9 bits, discard the most significant bit)
For example:
  +17 => 2's complement => -17
  -17 => 2's complement => +17

Note that multiplication and division are possible when using only bit shifts, addition, comparison to value 0, and memory. This is slow, but it works.
https://www.cise.ufl.edu/~mssz/CompOrg/CDA-arith.html


This is my most recent MineCraft build for the redstone computer. The computer needs slime blocks in order to work correctly, so extremely old versions of MineCraft may not work correctly. The intended version is MineCraft 1.19

The zip include 16 region files (.mca) which contain information about each chunk in the world.
The zipped files should be placed inside (and should overwrite, meaning you should delete the original region files from your new world's creation) the "region" folder of a new MineCraft save, where the world created is version 1.19.
You will need to extract the.zip file to your new MineCraft save's "AppData>Roaming>.minecraft>NewWorld[orInsertYourWorldName]>region".

Entities shouldn't matter as the MineCraft redstone computer doesn't depend on active mob entities. That's why I didn't include those files.
