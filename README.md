# File Manager Script

This Python script automatically organizes files in a specified folder by moving them into subfolders based on their file extensions (e.g., images, documents, music, etc.).

## Features

- Automatically sorts files into folders like `Images`, `Documents`, `Music`, `Programs`, etc.
- Creates folders if they do not exist.
- Skips files with unknown extensions.

## Supported File Types

| Extension | Folder        |
|-----------|--------------|
| .gif      | Images       |
| .jpeg     | Images       |
| .jpg      | Images       |
| .png      | Images       |
| .webp     | Images       |
| .mp4      | Video        |
| .zip      | Compressed   |
| .mp3      | Music        |
| .pdf      | Documents    |
| .docx     | Documents    |
| .xlsx     | Documents    |
| .csv      | Documents    |
| .py       | Programs     |
| .exe      | Programs     |
| .ini      | System Files |
| .icc      | System Files |

## How to Use

1. **Install Python**  
   Make sure you have Python 3 installed on your system.  
   Download from: https://www.python.org/downloads/

2. **Download the Script**  
   Save the `file manager.py` file to your computer.

3. **Edit the Script**  
   Open `file manager.py` in a text editor (like VS Code).  
   Find this line at the bottom:
   ```python
   main_folder_path = r"add folder location"  # Update this to your folder
   ```
   Replace `"add folder location"` with the path to the folder you want to organize.  
   Example:
   ```python
   main_folder_path = r"C:\Users\YourName\Downloads"
   ```

4. **Run the Script**
   - Open Command Prompt (Windows).
   - Navigate to the folder containing `file manager.py`:
     ```
     cd "C:\Users\YourName\Path\To\Script"
     ```
   - Run the script:
     ```
     python "file manager.py"
     ```

5. **Check Results**  
   The script will print messages for each file it moves.  
   Your files will be organized into new folders inside the main folder.

## Notes

- The script only organizes files in the specified folder (not subfolders).
- Files with extensions not listed in the script will be skipped.
- You can add more extensions and folder mappings in the `extension_folders` dictionary.

## Example

**Before:**
```
Downloads/
├── photo.jpg
├── song.mp3
├── document.pdf
├── script.py
```

**After running the script:**
```
Downloads/
├── Images/
│   └── photo.jpg
├── Music/
│   └── song.mp3
├── Documents/
│   └── document.pdf
├── Programs/
│   └── script.py
```

---

**Feel free to modify the script to suit
