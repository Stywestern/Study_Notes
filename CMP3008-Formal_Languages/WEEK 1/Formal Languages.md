Alphabet: Set of symbols (like a, b, c)

String: Finite sequence of symbols (like abcaaacb)

Operations:
- Concat: abc I cca = abccca
- Reverse: abc^rev = cba
- Repeat:  abc^rep = abcabc

If a string _s_ is constructed using the alphabet _A_, then _s_ is a string over _A_.

Length of a String: len(string) = num_of(s where s is a symbol in alphabet)

Empty String: len(string) = 0, denoted $\lambda$. 

Substring: If elements of string w consecutively appears in string s, then w is a substring of s (like cad is a substring of cadage)

Σ* = set of all strings formed by concatenating zero or more symbols in Σ

Σ+ = set of all non-empty strings formed by concatenating symbols in Σ

A Formal Language is any subset of Σ* (like L1 = { a^nb^n: n ≥ 0 } and L2 = { ab, aa })

Grammar: The mechanism that describe strings in a language. A grammar G consists of:
- V: a finite set of variable or non-terminal symbols (like apostrophe)
- T: a finite set of terminal symbols (like the dot)
- S: a variable called the start symbol (empty string in English)
- P: a set of productions (like and)
