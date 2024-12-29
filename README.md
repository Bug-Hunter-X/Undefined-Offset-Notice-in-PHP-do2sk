# PHP Undefined Offset Notice

This repository demonstrates a common PHP error: the "Undefined offset" notice.  This notice arises when trying to access an array element using an index that doesn't exist.  The example shows how to prevent this error by checking if the index exists before accessing it.

The `bug.php` file contains the buggy code, while `bugSolution.php` provides the corrected version.

**Issue:** The code attempts to access `$myArray[0]` without verifying if the array is empty, leading to a notice if the array is empty or doesn't contain an element at index 0.

**Solution:** The solution adds an `isset()` check to ensure the index exists before access.  This prevents the notice and improves code robustness.