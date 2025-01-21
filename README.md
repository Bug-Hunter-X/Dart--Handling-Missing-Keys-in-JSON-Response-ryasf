# Dart: Handling Missing Keys in JSON Response

This repository demonstrates a common error in Dart when handling JSON responses from APIs: attempting to access a key that might not exist. The `bug.dart` file shows the problematic code, while `bugSolution.dart` provides a corrected version.

## Problem

The original code assumes the JSON response always contains a key named 'key'. If the API response changes or this key is missing, a runtime exception will occur. 

## Solution

The improved code uses the `containsKey` method to check if the key exists before accessing it. If the key is missing, it gracefully handles the situation without crashing. It also demonstrates safer null handling using the null-aware operator (`?.`).