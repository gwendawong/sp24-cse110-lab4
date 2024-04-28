1. At line 12, "3" will be printed. This is because `i` was declared with the keyword `var`, so it is accessible throughout the entire function and its value can be reassigned. Since the given array `[100, 200, 300]` has three values and the for loop stops executing once `i` has incremented to be equal to or above the length of this array, when `i` is `3`, it stays at this value and the for loop doesn't execute. Thus, the value of `i` as of line 12 is `3`, which is printed because it is in scope.
2. At line 13, "150" will be printed. This is because `discountedPrice` was declared with the keyword `var`, so it is accessible throughout the entire function and its value can be reassigned. Its value is assigned in line 7, and since the for loop exits with the last loop being when `i` is `2`, the last value `discountedPrice` is assigned to is `price[2] * (1 - 0.5)` (which is `150` with the given input of `[100, 200, 300]` for `price` and `0.5` for `discount`).
3. At line 14, "150" will be printed. This is because `finalPrice` was declared with the keyword `var`, so it is accessible throughout the entire function and its value can be reassigned. Its value is assigned in line 8, and since the for loop exits with the last value `discountedPrice` being assigned to as `150` (as discussed in question 2), `finalPrice` is lastly assigned the value of `Math.round(150 * 100) / 100`, which evalues to `150`, as printed. 
4. This function returns an array where `discount` has been applied to the values of the array `prices`, in this case, `[50, 100, 50]`. This is because `discounted` is declared with the keyword `var`, so it is accessible and can be reassigned throughout the function. The values of `prices` with `discount` applied to them are appended to `discounted` in line 9, and this value is calculated in lines 7 and 8 (as discussed in questions 2 and 3).
5. At line 12, the code causes an error. This is because the variable `i` was declared using the `let` keyword, and so the variable is only accessible from within the block it is defined in. In this case, that is the for loop starting in line 6 and ending on line 10. Line 12 is outside of this block, so `i` isn't defined there and an error thus occurs. 
6. At line 13, the code causes an error. This is because the variable `discountedPrice` was declared using the `let` keyword, and so the variable is only accessible from within the block it is defined in. In this case, that is the for loop starting in line 6 and ending on line 10. Line 13 is outside of this block, so `discountedPrice` isn't defined there and an error thus occurs when it tries to be accessed.
7. At line 14, "150" will be printed. This is because `finalPrice` was declared with the keyword `let`, so it is accessible and can be reassigned throughout the entire block it was declared in. In this case, that is the entire function. Its value is assigned in line 8, and since the for loop exits with the last value `discountedPrice` being assigned to as `150` (as discussed in question 2), `finalPrice` is lastly assigned the value of `Math.round(150 * 100) / 100`, which evalues to `150`, as printed.
8. This function returns an array where `discount` has been applied to the values of the array `prices`, in this case, `[50, 100, 50]`. This is because `discounted` is declared with the keyword `let`, so it is accessible and can be reassigned throughout its code block. In this case, its scope is the entire function. The values of `prices` with `discount` applied to them are appended to `discounted` in line 9, and this value is calculated in lines 7 and 8 (as discussed in questions 2 and 3).
9. At line 11, the code causes an error. This is because the variable `i` was declared using the `let` keyword, and so the variable is only accessible from within the block it is defined in. In this case, that is the for loop starting in line 6 and ending on line 10. Line 11 is outside of this block, so `i` isn't defined there and an error thus occurs. 
10. At line 12, "3" will be printed. This is because `length` was declared with the keyword `const`, making its scope the block it is in and it cannot be reassigned. Its code block, in this case, is the entire function. It's original value was assigned to `prices.length`, which, with the given input, is `3`, so that didn't change the entire function and was thus printed. 
11. This function returns an array where `discount` has been applied to the values of the array `prices`, in this case, `[50, 100, 50]`. This is because `discounted` is declared with the keyword `const`, so it is accessible (but cannot be reassigned) throughout its code block. In this case, its scope is the entire function. Note that, although `const` variables cannot be reassigned, its contents can be mutated, which is what is happening here with the `push` method to add the values to `discounted`. The values of `prices` with `discount` applied to them are appended to `discounted` in line 9, and this value is calculated in line 7 (as discussed in questions 2).
12. Object notation
    
    A. `student.name`

    B. `student['Grad Year']`

    C. `student.greeting()`

    D. `student['Favorite Teacher'].name`

    E. `student.courseLoad[0]`
13. Arithmetic 
    
    A. `'3' + 2 = '32'` since integers map to their exact string representation and the `+` is used for concatenation.
    
    B. `'3' - 2 = 1` since you can't do subtraction on strings, the string is mapped to a number and integer subtraction is done.

    C. `3 + null = 3` since `null` is mapped to `0`. 

    D. `'3' + null = 3null1` since `null` is mapped to its exact string representation and the `+` is used for concatenation.

    E. `true + 3 = 4` since `true` is mapped to `1`.

    F. `false + null = 0` since both `false` and `null` map to `0`.

    G. `'3' + undefined = 3undefined` since `undefined` maps to its exact string representation and the `+` is used for concatenation. 
    
    H. `'3' - undefined = NaN` since  `'3'` maps to `3` for integer subtraction and `undefined` maps to `NaN`. (`3 - NaN = NaN`)
14. Comparison
    
    A. `'2' > 1` evaluates to `true` because `'2'` maps to `2` for integer comparison.
    
    B. `'2' < '12'` evaluates to `false` because `'1'` comes before `'2'` alphabetically, so `'12'` is less than `'2'`. 

    C. `2 == '2'` evaluates to `true` because `'2'` maps to `2` for integer comparison. 

    D. `2 === '2'` evaluates to `false` because the types are different (this conducts a strict equality check without type mapping). 

    E. `true == 2` evaluates to `false` because `true` maps to `1`.

    F. `true === Boolean(2)` evaluates to `true` because the explicit `Boolean` conversion maps all numbers other than `0`, `-0`, and `NaN` to `true`. 
15. `==` does an equality check while `===` does a strict equality check. Essentially, `==` does type conversion and then comparison, while `===` compares both the values and data types of the operands directly against one another. 
16. Code is in file `part2-question16.js`.
17. If the given function is called with the given input, the result will be `[2, 4, 6]`. First, `array` in `modifyArray` is assigned to the value of `[1,2,3]` and `callback` in `modifyArray` is assigned to `doSomething`. For each element of `array`, `doSomething` is called on it, and then that value is stored to the back of `newArr` (which was initialized to be empty). `doSomething` multiplies its input by `2`, so `newArr`, at the end of the for loop, is `array` except each value of `array` has been multiplied by 2. `newArr` is then returned, which is what the result was found to be.  