# README.md

# Superstore Sales Data Cleaning and Transformation using Power BI

## Project Overview

This project involves importing the **Superstore Sales CSV dataset** into **Power BI** and performing data cleaning and transformation using **Power Query Editor**.

The dataset was transformed to improve data consistency and prepare it for further analysis and dashboard creation.

---

## Dataset

**Dataset Name:** Superstore Sales Data
**Tool Used:** Microsoft Power BI
**Transformation Tool:** Power Query Editor

---

# Steps Performed

## 1. Imported the CSV File

The Superstore Sales CSV file was imported into Power BI using:

**Home → Get Data → Text/CSV**

The data was then opened in **Power Query Editor** for cleaning and transformation.

---

## 2. Promoted Headers

The first row of the dataset was converted into column headers.

**Applied Step:**

```text
Promoted Headers
```

This ensures that the dataset has proper column names.

---

## 3. Changed Data Types

The data types of columns were modified according to their values.

For example:

* Order Date → Date
* Ship Date → Date
* Segment → Text
* Category → Text
* Sub-Category → Text

**Applied Steps:**

```text
Changed Type
Changed Type with Locale
Changed Type with Locale1
```

Using **Locale** helps Power BI correctly understand the date format.

---

## 4. Standardized Text Formatting

The text values were formatted to maintain consistency.

The **Capitalize Each Word** transformation was applied to relevant text columns such as:

* Segment
* Category
* Sub-Category

**Applied Step:**

```text
Capitalized Each Word
```

Example:

```text
office supplies → Office Supplies
consumer → Consumer
home office → Home Office
```

---

## 5. Added Custom Columns

Custom columns were created using **Power Query transformations and M expressions**.

**Applied Steps:**

```text
Add Custom
Add Custom1
Add Custom2
Add Custom3
```

These custom columns were added to derive additional information from the existing dataset.

---

## 6. Duplicated Columns

Some existing columns were duplicated before applying transformations.

**Applied Steps:**

```text
Duplicated Column
Duplicated Column1
```

Duplicating columns helps preserve the original data while creating transformed versions.

---

## 7. Renamed Columns

The newly created or duplicated columns were renamed for better understanding.

**Applied Steps:**

```text
Renamed Columns
Renamed Columns1
```

This makes the dataset more organized and easier to use for analysis.

---

## 8. Calculated Week of the Year

A new column was created to calculate the **Week of the Year** from date values.

**Applied Steps:**

```text
Calculated Week of Year
Calculated Week of Year1
```

This transformation helps in performing weekly sales analysis.

---

## 9. Selected Required Columns

After completing the transformations, unnecessary columns were removed.

The final dataset contains the following important columns:

* Calculated Week of Year1
* Order Date
* Ship Date
* Segment
* Category
* Sub-Category

The Power Query formula used for selecting the columns is:

```powerquery
Table.SelectColumns(
    #"Calculated Week of Year1",
    {
        "Order Date",
        "Ship Date",
        "Segment",
        "Category",
        "Sub-Category"
    }
)
```

**Applied Step:**

```text
Removed Other Columns
```

---

# Final Data Transformation Process

```text
Import CSV File
        ↓
Promote Headers
        ↓
Change Data Types
        ↓
Apply Locale for Date Columns
        ↓
Capitalize Text Values
        ↓
Add Custom Columns
        ↓
Duplicate Required Columns
        ↓
Rename Columns
        ↓
Calculate Week of Year
        ↓
Remove Unnecessary Columns
        ↓
Final Cleaned Dataset
```

---

# Final Output

The Superstore Sales dataset was successfully cleaned and transformed using **Power Query in Power BI**.

The final dataset is prepared for:

* 📊 Data Analysis
* 📈 Sales Analysis
* 📅 Weekly Analysis
* 📉 Dashboard Creation
* 📊 Data Visualization

---

## Tools and Technologies Used

* **Microsoft Power BI Desktop**
* **Power Query Editor**
* **Power Query M Language**
* **CSV Dataset**

---

## Author

**Archana Devi M**

**Project:** Superstore Sales Data Cleaning and Transformation using Power BI
