# Visualize Data with Amazon QuickSight

This README provides an overview of a project to analyze and visualize data using **Amazon QuickSight**, leveraging datasets stored in S3.

---

## What is Amazon QuickSight?

Amazon QuickSight is a powerful tool for:

- Analyzing large-scale data.
- Creating visualizations with a variety of graph types.

**Why use QuickSight?**

- Easy data manipulation with features like "select values," "group by," and "filters."
- Ideal for narrowing down data and generating meaningful insights.

---

## Project Overview

### Tools and Resources

- **Amazon S3**: For storing datasets.
- **Amazon QuickSight**: For visualizing data.

**Dataset Used**

- `netflix_titles.csv`
- `manifest.json` (describes bucket name and dataset).

---

## Steps to Visualize Data

### 1. Upload Files to S3

- Files uploaded: `manifest.json` and `netflix_titles.csv`.
- Edited `manifest.json` to include bucket name for correct data linkage.

### 2. Create a QuickSight Account

- Used **Enterprise Edition Free Trial** (ensured no charges by unchecking "Add Paginated Reports").
- Time taken: Less than 10 minutes.

### 3. Connect S3 to QuickSight

- Linked S3 bucket by navigating to **QuickSight -> S3 -> Paste S3 URI**.
- `manifest.json` directed QuickSight to the correct dataset.

### 4. Visualizations in QuickSight

- **Steps:**
  1. Selected a visual type (e.g., pie chart, bar graph).
  2. Dragged dataset fields to the Y-Axis, Values, and Group/Color columns.
- Example visuals:
  - Records released by year (pie chart).
  - Breakdown by year and type (horizontal bar graph).

### 5. Using Filters

- Applied filters for categories like:
  - "Action & Adventure"
  - "TV Comedies"
  - "Thrillers"
- Filters helped refine data for specific insights.

### 6. Setting Up a Dashboard

- Edited header graphs by double-clicking the header and using the editing window.
- Exported the dashboard as a **PDF** using the export tool.

---

## Updating Source Data

To ensure accuracy:

- Downloaded a new, complete dataset.
- Updated the S3 bucket with:
  - New CSV file.
  - Updated `manifest.json` file.

### Refreshing Data in QuickSight

- Went to **Datasets -> Dataset Analysis**.
- Verified the new data was uploaded, then refreshed the data view.

---

## Project Duration

- Total time for setup and analysis: Approximately 1 hour.
