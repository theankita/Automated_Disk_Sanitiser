Automated Disk Sanitizer

A Python-based automation tool that recursively scans directories, detects duplicate files using MD5 checksum hashing, and removes redundant copies to optimize disk storage.

>Features

Recursive directory scanning using os.walk()

Duplicate detection using MD5 hashing

Automatic removal of redundant files

Lightweight and fast execution

Simple and easy-to-use script

>Tech Stack

Python

OS Module

Hashlib (MD5)

File Handling

Automation Scripting

>How It Works

The program scans the given directory recursively.

Each file’s MD5 checksum is calculated.

Files with identical checksums are identified as duplicates.

All redundant copies (except one original file) are deleted.

Total deleted file count is displayed.
