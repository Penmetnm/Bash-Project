This bash script is designed to analyze log files and extract specific information based on user-provided criteria. It's particularly useful for system administrators, developers, or anyone who needs to quickly parse and summarize log files.

## Features

1. **Flexible filtering**: The script allows users to filter log entries by date and severity level.
2. **Regular expression matching**: It uses regex to parse log entries, ensuring accurate extraction of information.
3. **Summary statistics**: The script provides a summary of the number of entries for each severity level.
4. **User-friendly output**: Parsed log entries are displayed in a readable format.

## Why it's useful

1. **Time-saving**: Quickly extract relevant information from large log files without manual searching.
2. **Customizable**: Users can easily modify the script to fit their specific log format or add additional filtering options.
3. **Error identification**: By filtering for specific severity levels (e.g., ERROR), users can quickly identify and address critical issues.
4. **Compliance and auditing**: Helps in generating reports for compliance requirements or system audits.

## Usage

```
./log_analyzer.sh [-h] [-d DATE] [-s SEVERITY] <log_file>
```

Options:
- `-h`: Display help message
- `-d DATE`: Filter logs by date (YYYY-MM-DD format)
- `-s SEVERITY`: Filter logs by severity (INFO, WARNING, ERROR)

Argument:
- `log_file`: Path to the log file to analyze

Example:
```
./log_analyzer.sh -d 2023-03-15 -s ERROR /var/log/application.log
```

This script provides a powerful and flexible tool for log analysis, making it easier to maintain and troubleshoot systems by quickly extracting relevant information from log files.
