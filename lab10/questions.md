
# Worksheet for Lab 10

### Question 1: What happens when you swap the delimiter from commas to tabs? How does the preview change?

When I change the delimiter from commas to tabs, the data no longer separates correctly into different columns. Instead, multiple values appear together in one column because the file uses commas to separate the data. When I change it back to commas, the preview shows the information in the correct columns again.

### Question 2: Try sorting the scientificName facet by name and by count. What problems are there with the data?

The scientificName column contains spelling errors and inconsistent formatting. Some names have extra spaces, and some species are spelled differently even though they refer to the same species. For example, Ammospermophilis harrisi and Ammospermophilus harrisi are incorrect variations of Ammospermophilus harrisii. These differences cause OpenRefine to count the same species as separate values, which makes the data inaccurate. We can fix this by removing extra spaces and correcting the misspelled names.

### Question 3: Use faceting to figure out the following:

**How many different years are represented in this file?**

There are 16 different years represented in the dataset.

**What year occurs the most times?**

The year 1978 occurs the most, appearing 237 times in the dataset.

**What year occurs the least number of times?**

The year 1993 occurs the least, appearing only 1 time in the dataset.

# Questions for Post-Lab Assignment 10

### Question 4: What happens when you make a numerical facet of column note1, then convert the column to numbers? Is something different about the facet compared to yr?

When I first created a numerical facet for the note1 column, OpenRefine showed "No numeric value present" because the values were stored as text. After converting the column to numbers, a histogram appeared showing values from 1 to 14. The facet showed 275 numeric values, 515 blank values, and no errors or non-numeric values. This is different from the yr column because note1 has many missing values, while yr contains years that can be displayed as numbers. The histogram helps us see the numerical values and identify missing data that may need cleaning.

### Question 5: Click and drag on the scatterplot facet you made to highlight a rectangle. What happens to the data points being displayed?

When I click and drag to highlight a rectangle on the scatterplot, OpenRefine filters the dataset to show only the data points inside the selected area. The rows outside the selected range are temporarily hidden. This allows me to focus on a smaller group of records and look for patterns or unusual values. I can change or remove the selection to see all the data points again.

### Question 6: After the last step, some columns are empty. (You can check by text faceting a column.) Why? What do you think we can do to fix it?

Some columns are empty because the scientificName column has extra spaces and inconsistent formatting. When OpenRefine splits the names into separate columns, these spaces can create blank cells. We can fix this by trimming extra whitespace, removing repeated spaces between words, and splitting the column again. We can also use a text facet to find any remaining blank values. This makes the data cleaner and more consistent.
