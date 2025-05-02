==================================================================================================================
CIT383 – Scripting 1 
Final Project – Comprehensive System Administration Check
Group 1 – Spring 2025
==================================================================================================================
Group Members:
- Dustin Morris
- Luke Mokas
- Brianna Deami
- Aaron Dube
==================================================================================================================
Team Contributions by Section:
1. Dustin Morris - User Requirements Analysis & Pseudocode Design
- Translated project requirements into clear, step-by-step pseudocode  
- Provided structure for each function in the system (user creation, deletion, etc.)  
- Ensured logic clarity for development and testing phases

2. Luke Mokas - User Management
- Implemented `--create`, `--delete`, `--update`, and `--create-batch` functionality  
- Integrated CSV batch user creation with validation  
- Applied role-based access for `admin` and `user` roles  
- Used subprocess commands to interface with system user management

3. Brianna Deami - Directory and File Management
- Built tools to organize files by type within a given directory  
- Created folders such as `/text_files`, `/image_files`, etc., as needed  
- Moved files based on extension with appropriate error handling

4. Dustin Morris - System Health Monitoring 
- Monitored system performance for 10 minutes at 1-minute intervals  
- Tracked CPU and memory usage  
- Triggered alerts for high usage 
- Logged all findings to `system_health_group_1.log` for review

5. Aaron Dube - Security and Error Handling
- Developed centralized error and info logging to `error_log_group_1.log`  
- Designed global input validation functions (for username, role, password, etc.)  
- Implemented error messages matching project examples  
- Ensured safe handling of sensitive or malformed input across all scripts

6. All Members - Code Documentation and ReadMe
- Made sure all code was commented before every function
- Collaborated to create README file

Overview:
This project is a Python-based system administration tool designed for CentOS 9. It allows administrators to automate a range of tasks through command-line subcommands. The script supports:
- Creating, deleting, and updating user accounts
- Adding multiple users from a CSV file
- Organizing files by type into categorized folders
- Monitoring system CPU and memory usage with logging
- Checking disk space and alerting on high usage
- Backing up and optionally encrypting files
- Centralized error and info logging with timestamps

All key events and errors are logged in `error_log_group_1.log`.

Usage Instructions:
Run the script from the terminal using ./sys_admin-group-1.py. along with any options and subcommands. 


Dependencies:
- Python 3
- Standard Python libraries:
  - logging
  - sys
  - re
  - os
  - pwd
  - argparse
  - subprocess
