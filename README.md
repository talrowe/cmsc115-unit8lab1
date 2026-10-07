# Lab Reflection: Git Version Control + Debugging (BuggyProgram)

## Student Name
Thomas Rowe

## GitHub Repository URL
https://github.com/talrowe/cmsc115-unit8lab1

---

# Commit 1: Initial Commit

## What did you include in this commit?
- This is a first upload for the README and BuggyProgram from the class and the three task test file placeholders.

## What was the purpose of this commit?
- The purpose of this commit was to create a baseline version of the project before making any debugging changes.

---

# Commit 2: Task 1 (getGrade)

## Which tests in Task1Test were failing before your fix?
None. Both Task1Test tests passed.

## What was the issue in the code?
There was no issue with the getGrade method. The existing grade boundaries matched the expected behavior in the JUnit tests.

## What change did you make to fix it?
No change to getGrade was required.

## How did the tests help guide your fix?
The tests confirmed that the existing implementation was already correct.

# Commit 3: Task 2 (sumEvenNumbers)

## Which tests in Task2Test were failing before your fix?
All three tests were failing: testEmpty, testOddNumbers, and testSumEvenNumbers.

## What was the issue in the code?
The loop used `i <= values.length`, which caused the program to access an array index beyond the end of the array. The sum also started at 1 instead of 0.

## What change did you make to fix it?
I changed the loop condition to `i < values.length` and initialized `sum` to 0.

## How did the tests help guide your fix?
The tests showed that the method was throwing ArrayIndexOutOfBoundsException for every input. After fixing the loop and initial sum value, all three tests passed.
-

---

# Commit 4: Task 3 (sumRange)

## Which tests in Task3Test were failing before your fix?
-

## What was the issue in the code?
-

## What change did you make to fix it?
-

## How did the tests help guide your fix?
-

---

# Overall Reflection

## Which task was the easiest to fix? Why?
-

## Which task was the most difficult? Why?
-

## How did Git help you track your progress through the debugging process?
-

## Why is it important to make small, frequent commits when debugging code?
-

## What did you learn about using JUnit tests to guide debugging?
-

---

# Commit 5: Final Reflection

## What did you complete or update before making this final commit?
-

## Why is it useful to document your work after completing a programming task?
-