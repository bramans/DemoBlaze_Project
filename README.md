# DemoBlaze Testing Toolkit Project

## 📌 Project Overview

This project is a **software testing assignment** built around the [DemoBlaze](https://www.demoblaze.com/) e-commerce platform.
It follows a full testing workflow, from **requirements analysis** to **JIRA migration** and **test automation**.

The project demonstrates:

* Writing **user stories** and acceptance criteria.
* Identifying **ambiguities/issues** in requirements.
* Designing **test scenarios and functional test cases**.
* Executing manual tests and logging defects.
* Performing **usability testing**.
* Preparing a **release report**.
* Designing a **regression testing strategy** for a new feature (product filters).
* Migrating artifacts to **JIRA** (with optional **Xray integration**).
* Automating **two regression test cases** using Selenium (Python).

---

## 📂 Project Structure

```
DemoBlaze_Project/
├─ Requirements_Analysis/
│  ├─ User_Stories.xlsx
│  ├─ User_Story_Issues.docx
├─ Test_Design/
│  ├─ Test_Scenarios.xlsx
│  ├─ Functional_Test_Cases.xlsx
├─ Testing_Execution/
│  ├─ Functional_Test_Report.docx
│  ├─ Defect_Logs.xlsx
├─ Usability_Testing/
│  ├─ Usability_Report.docx
├─ Release_Management/
│  ├─ Release_Report.docx
├─ Regression_Testing/
│  ├─ Regression_Strategy.xlsx
│  ├─ test_add_to_cart.py
│  ├─ test_place_order.py
├─ JIRA_Migration/
│  ├─ Bulk_Import_CSV.csv
│  ├─ Excel_to_JIRA_Traceability_Screenshot.png
```

---

## ⚙️ Setup Instructions

### 1. Install Requirements

Make sure Python 3.8+ is installed, then run:

```bash
pip install selenium webdriver-manager pandas openpyxl
```

### 2. Run Automation Scripts

Run the automated test cases from the `Regression_Testing/` folder:

```bash
python test_add_to_cart.py
python test_place_order.py
```

These scripts will:

* Add a product to the cart and verify it appears.
* Place an order as a guest and confirm the purchase dialog.

---

## 📑 Deliverables Summary

* **Requirements Analysis** → User stories & identified issues.
* **Test Design** → Test scenarios & test cases.
* **Testing Execution** → Functional test report & defect logs.
* **Usability Testing** → Usability issues report.
* **Release Management** → Release report (summary & readiness).
* **Regression Testing** → Strategy, test cases, automation scripts.
* **JIRA Migration** → CSV import file & traceability screenshot.

---

## 📌 JIRA Migration Notes

1. Use `JIRA_Migration/Bulk_Import_CSV.csv` to bulk import issues.
2. Map columns to JIRA fields (Issue Type → Story/Test, Summary → Summary, etc.).
3. If using **Xray**, map `Test Steps` column properly.
4. After import, link stories with their tests and export a **traceability screenshot**.

