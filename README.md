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
The testSumRangeReverseOrder test was failing. It expected 15 but the method returned 0.

## What was the issue in the code?
The loop only worked when the start value was less than or equal to the end value. When the range was given in reverse order, the loop never executed.

## What change did you make to fix it?
I added logic to handle both ascending and descending ranges. If start is greater than end, the loop counts downward.

## How did the tests help guide your fix?
The failing reverse-order test showed that the method needed to support ranges in both directions. After updating the loop logic, all three tests passed.
-

---

# Overall Reflection

## Which task was the easiest to fix? Why?
Task 1 was the easiest because the existing getGrade method already passed all of the provided JUnit tests.

## Which task was the most difficult? Why?
Task 3 was the most difficult because the method worked for normal ranges but failed when the start value was greater than the end value.

## How did Git help you track your progress through the debugging process?
Git allowed me to save each stage of the debugging process as a separate commit and keep a history of the changes I made.

## Why is it important to make small, frequent commits when debugging code?
Small commits make it easier to identify which changes fixed a problem and make it easier to return to an earlier working version.

## What did you learn about using JUnit tests to guide debugging?
JUnit tests helped identify the specific inputs that caused incorrect behavior and confirmed when my changes fixed the problems.

---

# Commit 5: Final Reflection

## What did you complete or update before making this final commit?
I completed the Task 3 reflection, reviewed the previous reflection sections, and completed the overall reflection.

## Why is it useful to document your work after completing a programming task?
Documentation provides a record of what was changed, why it was changed, and what was learned during the development process.
-