# add-frac

# task
You will have a list of rationals in the form

m = [ [numer_1, denom_1] , ... , [numer_n, denom_n] ] or m = [ (numer_1, denom_1) , ... , (numer_n, denom_n) ]

where all numbers are positive integers.
You have to produce the sum N/D of these rationals in an irreducible form
ie N and D have only 1 for divisor.

The result will be written in the form

[N, D] in Ruby/Python/Clojure/JS/CS/PHP

Just "N D" in Haskell or Some "N D" in F#, Ocaml

Some((N, D)) in Rust
"[N, D]" in Java, CSharp, TS
{N, D} in C++
{N, D} in Elixir
c(N, D) in R
#Example:

[ [1, 2], [1, 3], [1, 4] ] ---->
[13, 12] or: Just "13 12" (Haskell) or: "[13, 12]" (Java, CSharp, TS) or: {13, 12} (C++, Elixir), (Some "13 12") Fsharp, (13, 12) Swift,
c(13, 12) R



pseudo code

adding 3 fractions

first multiply all the denominators together.... thats how you get the denominators
  loop through the array and multiply all the denominators together
second numerator is kinda more diffcult.. a/b c/d e/f
  (a * d * f) + (c * b * f) + (e * d * a) this will give you the numerator
loop though the array
find the fjrst numerator and multiply it by the other denominators
