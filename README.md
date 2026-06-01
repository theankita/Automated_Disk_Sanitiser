# Automated Disk Sanitiser

## Overview

Automated Disk Sanitiser is a Python-based automation tool designed to identify and remove duplicate files from a system. The application recursively scans directories, generates MD5 checksums for files, detects duplicates, and automatically deletes redundant copies to optimize disk storage usage.

This project demonstrates practical applications of file handling, hashing algorithms, automation scripting, and directory traversal in Python.

---

## Features

* Recursive directory scanning
* Duplicate file detection using MD5 hashing
* Automatic removal of redundant files
* Fast and lightweight execution
* Efficient storage optimization
* Simple command-line interface
* Automated file management

---

## Technologies Used

### Programming Language

* Python

### Libraries & Modules

* os
* hashlib
* File Handling

### Concepts

* Automation Scripting
* Directory Traversal
* Checksum Generation
* Duplicate Detection
* Storage Optimization
* File Management

---

## Project Structure

```bash
Automated_Disk_Sanitiser/
│
├── DiskSanitiser.py
│
├── README.md
```

---

## Workflow

Select Directory
↓
Recursive Directory Scan
↓
Generate MD5 Checksum
↓
Compare File Hashes
↓
Identify Duplicate Files
↓
Remove Redundant Copies
↓
Display Summary Report

---

## How It Works

### 1. Directory Scanning

The application recursively scans all files and subdirectories using:

```python
os.walk()
```

### 2. Checksum Generation

Each file is processed and assigned a unique MD5 checksum.

```python
hashlib.md5()
```

### 3. Duplicate Detection

Files with identical MD5 hashes are considered duplicates.

### 4. File Removal

The program preserves one original file and deletes all duplicate copies.

### 5. Reporting

After completion, the application displays:

* Total files scanned
* Duplicate files detected
* Files deleted
* Storage optimization summary

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
Scanning Directory...

Duplicate File Found:
photo_copy.jpg

Deleted Successfully

Total Files Scanned : 250
Duplicate Files Removed : 15
```

---

## Learning Outcomes

This project demonstrates:

* Python Automation
* File Handling
* Hashing Algorithms
* Directory Traversal
* Storage Management
* Command-Line Application Development

---

## Future Enhancements

* SHA-256 Based Duplicate Detection
* GUI Interface
* Recovery Bin for Deleted Files
* Duplicate File Report Generation
* Multi-threaded Scanning
* Storage Usage Analytics

---

## Author

### Ankita Dnyanoba Shinde

GitHub:
https://github.com/theankita

**Project Type:** Python Automation & File Management Project
