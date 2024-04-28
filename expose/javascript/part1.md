1. Line 9 prints "values added: 20".
2. Line 13 prints "final result: 20".
3. Line 9 prints "values added: 20".
4. Line 13 causes the code to return an error. This is because the variable 'result' was declared using the 'let' keyword, and so the variable is only accessible from within the block it is defined in. Line 13 is outside of this block, so 'result' isn't defined there and an error is thus returned. 
5. Line 9 causes the code to return an error. This is because the variable 'result' was declared using the 'const' keyword, and so this variable's value cannot be reassigned from what it was originally initialized as. 
6. Line 13 causes the code to return an error. This is because the variable 'result' was declared using the 'const' keyword, and so the variable is only accessible from within the block it is defined in. Line 13 is outside of this block, so 'result' isn't defined there and an error is thus returned.