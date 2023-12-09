# EditElf

# Overview
EditElf is a text editing and spell-checking application written in Java. It offers a user-friendly interface for loading, editing, and saving text files, along with spell-checking capabilities for the content.（CS2212  Shuqi Liang, Jingpeng Ruan(Alan Ruan))
 
<img width="338" alt="811263dd865a8a009c9c9afa6499d78" src="https://github.com/Cheskaqiqi/EditElf/assets/109261504/4f01b8e1-ae45-47ab-bad0-a1750e70882e">

## Running the Application

You can run it by following these steps:

1. Run the `Application.java` file which serves as the entry point of the application. This can be done through an IDE.

#### File Operations

- **Open Files:** Use the file menu to load text files for spell checking.
- **Save Files:** Corrected text can be saved back to the file system.
- **User Dictionary Management:** Manage custom words in the user dictionary through `SettingUserDictionary.java`.

#### Spell Checking and Corrections

- **Initialization:** `CheckUtils.initWordData()` loads the standard dictionary for spell checking.
- **Spell Checking:** The application highlights spelling errors in the loaded text.
- **Error Types:** Different types of errors (misspelled words, mis-capitalizations, double words, etc.) are identified.
- **Suggestions:** Suggests corrections for identified errors, which can be manually applied.
- **Custom Corrections:** Users can add words to the user dictionary, affecting future spell checks.

#### Text Editing Features

- **Word Editing Operations:** Includes deletion, transposition, alteration, insertion, and appending of characters in words.
- **Special Case Handling:** Recognizes and handles special abbreviations like "Dr", "Mr", "Mrs", etc.
- **Mixed Case Handling:** Detects and corrects words with mixed upper and lower case letters.

#### Error Reporting

- **Error Information:** `ErrorInfo.java` stores details about each identified error, including its type and location in the text.
- **Error Display:** Errors are displayed in the GUI, allowing users to understand and correct them.

#### User Dictionary
<img width="340" alt="d7f9cd4a489175929326eec7addc091" src="https://github.com/Cheskaqiqi/EditElf/assets/109261504/41d0df0c-dc9d-4f43-9da1-d37b26de6585">

- **Reading and Writing:** `FileUtils.java` handles reading from and writing to the user dictionary.
- **Customization:** Users can add or remove words, tailoring the spell checker to their specific needs.

#### Additional Utilities

- **Text Processing:** Provides functions for splitting text and removing unwanted characters or labels.
- **Double Word Check:** Identifies and allows correction of repeated words.

#### Interacting with the Application

- The GUI is designed for easy navigation, with clear menus and buttons for each function.
- Users can interact with the text area to apply corrections and view error reports.

## Technology Stack

- Java: The application is primarily written in Java, ensuring cross-platform compatibility.

- Swing: Used for creating the graphical user interface.

