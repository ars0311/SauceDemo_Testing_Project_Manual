# 🧪 SauceDemo Manual Testing Project

## 📌 Project Overview

This repository contains a **complete A-Z manual testing suite** for the [SauceDemo](https://www.saucedemo.com/) e-commerce website. The project covers **129 test cases** across 10 modules including functional, negative, security, visual, performance, and edge case testing.

### 🎯 Key Features

- ✅ **129 Test Cases** — Full coverage of all functionalities
- ✅ **10 Test Modules** — Login, Inventory, Cart, Checkout, Security, Visual, Edge Cases
- ✅ **6 Special Users** — standard_user, locked_out_user, problem_user, performance_glitch_user, error_user, visual_user
- ✅ **Complete Documentation** — Test Plan, Scenarios, Test Data, Bug Reports, Final Report
- ✅ **11 Real Bugs Found** — Including 2 Blocker, 6 Major, 3 Minor
- ✅ **91.5% Pass Rate** — 118 passed / 11 failed

---

## 📊 Project Statistics

| Metric | Value |
|--------|-------|
| **Total Test Cases** | 129 |
| **Test Cases Executed** | 129 (100%) |
| **Passed** | 118 |
| **Failed** | 11 |
| **Pass Rate** | 91.5% |
| **Total Bugs Found** | 11 |
| **Blocker Bugs** | 2 |
| **Major Bugs** | 6 |
| **Minor Bugs** | 3 |
| **Test Duration** | 6 Days |
| **Browsers Tested** | Chrome, Firefox, Edge |

---

SauceDemo_Manual_Testing_Project/
│
├── README.md # This file (complete project documentation)
│
├── 01_Test_Planning/
│ ├── Test_Plan.docx # Complete test strategy document
│ └── Test_Scenarios.xlsx # High-level scenario list
│
├── 02_Test_Cases/
│ └── Test_Cases_Master.xlsx # 129 detailed test cases
│
├── 03_Test_Data/
│ └── Test_Data.csv # All test data reference
│
├── 04_Bug_Reports/
│ └── Bug_Reports.xlsx # 11 bugs with severity/priority
│
├── 05_Screenshots/
│ ├── BUG-001.png # problem_user broken images
│ ├── BUG-002.png # visual_user text overlap
│ ├── BUG-003.png # Sorting reset issue
│ ├── BUG-004.png # error_user add to cart fails
│ ├── BUG-005.png # error_user remove from cart fails
│ ├── BUG-006.png # error_user stuck on checkout
│ ├── BUG-007.png # Tax rounding error
│ ├── BUG-008.png # problem_user tax wrong
│ ├── BUG-009.png # visual_user overlap
│ ├── BUG-010.png # problem_user full flow tax
│ └── BUG-011.png # error_user cannot checkout
│
└── 06_Final_Reports/
└── Test_Completion_Report.docx # Final execution report


---

## 🚀 Getting Started

### Prerequisites

| Tool | Version | Purpose |
|------|---------|---------|
| Browser | Chrome 120+ | Test execution |
| Microsoft Excel | 2021+ | View test cases & data |
| Microsoft Word | 2021+ | View reports |
| Notepad | Any | CSV file editing |

### Test Environment

| Component | Specification |
|-----------|---------------|
| **URL** | https://www.saucedemo.com/ |
| **OS** | Windows 11 / macOS |
| **Browsers** | Chrome 120, Firefox 121, Edge 120 |

### Test Users (All password: `secret_sauce`)

| Username | Purpose |
|----------|---------|
| `standard_user` | Normal positive flow testing |
| `locked_out_user` | Negative login testing |
| `problem_user` | Broken images / weird behavior |
| `performance_glitch_user` | Slow loading / performance |
| `error_user` | Checkout failure testing |
| `visual_user` | Layout / alignment testing |

---

## 📋 Test Coverage

### Module-Wise Breakdown

| Module | TCs | Passed | Failed | Pass Rate |
|--------|-----|--------|--------|-----------|
| Login | 13 | 13 | 0 | 100% |
| Inventory | 18 | 15 | 3 | 83.3% |
| Product Detail | 12 | 11 | 1 | 91.7% |
| Cart | 15 | 14 | 1 | 93.3% |
| Checkout Step 1 | 14 | 13 | 1 | 92.9% |
| Checkout Step 2 | 15 | 12 | 3 | 80.0% |
| Menu | 10 | 10 | 0 | 100% |
| Security | 12 | 12 | 0 | 100% |
| Visual | 8 | 7 | 1 | 87.5% |
| Negative/Edge | 12 | 11 | 1 | 91.7% |
| **TOTAL** | **129** | **118** | **11** | **91.5%** |

### Test Type Coverage
Positive Functional: 27 TCs (20.9%)
Negative Testing: 89 TCs (69.0%)
Security Testing: 12 TCs (9.3%)
Visual/UI Testing: 8 TCs (6.2%)
Edge Cases: 12 TCs (9.3%)


---

## 🐛 Bugs Found

### Bug Summary

| Severity | Count | Percentage |
|----------|-------|------------|
| Blocker | 2 | 18% |
| Major | 6 | 55% |
| Minor | 3 | 27% |
| **Total** | **11** | **100%** |

### Detailed Bug List

| Bug ID | Module | Severity | Title | Status |
|--------|--------|----------|-------|--------|
| BUG-001 | Inventory | Major | Product images missing for problem_user | Open |
| BUG-002 | Inventory | Minor | Text overlapping for visual_user | Open |
| BUG-003 | Inventory | Minor | Sorting resets after navigation | Open |
| BUG-004 | Product Detail | Major | Add to cart fails for error_user | Open |
| BUG-005 | Cart | Major | Remove from cart fails for error_user | Open |
| BUG-006 | Checkout | Blocker | error_user stuck on checkout step 1 | Open |
| BUG-007 | Checkout | Major | Tax rounding error for 3+ items ($7.03 vs $7.04) | Open |
| BUG-008 | Checkout | Major | Incorrect tax for problem_user | Open |
| BUG-009 | Visual | Minor | visual_user text overlap | Open |
| BUG-010 | Edge | Major | problem_user wrong tax on full flow | Open |
| BUG-011 | Edge | Blocker | error_user cannot complete checkout | Open |

---

## 📝 Sample Test Cases

### TC-001: Login Positive (LOG-001)

| Field | Value |
|-------|-------|
| **TC ID** | LOG-001 |
| **Module** | Login |
| **Test Type** | Positive |
| **Preconditions** | Browser open, clear cache |
| **Test Steps** | 1. Navigate to https://www.saucedemo.com/<br>2. Enter username: standard_user<br>3. Enter password: secret_sauce<br>4. Click Login |
| **Expected Result** | Redirected to /inventory.html; No error message |
| **Status** | ✅ PASS |

### TC-002: Login Negative - Locked User (LOG-006)

| Field | Value |
|-------|-------|
| **TC ID** | LOG-006 |
| **Module** | Login |
| **Test Type** | Negative |
| **Preconditions** | Browser open |
| **Test Steps** | 1. Navigate to login page<br>2. Enter username: locked_out_user<br>3. Enter password: secret_sauce<br>4. Click Login |
| **Expected Result** | Error: "Epic sadface: Sorry, this user has been locked out." |
| **Status** | ✅ PASS |

### TC-003: Checkout Math Validation (CH2-004)

| Field | Value |
|-------|-------|
| **TC ID** | CH2-004 |
| **Module** | Checkout Step 2 |
| **Test Type** | Math Validation |
| **Preconditions** | 3 items in cart: Backpack ($29.99) + Fleece Jacket ($49.99) + Onesie ($7.99) |
| **Calculation** | Item Total = $87.97<br>Tax (8%) = $7.0376 → Expected $7.04<br>Final Total = $95.01 |
| **Actual Result** | UI shows Tax = $7.03 |
| **Status** | ❌ FAIL (BUG-007) |

---

## 🔧 Test Data Reference

### Login Credentials

| DATA ID | Field | Value | Used In |
|---------|-------|-------|---------|
| D001 | Valid Username | standard_user | LOG-001, LOG-003... |
| D002 | Valid Password | secret_sauce | All Login TCs |
| D003 | Locked Username | locked_out_user | LOG-006 |
| D004 | Problem Username | problem_user | INV-010, CH2-013 |
| D005 | Performance Username | performance_glitch_user | INV-012, NEG-009 |
| D006 | Error Username | error_user | PDP-008, CART-015, NEG-011 |
| D007 | Visual Username | visual_user | INV-011, VIS-001 |

### Checkout Test Data

| DATA ID | Field | Value | Used In |
|---------|-------|-------|---------|
| D014 | Valid First Name | John | CH1-001, CH1-003... |
| D015 | Valid Last Name | Doe | CH1-001, CH1-002... |
| D016 | Valid Postal Code | 12345 | CH1-001, CH1-002... |
| D017 | Empty First Name | "" | CH1-002 |
| D018 | Empty Last Name | "" | CH1-003 |
| D019 | Empty Postal Code | "" | CH1-004 |

### Product Prices

| DATA ID | Product | Price |
|---------|---------|-------|
| D030 | Sauce Labs Backpack | $29.99 |
| D033 | Sauce Labs Bike Light | $9.99 |
| D036 | Sauce Labs Bolt T-Shirt | $15.99 |
| D039 | Sauce Labs Fleece Jacket | $49.99 |
| D042 | Sauce Labs Onesie | $7.99 |
| D045 | Test.allTheThings() T-Shirt (Red) | $15.99 |

---

## 📊 Execution Results

### Daily Progress

| Date | Day | TCs Executed | Passed | Failed | Cumulative Pass % |
|------|-----|--------------|--------|--------|-------------------|
| 2026-05-20 | Day 1 | 20 | 19 | 1 | 95% |
| 2026-05-21 | Day 2 | 30 | 28 | 2 | 94% |
| 2026-05-22 | Day 3 | 30 | 27 | 3 | 91% |
| 2026-05-23 | Day 4 | 25 | 23 | 2 | 92% |
| 2026-05-24 | Day 5 | 24 | 21 | 3 | 91.5% |
| **TOTAL** | | **129** | **118** | **11** | **91.5%** |

### Browser Compatibility

| Browser | Version | Pass Rate | Issues |
|---------|---------|-----------|--------|
| Chrome | 120 | 91.5% | None |
| Firefox | 121 | 90.7% | 1 additional UI issue |
| Edge | 120 | 91.5% | None |

### Special User Results

| User Type | Pass Rate | Key Issues |
|-----------|-----------|------------|
| standard_user | 100% | No issues |
| locked_out_user | 100% | Works as expected |
| problem_user | 60% | Images broken, tax wrong |
| performance_glitch_user | 100% | Slow but works |
| error_user | 41.7% | Checkout completely broken |
| visual_user | 87.5% | Text overlap |

---

## 📝 Recommendations

### Critical (Fix Before Production)

| Bug ID | Issue | Priority |
|--------|-------|----------|
| BUG-006 | error_user stuck on checkout step 1 | 🔴 Critical |
| BUG-011 | error_user cannot complete checkout | 🔴 Critical |

### High Priority (Fix Before UAT)

| Bug ID | Issue | Priority |
|--------|-------|----------|
| BUG-004 | Add to cart fails for error_user | 🟠 High |
| BUG-005 | Remove from cart fails for error_user | 🟠 High |
| BUG-008 | Incorrect tax for problem_user | 🟠 High |

### Medium Priority (Fix This Sprint)

| Bug ID | Issue | Priority |
|--------|-------|----------|
| BUG-001 | Product images missing for problem_user | 🟡 Medium |
| BUG-007 | Tax rounding error for 3+ items | 🟡 Medium |
| BUG-010 | problem_user wrong tax on full flow | 🟡 Medium |

### Low Priority (Fix Later)

| Bug ID | Issue | Priority |
|--------|-------|----------|
| BUG-002 | Text overlapping for visual_user | 🟢 Low |
| BUG-003 | Sorting resets after navigation | 🟢 Low |
| BUG-009 | visual_user text overlap | 🟢 Low |


## 📁 Repository Structure
