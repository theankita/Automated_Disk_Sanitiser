# Automated Disk Sanitiser

## Overview

Automated Disk Sanitiser is a Python-based automation tool that identifies and removes duplicate files from a specified directory. The application traverses directories, generates MD5 checksums for files, detects duplicates based on matching checksums, and deletes redundant copies while retaining one original file.

This project demonstrates the use of Python for file handling, hashing algorithms, directory traversal, and automation scripting.

---

## Features

* Directory traversal using `os.walk()`
* Duplicate file detection using MD5 hashing
* Automatic deletion of duplicate files
* Retains one original copy of each file
* Lightweight command-line utility
* Fast checksum-based file comparison
* Automated file management

---

## Technologies Used

### Programming Language

* Python

### Libraries & Modules

* os
* hashlib

### Concepts

* File Handling
* Directory Traversal
* Checksum Generation
* Duplicate Detection
* Automation Scripting
* File Management

---

## Project Structure

```bash
Automated_Disk_Sanitiser/
│
├── DiskSanitiser.py
│
└── README.md
```

---

## Workflow

Select Directory
↓
Traverse Files Using os.walk()
↓
Generate MD5 Checksum for Each File
↓
Store Checksums in Dictionary
↓
Identify Duplicate Files
↓
Delete Redundant Copies
↓
Display Total Deleted Files

---

## How It Works

### 1. Calculate File Checksum

The application reads each file in binary mode and generates an MD5 checksum.

```python
hashlib.md5()
```

Files with identical content produce the same checksum.

### 2. Directory Traversal

The program traverses the specified directory and its subdirectories using:

```python
os.walk()
```

### 3. Duplicate Detection

A dictionary is used to store file checksums and corresponding file paths.

```python
Duplicate[Checksum] = [filename]
```

If multiple files have the same checksum, they are considered duplicates.

### 4. Delete Duplicate Files

The program keeps the first file and removes all additional copies.

```python
os.remove()
```

### 5. Summary

After completion, the application displays:

* Names of deleted files
* Total number of duplicate files removed

---

## How to Run the Project

### Step 1: Clone Repository

```bash
git clone https://github.com/theankita/Automated_Disk_Sanitiser.git
```

### Step 2: Navigate to Project Directory

```bash
cd Automated_Disk_Sanitiser
```

### Step 3: Run the Script

```bash
python DiskSanitiser.py
```

---

## Sample Output

```text
Deleted file : D:\Documents\copy1.txt
Deleted file : D:\Documents\copy2.txt

Total deleted files : 2
```

---

## Learning Outcomes

This project demonstrates:

* Python Automation
* File Handling
* Hashing with MD5
* Dictionary-Based Data Storage
* Directory Traversal using os.walk()
* Duplicate File Detection
* Command-Line Application Development

---

## Future Improvements

* SHA-256 Based Hashing
* File Recovery Option
* Storage Space Saved Calculation
* Duplicate File Report Generation
* Graphical User Interface (GUI)
* Multi-threaded File Scanning

---

## Author

### Ankita Dnyanoba Shinde

GitHub:
https://github.com/theankita

**Project Type:** Python Automation & File Management Project
