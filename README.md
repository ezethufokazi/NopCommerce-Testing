# nopCommerce Demo Store Testing

## Project Overview
This QA project contains test cases, test execution results, and bug reports for the nopCommerce demo store (https://demo.nopcommerce.com/). The tests validate key functionality including registration, login/logout, product browsing, shopping cart, checkout, account management, site navigation, footer links, sitemap, currency selection, and newsletter subscription.

---

## Tools Used
- **Test Management:** Microsoft Excel
- **Bug Tracking:** Excel Bug Report
- **Browser:** Chrome (latest version)
- **OS:** Windows 11
- **Screenshot Tool:** Snipping Tool

---

## Test Scope
- **User Registration & Authentication:** Register, login, password recovery, input validation
- **Product Browsing & Interaction:** Home page, top menu, PDP, wishlist, shopping cart, add to cart
- **Checkout Process:** Guest and logged-in checkout, billing/shipping addresses, shipping/payment methods, order confirmation
- **Account Management:** Customer info, addresses, orders, recurring payments, downloadable products, back in stock subscriptions, reward points, password change, product reviews
- **Navigation & Links:** Sitemap, header, footer, social media icons
- **Additional Features:** Currency change (USD/Euro), RSS, newsletter subscription

---

## Test Summary

| Total Test Cases | Passed | Failed | Blocked | Pass Rate |
|---|---|---|---|---|
| 258 | 243 | 6 | 9 | 94.2% |

---

## Bug Report Summary

| Bug ID | Description | Severity | Priority |
|---|---|---|---|
| NC_BUG_001 | Registration allows numeric and special characters in First Name and Last Name fields | Medium | P1 (Medium) |
| NC_BUG_002 | Sample download fails when clicking Download sample button | Medium | P1 (Medium) |
| NC_BUG_003 | Shipping & returns page displays placeholder text instead of actual content | Low | P2 (Low) |
| NC_BUG_004 | Privacy notice page displays placeholder text instead of actual content | Low | P2 (Low) |
| NC_BUG_005 | Conditions of Use page displays placeholder text instead of actual content | Low | P2 (Low) |
| NC_BUG_006 | About Us page displays placeholder text instead of actual content | Low | P2 (Low) |

---

## Test Case Structure
Each test case includes:
- TC ID
- Test Scenario
- Pre-requisites
- Test Steps
- Test Data
- Expected Result
- Actual Result
- Status (Pass/Fail/Blocked)
- Comments

Blocked test cases are documented but not included in bug reports.

---

## Bug Report Structure
Each bug report includes:
- Bug ID
- Title/Description
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Priority
- Screenshot

Failed test cases link to their corresponding bug report via Bug ID. Blocked test cases are noted separately with a reason.

---

## Test Environment
- **OS:** Windows 11
- **Browser:** Chrome (latest version)
- **URL:** https://demo.nopcommerce.com/
- **User Account:** Test accounts created in the application

---

## Repository Structure
```
nopCommerce-Testing
├── README.md
├── NopCommerce_TestCases.xlsx
├── NopCommerce_TestExecutionResults.xlsx
├── NopCommerce_BugReport.xlsx
└── Screenshots/
    ├── NC_BUG_001_Invalid_Input.png
    ├── NC_BUG_001_Registration_Success.png
    ├── NC_BUG_002_Sample_Download_Error.png
    ├── NC_BUG_003_Shipping_Returns_Placeholder.png
    ├── NC_BUG_004_Privacy_Notice_Placeholder.png
    ├── NC_BUG_005_Conditions_of_Use_Placeholder.png
    └── NC_BUG_006_About_Us_Placeholder.png
```

---

## Notes
- Single quotes are used for page names, buttons, and fields throughout the test cases.
- Mandatory fields, invalid inputs, and navigation links were tested thoroughly.
- Some features (recurring payments, downloadable products) are blocked due to lack of available products in the demo store.
- RSS link opens raw XML which is technically correct behaviour for an RSS feed but may appear broken to non-technical users.
