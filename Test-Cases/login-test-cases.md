# Login Page Test Cases

## Test Case 1: Valid Login
**Test Case ID:** TC_LOGIN_001  
**Priority:** High  
**Test Type:** Functional

### Pre-conditions:
- User must be registered
- User must have valid credentials

### Test Steps:
1. Open the login page
2. Enter valid email: test@example.com
3. Enter valid password: Test@123
4. Click "Login" button

### Expected Result:
- User is logged in successfully
- Redirected to dashboard/home page
- Welcome message is displayed

### Actual Result:
Pass ✅

---

## Test Case 2: Invalid Email
**Test Case ID:** TC_LOGIN_002  
**Priority:** High  
**Test Type:** Negative

### Test Steps:
1. Open the login page
2. Enter invalid email: invalidemail
3. Enter valid password: Test@123
4. Click "Login" button

### Expected Result:
- Error message: "Please enter a valid email address"
- User remains on login page

### Actual Result:
Pass ✅

---

## Test Case 3: Empty Password
**Test Case ID:** TC_LOGIN_003  
**Priority:** High  
**Test Type:** Negative

### Test Steps:
1. Open the login page
2. Enter valid email: test@example.com
3. Leave password field empty
4. Click "Login" button

### Expected Result:
- Error message: "Password is required"
- Login button should be disabled or show error

### Actual Result:
Pass ✅

---

## Test Case 4: Wrong Password
**Test Case ID:** TC_LOGIN_004  
**Priority:** High  
**Test Type:** Negative

### Test Steps:
1. Open the login page
2. Enter valid email: test@example.com
3. Enter wrong password: WrongPass123
4. Click "Login" button

### Expected Result:
- Error message: "Invalid email or password"
- User remains on login page
- Login attempts should be tracked

### Actual Result:
Pass ✅

---

## Test Case 5: Password Visibility Toggle
**Test Case ID:** TC_LOGIN_005  
**Priority:** Medium  
**Test Type:** Functional

### Test Steps:
1. Open the login page
2. Enter password in password field
3. Click on "Show Password" icon/button

### Expected Result:
- Password should become visible in plain text
- Icon should change to "Hide Password"
- Clicking again should hide password

### Actual Result:
Pass ✅

---

## Summary
- Total Test Cases: 5
- Passed: 5
- Failed: 0
- Success Rate: 100%
