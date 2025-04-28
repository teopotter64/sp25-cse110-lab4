1. The console will print 3. The for-loop starts to run from i=0, starting from the 0-index in the inputted prices array. After finishing the final element of the array (index 2), i will increment once more and check if "i < prices.length". Since 3 < 3 is NOT true, the for-loop will be exited and i will stop at 3. Since i was defined as a var, it can be accessed outisde of the for loop. Thus, the console.log will be able to access the i-value and print 3.
2. The console will print 150. Every iteration of the for-loop will redefine "discountedPrice" depending on the original price we are checking. The value of disconted price will be the half of the price at index i in the prices array. In the last iteration of the for-loop, the value of discountedPrice will be 150, and since it was defined as a var, that value can be accessed outside of the for-loop. Thus, the console.log will be able to access the final discountedPrice value and print 150.
3. The console will print 150. Every iteration of the for-loop will redefine "finalPrice" depending on the discountedPrice value of that specific iteration. In the last iteration of the for-loop, the value of discountedPrice will be 150 since (150*100)/100 = 150, and since it was defined as a var, that value can be accessed anywhere in the function. Thus, the console.log will be able to access the final discountedPrice value and print 150.
4. This function will return an array of the discounted prices of each original price. This is done by pushing the final price of every for-iteration in to the discounted array defined at the beginning of the function. Since the input prices were [100, 200, 300] with a discount value of 0.5, the function will return an array [50, 100, 150].
5. This will give a "ReferenceError: i is not defined" error. Since i is defined as let, it can only be accessed in the for-loop. Thus, the console.log outisde of the for-loop trying to access it will return an error.
6. This will give a "ReferenceError: discountedPrice is not defined" error. Since discountedPrice is defined as let, it can only be accessed in the for-loop. Thus, the console.log outisde of the for-loop trying to access it will return an error. 
7. The console will print 150. Since finalPrice was defined at the beginning of the function as a let and not in any specific if or for-loop, it can be accessed throughout the function. Thus, the console.log will be able to access the finalPrice value after the for-loop is done running and print the final value of finalPrice.
8. This function will return an array of the discounted prices of each original price, same as Q4.
9. This will give a "ReferenceError: i is not defined" error with the same reasoning in Q5.
10. The console will print 3. Length is a const defined at the beginning of the function, thus it can be accessed anywhere i the function. It is defined as the length of the inputted prices array. Since the inputted array has 3 elements, the value of length will be 3. Thus, the console.log will print 3.
11. This function will return an array of the discounted prices of each original price, same as Q4 and Q8.
12. 
    a. student.name
    b. student["Grad Year"]
    c. student.greeting()
    d. student["Favorite Teacher"].name
    e. student.courseLoad[0]
13. 
    a. 32, because integers map to their string representation, so 2 will be concatenated to the end of 3 as a string.
    b. 1, because strings can't be subtracted from, so '3' will be used as an integer and 2 will be subtracted from it.
    c. 3, becaus null will be treated as 0.
    d. 3null, because null will be treated as a string and concatenated to the end of the string '3'.
    e. 4, because true is mapped to the value 1.
    f. 0, because both false and null are mapped to the value 0.
    g. 3undefined, because undefined will be treated as a string and concatenated to the end of the string '3'.
    h. NaN, because strings can't be subtracted from, so '3' will be used as an integer, and undefined doesn't have a mapping to a nubmer value, so the result will be NaN.
14. 
    a. true, because the string '2' can be mapped to the number 2, and 2 > 1.
    b. false, because the first characters are looked at, and '2' < '1' is false.
    c. true, true, because the string '2' can be mapped to the number 2 and vice versa.
    d. false, because no type conversion is applied in this equality, and a number is not equal to a string.
    e. false, because true is mapped onto the number 1.
    f. true, because any Boolean(a) where a is not 0 or undefined is treated as true.
15. == allows type conversion while === doesn't and also checks the equality of types.
17. The result will be the array [2,4,6]. The inputs for the when modifyArray is called with the input [1,2,3] and doSomething, modifyArray will go through each value of the input array while applying the callback function, i.e doSomething, on that value, pushing it into a new array. Once all values are modified by the callback, the new array is returned. The doSomething function takes a number as input and returns its double. So, 1,2,3 will become 2,4,6 resepctively. The returned array, therefore, will be [2,4,6].
19. The function will outut 1,4,3,2 in that order. 1,4,3 will be outputted at the same time, but 2 will be outputted with a 1 second delay. 