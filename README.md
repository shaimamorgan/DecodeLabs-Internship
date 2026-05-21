# DecodeLabs Internship – Project 1: Data Cleaning & Preparation

## 🎯 Project Objective
Transform a raw, messy sales dataset into a **production-ready "Gold Standard"** dataset by handling missing values, removing duplicates, and correcting data formats using **Microsoft Excel Power Query (Get & Transform)**.

## 🛠️ Tools Used
- Microsoft Excel (Power Query Editor)


## 📂 Files in this Repository
| File Name | Description |
|-----------|-------------|
| `Dataset for Data Analytics (Project 1).xlsx` | Raw original dataset (provided by DecodeLabs) |
| `Cleaned_Dataset_Shaima.xlsx` | Final cleaned dataset after all transformations |
| `Change Log (Project 1) - Shaima.pdf` | Documentation of every cleaning step with Change ID, Description, Impact, and Status |
| `Reference of Data Cleaning & Preparation.png` | Screenshot reference of the cleaning process |
| `Reference of Change Log.png` | Screenshot reference of the change log table |

## 🧹 Data Cleaning Steps Performed (in Power Query)

| Step | Action | Why? |
|------|--------|------|
| 1 | Removed duplicate `OrderID` rows | Ensures 0% error rate on unique identifiers |
| 2 | Changed `Date` column to **Date** data type (ISO 8601 ready) | Standardizes date format, removes time component |
| 3 | Rounded `UnitPrice` and `TotalPrice` to **2 decimal places** | Achieves required numeric precision |
| 4 | Trimmed whitespace from all text columns | Eliminates hidden leading/trailing spaces that break filters/lookups |
| 5 | Applied **Capitalize Each Word** (Proper Case) to `Product`, `ShippingAddress`, `PaymentMethod`, `OrderStatus`, `ReferralSource` | Standardizes text casing for consistent grouping and professional appearance |
| 6 | Left `null` values in `CouponCode` as is | Null represents "no coupon used" – deleting rows would corrupt integrity |

## ✅ Final Data Quality Checks
- No duplicate `OrderID` values
- All dates in valid date format (no timestamps)
- Numbers stored with exactly 2 decimal places
- No leading/trailing spaces in any text field
- Uniform capitalization across categorical columns
- Missing values only in `CouponCode` (intentional, valid business meaning)

## 📊 Procedures 
1. Open Excel → Data tab → Get Data → From Excel Workbook.
2. Select the raw dataset → Transform Data (Power Query Editor).
3. Apply the steps listed in the **Data Cleaning Steps Performed** table above.
4. Close & Load to a new worksheet.
5. Generate change log PDF as documented.



---

*Intern: Shaima Morgan*  
*Batch: 2026*  

