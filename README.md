# KLH-CSE-2520030141-Rayanki-Himavarshini-DSA-3


# **Rayanki Himavarshini**
# 1. Implemented basic Z-array construction
# 2. Added Z-box optimization
# 3. Documented Z-Algorithm implementation


# Text + Pattern
#     ↓
 # Pattern Matching Problem
       ↓
# Z-Algorithm / Z-Function
       ↓
# Z-Array
       ↓
# Find all pattern occurrences
       ↓
# O(n + m)

# src/
#  └── ZAlgorithm.java

# The Abstract


# Pattern matching is the process of locating every occurrence of a small string (the pattern) within a larger string (the text). It underlies search engines, text editors, DNA sequencing tools, and cyber-security systems. The naive character-by-character approach re-examines text after every failed attempt, giving a worst-case time complexity of O(n × m) that degrades sharply on large or repetitive data.
# This project implements the Z-Algorithm, a linear-time exact string-matching technique. The pattern and text are concatenated into a single string S = P + "$" + T, and a Z-array is built in one pass, where Z[i] is the length of the longest substring starting at position i that matches a prefix of S. A pattern occurrence is found wherever Z[i] equals the length of the pattern.
# By reusing previously matched information through the Z-box technique, the algorithm avoids redundant comparisons and guarantees O(n + m) time in the best, average, and worst cases. The system is implemented in Java and validated on sample text-pattern pairs, including overlapping and near-miss cases, to confirm correctness and demonstrate its efficiency over naive searching.
