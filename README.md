# React Native AsyncStorage Error Handling Bug

This repository demonstrates a common bug in React Native applications involving the use of AsyncStorage without proper error handling.  The bug causes the app to crash if there's an error during data storage or retrieval.  The solution demonstrates best practices for handling these potential errors and ensures a more robust application.

## Bug

The original code lacks error handling when using `AsyncStorage.getItem` and `AsyncStorage.setItem`.  This can lead to crashes if AsyncStorage encounters issues such as device storage limitations or corrupted data.

## Solution

The solution implements comprehensive error handling using `.catch` blocks to gracefully handle potential errors.  It also includes input validation to prevent errors caused by incorrect JSON data.