# Registration Page Test Cases

## Test Case 1: Valid Registration
**Test Case ID:** TC_REG_001  
**Priority:** High  
**Test Type:** Functional

### Test Steps:
1. Open registration page
2. Enter valid first name: John
3. Enter valid last name: Doe
4. Enter valid email: john.doe@example.com
5. Enter valid password: Test@123
6. Confirm password: Test@123
7. Check "I agree to terms and conditions"
8. Click "Register" button

### Expected Result:
- Registration successful
- Confirmation email sent
- User redirected to login page or dashboard
- Success message displayed

### Actual Result:
Pass ✅

---

## Test Case 2: Duplicate Email Registration
**Test Case ID:** TC_REG_002  
**Priority:** High  
**Test Type:** Negative

### Test Steps:
1. Open registration page
2. Enter email that already exists in system
3. Fill all other fields correctly
4. Click "Register" button

### Expected Result:
- Error message: "Email already exists"
- User remains on registration page
- Suggest login or password recovery

### Actual Result:
Pass ✅

---

## Test Case 3: Weak Password
**Test Case ID:** TC_REG_003  
**Priority:** High  
**Test Type:** Negative

### Test Steps:
1. Open registration page
2. Enter all valid details
3. Enter weak password: 123
4. Click "Register" button

### Expected Result:
- Error message: "Password must be at least 8 characters with uppercase, lowercase, number, and special character"
- Show password strength indicator
- Registration blocked

### Actual Result:
Pass ✅

---

## Test Case 4: Password Mismatch
**Test Case ID:** TC_REG_004  
**Priority:** High  
**Test Type:** Negative

### Test Steps:
1. Open registration page
2. Enter password: Test@123
3. Enter confirm password: Test@124
4. Click "Register" button

### Expected Result:
- Error message: "Passwords do not match"
- Highlight both password fields
- Registration blocked

### Actual Result:
Pass ✅

---

## Test Case 5: Invalid Email Format
**Test Case ID:** TC_REG_005  
**Priority:** Medium  
**Test Type:** Negative

### Test Steps:
1. Open registration page
2. Enter invalid email: testuser@
3. Fill other fields correctly
4. Click "Register" button

### Expected Result:
- Error message: "Please enter a valid email address"
- Email field highlighted in red
- Registration blocked

### Actual Result:
Pass ✅

---

## Test Case 6: Empty Required Fields
**Test Case ID:** TC_REG_006  
**Priority:** High  
**Test Type:** Negative

### Test Steps:
1. Open registration page
2. Leave all fields empty
3. Click "Register" button

### Expected Result:
- Error messages for all required fields
- "First name is required"
- "Email is required"
- "Password is required"
- Registration blocked

### Actual Result:
Pass ✅

---

## Summary
- Total Test Cases: 6
- Passed: 6
- Failed: 0
- Success Rate: 100%
