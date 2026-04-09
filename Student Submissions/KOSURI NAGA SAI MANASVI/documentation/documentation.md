Data Cleaning Process
1. Removal of Irrelevant Columns

Unnecessary columns that were not required for analysis were identified and removed to improve dataset clarity and performance.
This was done using the “Remove Columns” option in Power Query.

2. Handling Missing Values

The dataset was checked for null or blank values.

Rows with missing values in critical columns such as State and Severity were removed.
In cases where appropriate, missing values were handled to ensure consistency.
3. Correction of Data Types

Each column was assigned the correct data type to ensure accurate calculations and visualizations.

Column Name	Data Type
State	Text
City	Text
Casualties	Whole Number
Number of Fatalities	Whole Number
Speed Limit	Whole Number
Date	Date
Time	Time

This was done using the “Data Type” option in Power Query.

4. Cleaning the Time Column

The “Time of Day” column contained values in an incorrect datetime format (e.g., 31-12-1899 00:05:00), where the date component was irrelevant.

Extracted only the time component from the column.
Removed the default date (1899) as it was not meaningful for analysis.

This ensured the column contained only valid time values.

5. Creation of Time Categories

A new column was created to categorize time into meaningful groups for analysis.

The categories used:

Dawn
Day
Dusk
Night

This was implemented using conditional logic based on time ranges.

6. Standardization of Categorical Values

Text-based columns such as Weather, Light Conditions, and Severity were checked for inconsistencies.

Corrected spelling variations
Ensured uniform naming conventions
Removed duplicates caused by inconsistent entries
7. Extraction of Date Components

The Date column was further processed to extract useful components:

Year
Month
Day
Day of Week

This enabled time-based analysis and filtering in the dashboard.

8. Validation of Day and Date Consistency

Ensured that the Day of Week matched the corresponding Date values.
Any inconsistencies were corrected to maintain data integrity.

9. Removal of Duplicate Records

The dataset was checked for duplicate entries.

Duplicate rows were identified and removed
Ensured each record represented a unique event
10. Final Data Verification

After all cleaning steps:

Data was reviewed for consistency and accuracy
Column names were standardized
Dataset was finalized for visualization and analysis in Power BI
