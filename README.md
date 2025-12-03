# Advanced Shell Scripting: Pokémon API Automation

This project is a practical deep dive into Advanced Shell Scripting, focusing on automating interactions with a RESTful API (the Pokémon API). It simulates real-world DevOps and Data Engineering tasks where automation, reliability, and efficiency are paramount.

## Project Overview

The core of the project is to build a series of shell scripts that can:
- Fetch data from a public API.
- Process JSON responses.
- Handle errors and retries.
- Perform batch operations, both sequentially and in parallel.
- Generate summary reports from the collected data.

## Learning Objectives

By completing this project, you will demonstrate proficiency in:

- **API Interaction**: Making HTTP requests from the command line using `curl`.
- **JSON Manipulation**: Parsing, filtering, and extracting data from JSON responses using `jq`.
- **Text Processing**: Utilizing `grep`, `sed`, and `awk` to transform and format data.
- **Robust Scripting**: Implementing error handling, status checking, and retry logic.
- **Process Management**: Using shell job control (`&`, `wait`, `kill`, `jobs`) to run tasks in parallel.
- **Data Reporting**: Aggregating data and generating structured reports in CSV format.
- **Modular Design**: Structuring scripts to be maintainable and adaptable.

## Tools and Concepts

- **`curl`**: For making HTTP GET requests to the Pokémon API.
- **`jq`**: For parsing and manipulating JSON data from the API responses.
- **`awk`**: For text extraction, report generation, and calculations.
- **`sed`**: For stream editing and text transformations.
- **Core Shell Utilities**: Loops, conditionals, functions, and process control.

## Project Structure

The project is located in the `Advanced_shell/` directory and is composed of the following scripts:

- **`apiAutomation-0x00`**: Fetches data for a single Pokémon (Pikachu) and saves it to `data.json`.
- **`data_extraction_automation-0x01`**: Parses `data.json` to extract and display key stats in a human-readable format.
- **`batchProcessing-0x02`**: Fetches data for a list of Pokémon sequentially, with robust error handling and retry logic.
- **`summaryData-0x03`**: Reads the data files from the batch process, generates a `pokemon_report.csv`, and calculates average height and weight.
- **`batchProcessing-0x04`**: A more advanced version of the batch script that fetches Pokémon data in parallel to improve performance.