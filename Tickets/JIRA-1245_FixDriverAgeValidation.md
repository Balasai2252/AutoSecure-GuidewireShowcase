# 🐞 JIRA-1245 – Driver Age Validation Not Triggering

**Type:** Bug  
**Module:** Underwriting Rules  
**Assigned To:** Bala Sai  
**Status:** Fixed  
**Environment:** Guidewire PolicyCenter (Simulated Setup)

---

## 🧾 Summary

DriverAgeValidationRule was not rejecting policies even when driver age was below 18 years.

---

## 🔍 Root Cause

- The rule wasn’t linked properly to `PersonalAutoLine`
- Also missing a null check for empty driver list

---

## 🔧 Fix Implemented

- Corrected product model linkage
- Added null check before accessing `driver.age`

---

## 🧪 Test Cases

| Scenario                        | Expected Outcome      | Status |
|--------------------------------|------------------------|--------|
| Driver age = 16                | Policy rejected        | ✅     |
| Driver age = 18                | Policy accepted        | ✅     |
| No driver attached             | No exception triggered | ✅     |

---

**Resolution:** Deployed fix and verified rule is now triggering as expected.
