# LeetCode-Week-4
TITLE - LONGEST COMMON PREFIX
EASY
Approach: Horizontal Scanning
The logic behind this solution is to compare the strings one by one, narrowing down the prefix as inconsistencies are found.
• Initialization: We start by assuming the first string in the array is the potential longest common prefix.
• Comparison: We iterate through the rest of the strings. For each string, we check if the current prefix exists at the very beginning (index 0).
• Reduction: If the string does not start with the current prefix, we shorten the prefix by removing its last character and try again.
• Termination: This continues until either the prefix matches the start of the current string or the prefix becomes an empty string (meaning no commonality exists).
Complexity Analysis
• Time Complexity: O(S), where S is the sum of all characters in all strings. In the worst case, every character in every string is compared once.
• Space Complexity: O(1), as we only store the prefix string and do not use additional data structures that scale with the input size.
