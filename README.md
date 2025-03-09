# GitHub-Most-Popular-Repos-Analysis

## Project Overview

This project analyzes GitHub's most popular repositories using JSON files containing repository data based on different search terms. We use **Apache Spark** to process the data and store the results in an **SQLite database**. The goal is to extract meaningful insights such as:

1. **Most Used Programming Languages** - Number of repositories using each programming language.
2. **Organizations with the Most Stars** - Sum of stars across all repositories owned by an organization.
3. **Search Terms Relevance** - A custom relevance score based on forks, subscribers, and stars.

## Technologies Used

- **Google Colab** (for execution)
- **Apache Spark** (for processing JSON data)
- **SQLite** (for storing results)
- **PySpark** (for data processing)
- **Pandas** (for SQLite integration)

## Dataset

- The dataset consists of **30 JSON files**, each containing details about GitHub repositories.
- Each JSON file represents results for a specific search term.
- Schema of JSON files:
  ```
  |_corrupt_record|created|description|forks|full_name|id|language|open_issues|repo_name|stars|subscribers|topics|type|username|
  ```
  
## Running the Project

- Open **Google Colab** and run each step sequentially.
- Ensure that JSON files are uploaded before running the data processing steps.
- The final results will be stored in `github_repos.db` (SQLite database).

## Expected Output

- **`programming_lang`**** Table**: Shows how many repositories use each programming language.
- **`organizations_stars`**** Table**: Displays total stars per organization.
- **`search_terms_relevance`**** Table**: Ranks repositories based on calculated relevance scores.

## Contributing

Feel free to fork this repository and contribute improvements or new features. Suggestions are always welcome!


