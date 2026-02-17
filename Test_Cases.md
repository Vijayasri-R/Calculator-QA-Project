# Test Cases for Simple Calculator Application

## Project Overview
This document contains detailed test cases for a calculator application that supports basic arithmetic operations: Addition, Subtraction, Multiplication, and Division.

## 1. Functional Test Cases (Valid Inputs)

| Test Case ID | Test Description | Preconditions | Test Steps | Expected Results |
| :--- | :--- | :--- | :--- | :--- |
| **TC-01** | Addition of two positive integers | Calculator is open. | 1. Enter `10`<br>2. Press `+`<br>3. Enter `20`<br>4. Press `=` | Display shows `30`. |
| **TC-02** | Subtraction with negative result | Calculator is open. | 1. Enter `5`<br>2. Press `-`<br>3. Enter `15`<br>4. Press `=` | Display shows `-10`. |
| **TC-03** | Multiplication of decimals | Calculator is open. | 1. Enter `2.5`<br>2. Press `*`<br>3. Enter `4`<br>4. Press `=` | Display shows `10.0`. |
| **TC-04** | Division of a negative number | Calculator is open. | 1. Enter `-50`<br>2. Press `/`<br>3. Enter `5`<br>4. Press `=` | Display shows `-10`. |
| **TC-05** | Complex Calculation (BODMAS) | Multi-step input support. | 1. Enter `10 + 2 * 5` <br>2. Press `=` | Display shows `20`. |

## 2. Boundary & Error Handling (Invalid Inputs)

| Test Case ID | Test Description | Preconditions | Test Steps | Expected Results |
| :--- | :--- | :--- | :--- | :--- |
| **TC-06** | Division by Zero | Calculator is open. | 1. Enter `10`<br>2. Press `/`<br>3. Enter `0`<br>4. Press `=` | Display shows "Error" or "Cannot divide by zero". |
| **TC-07** | Non-numeric Input | Keyboard input enabled. | 1. Try to type `abc` using keyboard. | System should ignore letters or show "Invalid Input". |
| **TC-08** | Multiple Decimals | Calculator is open. | 1. Enter `5.5.5` | System should only accept the first decimal point (`5.5`). |
| **TC-09** | Empty Input Operation | Calculator is open. | 1. Press `+` without any number.<br>2. Press `=` | Display remains `0` or shows no change. |
| **TC-10** | Clear Functionality (Reset) | Numbers are on screen. | 1. Enter `12345`<br>2. Press `C` or `AC` button. | Display resets to `0`. |
