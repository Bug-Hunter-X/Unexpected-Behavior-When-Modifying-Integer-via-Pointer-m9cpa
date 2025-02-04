# Unexpected Integer Modification via Pointer in C
This repository demonstrates a subtle bug related to pointer arithmetic and integer modification in C. The code appears simple but can lead to unexpected behavior depending on the compiler's optimization level and memory management.

## Bug Description
The primary issue lies in the way the integer 'x' is modified through the pointer 'ptr'. Under certain compiler optimizations, the value of 'x' might not reflect the changes made through the pointer immediately. 

## Bug Solution
The solution involves ensuring the compiler doesn't perform aggressive optimizations that could interfere with the direct modification through the pointer. This is usually achieved by adding compiler flags.