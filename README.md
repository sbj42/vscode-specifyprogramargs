# Bug: Escape to cancel doesn't work

```
vscode 1.86.2
vscode-java-debug 0.56.1
jdk 17.0.4.1
```

# Example 1

1. Open this repo in vscode.
2. Open `Test.java` and press `F5`.
3. Pop-up appears with "Press 'Enter' to confirm your input or 'Escape' to cancel".
4. Press Escape.
5. Terminal appears and runs the test program with no arguments.

Expected behavior: At step 5, no terminal appears and the program is not run.

# Example 2

1. Open this repo in vscode.
2. Open `Test.java` and press `F5`.
3. Pop-up appears with "Press 'Enter' to confirm your input or 'Escape' to cancel".
4. Hold `Ctrl` and press `Tab`.  This closes the input popup and opens the tab switcher popup.
5. (while holding `Ctrl`) Terminal appears and runs the test program with no arguments.

Expected behavior: At step 5, no terminal appears and the program is not run.
