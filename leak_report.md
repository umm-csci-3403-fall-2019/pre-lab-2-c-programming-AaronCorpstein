# Leak report

The memory errors were happening because the char strip was being called into a variable locally called 'cleaned' and was not subsequently freed once it was not in use. to fix the issue I freed the local variable 'cleaned', but only after it was not needed anymore. 

_Use this document to describe whatever memory leaks you find in `clean_whitespace.c` and how you might fix them. You should also probably remove this explanatory text._

