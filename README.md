# SecureFileLoader Java Project

This folder contains a simple Java program that demonstrates safe failure when reading a file.

## Folder Structure

```text
Vulnerability_Ranking_Java_Assignment
├── data
│   └── example.txt
└── src
    └── SecureFileLoader.java
```

## How to Run in IntelliJ IDEA

1. Open IntelliJ IDEA.
2. Choose **Open** and select the `SecureFileLoader_Java_Assignment` folder.
3. Make sure the project is using **JDK 11 or higher**.
4. Open `src/SecureFileLoader.java`.
5. Go to **Run → Edit Configurations...**.
6. Select **SecureFileLoader** and set the **Working directory** to the inner project folder (the one that contains the `data` folder):
   `...\SecureFileLoader_Java_Assignment\Vulnerability_Ranking_Java_Assignment\Vulnerability_Ranking_Java_Assignment`
7. Click **Apply → OK**.
8. Click the green play button next to the `main` method.
9. Choose **Run 'SecureFileLoader.main()'**.


## Expected Output

```text
This is a test file.
The Java program is reading this file safely from the allowed data folder.
```

If the file is missing, unreadable, too large, or outside the allowed folder, the program prints:

```text
The file could not be read safely.
```

## Notes

The code reads only from the `data` folder. This prevents unsafe file access and helps demonstrate secure error handling.
