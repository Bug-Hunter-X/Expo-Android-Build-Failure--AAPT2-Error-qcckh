# Expo Android Build Failure: AAPT2 Error

This repository demonstrates a common error encountered during the Android build process using Expo CLI. The error, "Execution failed for task ':app:processDebugResources'. > AAPT2 aapt2-4.1.0-6812282...", often arises from problems with Android resource files such as XML layouts, images, or the AndroidManifest.xml itself.  This may include issues with resource naming, conflicts, or missing files.

## Reproducing the Bug

The `bug.js` file contains example code that (when integrated into a larger Expo project) might contribute to this issue.  This example demonstrates the potential for resource-related problems.

## Solution

The `bugSolution.js` file offers a potential solution.  Thoroughly inspect your `android/app/src/main/res` folder and `AndroidManifest.xml` for any inconsistencies or errors.  Common causes and solutions include:

* **Duplicate Resource Names:** Ensure all your resource file names are unique.
* **Missing Resources:** Verify all resources referenced in your code exist.
* **Incorrect Resource Paths:** Check that the resource paths in your code are correct.
* **AndroidManifest Errors:**  Examine `AndroidManifest.xml` for any syntax or structure problems.
* **Image File Issues:** Check if image file formats are supported and properly sized.
* **XML Layout Errors:** Carefully review XML layout files for errors in syntax and structure.

Follow the troubleshooting steps in `bugSolution.js` to systematically address these potential problems.