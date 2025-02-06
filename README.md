# Incorrect Null and Undefined Handling in JavaScript Function
This repository demonstrates a common error in JavaScript: incorrect handling of null and undefined values. The function `foo` attempts to add two numbers but fails to correctly handle cases where one or both inputs are null or undefined, leading to unexpected NaN values.
The solution demonstrates how to properly check for both null and undefined using loose comparison (==) to avoid such issues.
## Bug
The original function `foo` incorrectly handles null and undefined values. It checks only for null and doesn't consider undefined, which results in NaN when undefined is passed as an argument.
## Solution
The solution addresses this by explicitly checking for both null and undefined using loose equality (==). This ensures the function consistently returns 0 when either input is null or undefined. 