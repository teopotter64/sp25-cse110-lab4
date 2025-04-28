1. values added:  20
2. final result:  20
3. Even though the "result" variable is defined in the if-block the console.log outside the if-block also accesses the "result" variable and its value. We should not use var because in longer and more complicated codes, it can cause issues by causing naming conflicts or accidentally altering the value of a variable outisde of its intended block.
4. values added:  20
5. THe line returns a "ReferenceError: result is not defined" error. This is because let defines the variable as only accessible in the block it's in. As a result, "result" can't be accessed outside of the if-block it's defined in. Thus, the second console.log will give an error.
6. This will give a "TypeError: Assignment to constant variable" error. Since "result" is a const, it's value cannot be redeclared or reassigned. Thus, the line "result = num1 + num2;" will give an error.
7. This will give the same error as Q6. Additionally, const works only in the scope of the block, so any arbitrary const variable in an if-block couldn't be accessed with a console.log outisde of its if-block.