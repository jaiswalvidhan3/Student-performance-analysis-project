# Student Performance Analytics Engine

Subject: Essentials of AI

## About
Analysis of a 500 x 6 marks matrix (500 students, 6 subjects) using NumPy. It finds subject and student statistics, flags outliers and ranks the students.

## What it does
1. Imports, sets a seed and generates the marks matrix
2. Finds sum, mean, median, std and var with axis=0 (per subject) and axis=1 (per student)
3. Calculates z-scores using broadcasting, flags outliers and ranks students
4. Adds total and rank columns with hstack and exports a CSV using files.download

## How to run
1. Open `Student_Performance_Analytics.ipynb` in Google Colab
2. Click Runtime > Run all
3. The CSV file `student_marks.csv` downloads at the end

Only NumPy is used.

## Notes
- Marks are random (normal distribution, mean 65, std 15) and clipped between 0 and 100. The seed keeps them the same on every run.
- A mark is an outlier if its z-score is above 2 or below -2.
- Rank 1 is the student with the highest total.
- `files.download` only works in Colab. On a normal Jupyter setup, remove that line and the CSV is still saved in the working folder.

## Files
- `Student_Performance_Analytics.ipynb`: the notebook
- `README.md`: this file
