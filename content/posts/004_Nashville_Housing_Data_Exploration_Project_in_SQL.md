---
title: "Nashville Housing Data Exploration Project in SQL"
date: 2024-04-14T17:41:52+12:00
draft: false
summary: "This SQL project focuses on exploring the Nashville housing dataset to clean and prepare the data for analysis. The dataset contains information about housing sales in Nashville, including property addresses, sale dates, and sale prices."
tags: ["SQL","data science", "data exporation","projects"]
author: "David Cardona"
showToc: true
TocOpen: true
hidemeta: false
comments: false
canonicalURL: "https://canonical.url/to/page"
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: false
ShowReadingTime: true
ShowBreadCrumbs: false
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: false
cover:
    image: "<image path/url>" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---
## Overview

This SQL project focuses on exploring the Nashville housing dataset to clean and prepare the data for analysis. The dataset contains information about housing sales in Nashville, including property addresses, sale dates, and sale prices.

Link to the project 👉
[Nashville Housing Data Exploration Project](https://github.com/davidcardonadev/Nashville_Housing_Data_Exploration_Project_in_SQL)


![picture_data_covid](/images/nashville.jpg)
*[Picture of Tanner Boriack](https://unsplash.com/es/fotos/estadio-de-futbol-americano-junto-al-edificio-y-la-carretera-durante-el-dia-GmoaEH48m8c?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash)*
  
## Objectives
- Standardize date formats for consistency.
- Populate missing property address data.
- Split address and owner address columns into individual components.
- Convert 'Y' and 'N' values in the 'SoldAsVacant' field to 'Yes' and 'No' for clarity.
- Remove duplicate records to ensure data integrity.
- Delete unused columns to streamline the dataset.

## Methodology
### 1. Standardizing Date Format
   - Identified and converted the 'SaleDate' column to a standardized date format.

### 2. Populating Missing Property Address Data
   - Identified and populated missing property address values based on ParcelID.

### 3. Splitting Address Columns
   - Split the 'PropertyAddress' column into 'Address' and 'City' columns.
   - Split the 'OwnerAddress' column into 'Address', 'City', and 'State' columns.

### 4. Updating 'SoldAsVacant' Field
   - Replaced 'Y' with 'Yes' and 'N' with 'No' in the 'SoldAsVacant' field for clarity.

### 5. Removing Duplicate Records
   - Identified and removed duplicate records based on selected criteria.

### 6. Deleting Unused Columns
   - Removed unused columns such as 'OwnerAddress', 'TaxDistrict', 'PropertyAddress', and 'SaleDate' to streamline the dataset.

## Key Findings
- Standardized date formats for consistency across the dataset.
- Populated missing property address data based on ParcelID.
- Split address columns into individual components for better analysis.
- Updated 'SoldAsVacant' field for clarity.
- Ensured data integrity by removing duplicate records.
- Streamlined the dataset by deleting unused columns.

## Conclusion
This project successfully cleaned and prepared the Nashville housing dataset for further analysis. By standardizing date formats, populating missing data, splitting address columns, updating field values, removing duplicates, and deleting unused columns, the dataset is now ready for in-depth analysis and insights.

--- 
**Colophon**  

thanks Alex for his tutorials and explanations ([Alex The Analyst](https://www.alextheanalyst.com/))