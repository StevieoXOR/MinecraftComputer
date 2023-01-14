# MinecraftComputer
My process of creating a computer in Minecraft. Currently hasn't advanced past a weak calculator.

Note that subtraction is possible by using 2's complement on a positive number to turn it into its negative counterpart; vice versa also works. Don't forget to discard any extra bits (e.g. if starting with 8 bits and end up with 9 bits, discard the most significant bit)
For example:
  +17 => 2's complement => -17
  -17 => 2's complement => +17

Note that multiplication and division are possible when using only bit shifts, addition, comparison to value 0, and memory. This is slow, but it works.
https://www.cise.ufl.edu/~mssz/CompOrg/CDA-arith.html
