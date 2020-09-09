# Leak report

# Valgrind reports 46 bytes lost over 6 blocks with 7 allocations and 1 free. The reason we are getting memory leaks is because the program allocates memory to process the word but never frees it up unless its an empty string. We would fix this by simply adding a component to the program that frees up the space after the word has been processed. 

_Use this document to describe whatever memory leaks you find in `clean_whitespace.c` and how you might fix them. You should also probably remove this explanatory text._
