# Simple Data Filtering

Veda Technology intern task (AI & ML track).

## Description

Create a collection of student records and filter students based on marks, age, or department.

## Objective

Understand how conditions can be used to filter structured data.

## Tools

- Python 3
- Jupyter Notebook

## Files

- `simple_data_filtering.ipynb`: the notebook with the solution.
- `README.md`: this file.

## How to run

1. Install Jupyter if needed: `pip install notebook`
2. Start Jupyter: `jupyter notebook`
3. Open `simple_data_filtering.ipynb` and choose **Run All**.

## Approach

- Student records are stored as a list of dictionaries, with the fields `name`, `age`, `department`, and `marks`.
- A reusable function, `filter_students(records, condition)`, takes a condition (a function that returns True or False for one student) and returns the matching students.
- The filters use one condition (marks, department) and two conditions combined with `and` and `or`.
- A helper function prints each result with its count.

## Outcome

Running the notebook prints four filtered lists from the sample data:

| Filter | Students found |
|---|---|
| Marks >= 80 | 3 (Asha, Vikram, Sneha) |
| Department = CSE | 3 (Asha, Meera, Priya) |
| Marks >= 75 AND age <= 21 | 2 (Asha, Vikram) |
| Department = ME OR marks < 60 | 3 (Vikram, Sneha, Arjun) |

## Next steps

The sample records can be replaced with the Student Performance Dataset by loading it with pandas and converting each row into the same structure.
