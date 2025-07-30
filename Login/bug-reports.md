# 🐞 Bug Reports – Manual QA - OrangeHRM Login

This document lists identified bugs during manual testing of the login functionality in OrangeHRM.

---

## ❌ Bug 1: Access dashboard without logging in

- **Test Case**: Attempt to access the dashboard page directly without prior login.
- **Expected Result**: User is redirected to the login page with an appropriate "Please log in first" message.
- **Actual Result**: A 404 error page is displayed with the message: *"This page can’t be found."*
- **Status**: ❌ Failed
- **Severity**: Medium
- **Steps to Reproduce**:
  1. Open browser.
  2. Navigate directly to `[OrangeHRM Demo Site]([https://opensource-demo.orangehrmlive.com/](https://opensource-demo.orangehrmlive.com/web/index.php/dashboard/index)`.
  3. Observe the result.
- **Suggested Fix**: Implement proper authentication check with redirect to login when accessing protected pages without session.

---

### 🔚 Summary

- **Total Bugs Identified**: 1
- **Blocked Cases**: 0
- **Recommendation**: Ensure all protected routes require authentication and provide clear feedback to unauthorized users.


