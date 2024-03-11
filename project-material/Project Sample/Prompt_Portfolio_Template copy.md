# Prompt Portfolio

## Prompt ID:
FSL01-Enhanced

## Description:
This enhanced few-shot prompt provides multiple examples to generate Python code for filtering rows in a pandas DataFrame based on various conditions, aiming to improve the chatbot's ability to handle diverse data processing queries.

## Use Case:
Data Processing

## Prompt:
"Consider the following examples for filtering rows in a pandas DataFrame named `df`:
1. To select rows where the column `age` is greater than 30, use: `df[df['age'] > 30]`
2. To select rows where the column `status` is 'active', use: `df[df['status'] == 'active']`
3. To select rows where the column `score` is between 50 and 100, inclusive, use: `df[df['score'].between(50, 100)]`

Given these examples, how can I select rows where the column `salary` is greater than 50000?"

## Parameters:
Temperature: 0.4, Max Tokens: 200

## Sample Output:
"To filter rows in your DataFrame `df` where the `salary` column values are greater than 50000, you can use the following Python code: `filtered_df = df[df['salary'] > 50000]`."

## Adjustments:
The number of examples was increased to provide a more robust few-shot learning context, which helped in generating more accurate and specific Python code responses for a range of filtering conditions.

## Ethical Note:
Users should be aware of the potential for bias when filtering data and consider the ethical implications of their data processing decisions. It's essential to perform a comprehensive analysis to ensure that filtering does not inadvertently exclude important subsets of data that could affect conclusions.

## Version:
1.2, [Date]
