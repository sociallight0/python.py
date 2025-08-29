# File Read & Write Challenge with Error Handling Lab 🖋️🧪

A comprehensive Python program that demonstrates robust file operations with extensive error handling. This program combines the **File Read & Write Challenge** and **Error Handling Lab** into a single, powerful application.

## 🎯 Overview

This program creates a robust file processing system that can:
- Read files safely with comprehensive error handling
- Apply various modifications to file content
- Write modified content to new files
- Handle all types of file-related errors gracefully
- Provide detailed feedback and logging

## 🚀 Features

### Core Functionality
- **Safe File Reading**: Handles missing files, permission issues, encoding problems
- **Content Modification**: Multiple transformation options for file content
- **Secure File Writing**: Creates directories as needed, handles write permissions
- **Interactive Menu**: User-friendly interface for all operations
- **Error Logging**: Tracks and reports all errors encountered
- **Processing Summary**: Shows completed operations and error statistics

### File Modifications Available
1. **Word Count Analysis**: Adds detailed statistics (lines, words, characters)
2. **Uppercase Conversion**: Converts all text to uppercase
3. **Line Numbering**: Adds sequential line numbers to content

### Error Handling Coverage
- `FileNotFoundError`: File doesn't exist
- `PermissionError`: Insufficient read/write permissions
- `IsADirectoryError`: Attempting to read a directory as a file
- `UnicodeDecodeError`: Encoding/decoding issues
- `OSError`: General operating system errors
- `Exception`: Catch-all for unexpected errors

## 📁 Program Structure

```
file_processor.py
├── FileProcessor (Class)
│   ├── read_file()           # Safe file reading with error handling
│   ├── modify_content()      # Content transformation methods
│   ├── write_file()          # Safe file writing with error handling
│   ├── process_file()        # Complete processing pipeline
│   └── show_summary()        # Display processing results
├── create_sample_file()      # Generate test file
└── main()                    # Interactive user interface
```

## 🛠️ How to Use

### Running the Program
1. Save as `file_processor.py`
2. Run: `python file_processor.py`
3. Choose from the interactive menu options

### Menu Options
1. **Process an existing file**: Work with your own files
2. **Create sample file and process it**: Generate test content automatically
3. **View processing summary**: See results and error logs
4. **Exit**: Close the program

### Example Workflow
```
📋 MENU OPTIONS:
1. Process an existing file
2. Create sample file and process it
3. View processing summary
4. Exit

Enter your choice (1-4): 1
Enter the filename to process: my_document.txt

Modification options:
1. Add word count and statistics (default)
2. Convert to uppercase
3. Add line numbers

Choose modification type (1-3, default=1): 1
Enter output filename (press Enter for auto-generate): 

🔍 Attempting to read file: my_document.txt
✅ Successfully read 1250 characters from 'my_document.txt'
🔧 Applying modification: word_count
📝 Attempting to write to file: my_document_modified.txt
✅ Successfully wrote 1456 characters to 'my_document_modified.txt'
🎉 File processing completed successfully!
```

## 🔧 Sample Output Examples

### Word Count Analysis Output
```
=== FILE ANALYSIS REPORT ===
Generated on: 2025-08-30 14:30:15
Original file statistics:
- Lines: 12
- Words: 89
- Characters: 445
- Characters (no spaces): 378

=== ORIGINAL CONTENT ===
[Original file content follows...]
```

### Uppercase Conversion Output
```
=== UPPERCASE CONVERSION ===
Generated on: 2025-08-30 14:30:15
Original content converted to uppercase:

HELLO WORLD!
THIS IS A SAMPLE TEXT FILE...
```

### Line-Numbered Output
```
=== LINE-NUMBERED VERSION ===
Generated on: 2025-08-30 14:30:15

  1. Hello World!
  2. This is a sample text file for testing.
  3. It contains multiple lines of text.
```

## 🛡️ Error Handling Examples

### File Not Found
```
❌ File not found: File 'nonexistent.txt' does not exist.
```

### Permission Denied
```
❌ Permission denied: Cannot read 'protected_file.txt'. Check file permissions.
```

### Directory Instead of File
```
❌ Directory error: 'my_folder' is a directory, not a file.
```

### Encoding Issues
```
❌ Encoding error: Cannot decode 'binary_file.exe'. File may be binary or use different encoding.
```

## 📊 Processing Summary

The program tracks all operations and provides summaries:

```
==================================================
📊 PROCESSING SUMMARY
==================================================
Files successfully processed: 2
  ✅ sample_modified.txt
  ✅ document_analysis.txt

Errors encountered: 1
  ❌ File not found: File 'missing.txt' does not exist.
```

## 💡 Learning Outcomes

By using this program, you'll master:

### File Operations
- Reading files safely with proper resource management
- Writing files with directory creation
- Handling different file encodings
- Working with file paths and extensions

### Error Handling Techniques
- Try-catch blocks for specific exceptions
- Multiple exception handling in single block
- Custom error messages and logging
- Graceful degradation when errors occur

### Best Practices
- Resource management with context managers (`with` statements)
- User input validation
- Comprehensive error reporting
- Clean code organization with classes

## 🎓 Advanced Features

### Automatic Directory Creation
If the output path includes directories that don't exist, the program creates them automatically.

### Comprehensive Logging
All errors are logged with timestamps and detailed messages for debugging.

### Flexible Input Handling
- Auto-generates output filenames if not specified
- Handles empty inputs gracefully
- Validates user choices

### Cross-Platform Compatibility
Works on Windows, macOS, and Linux systems.

## 🔧 Requirements

- **Python Version**: 3.6 or higher
- **Dependencies**: Only built-in Python modules
- **Permissions**: Read access to input files, write access to output location

## 🎉 Success Indicators

After running this program, you'll have demonstrated mastery of:

✅ **Robust file reading** with comprehensive error handling  
✅ **Safe file writing** with automatic directory creation  
✅ **Content transformation** with multiple modification types  
✅ **User interaction** with input validation  
✅ **Error logging** and reporting systems  
✅ **Clean code organization** using classes and methods  

This program showcases the skills needed to build **strong, robust applications** that handle real-world file operations and unexpected issues gracefully! 🎊
