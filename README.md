# **iTunes Backup Explorer**
iTunes Backup Explorer is a desktop application that allows users to easily review iTunes backup files and view details of backup files. This Python and Tkinter-based tool analyzes backup files using SQLite databases and presents file structure, applications and device information to the user.
![image](https://github.com/user-attachments/assets/d24d12c1-2c9a-4ef5-a5bb-5a743bbc84ac)

## **Features**
Backup File Review: Easily load backup files and view the data within them.
File Search: File search function to quickly find specific files within backup files.
File and Application List: Listing backup files and applications with their real names instead of hash values.
Device Information: Shows the device information in the backup file.
User-Friendly Interface: A simple and intuitive interface to easily navigate through files and information.
## **Requirements**
Before running the project, make sure the following software is installed:

Python 3.8 or higher
Tkinter (comes with Python)
SQLite3 (comes with Python)
## **Installation**
To set up and run the iTunes Backup Explorer project on your local machine, follow these steps:

Prerequisites
Make sure you have the following installed:

Python 3.8+: Download Python
Git: Download Git
SQLite: Pre-installed with Python
Tkinter: Pre-installed with Python for GUI development
1. Clone the Repository
Clone the repository to your local machine using Git:
git clone https://github.com/edayigit/itunes-backup-explorer.git
cd itunes-backup-explorer

3. Create a Virtual Environment (Optional but recommended)
Create and activate a virtual environment to isolate the dependencies:

# On Windows
python -m venv env
env\Scripts\activate

# On macOS/Linux
python3 -m venv env
source env/bin/activate

3. Install the Required Dependencies
Run the following command to install the required Python libraries from the requirements.txt file:

pip install -r requirements.txt
This will install necessary packages like tkinterdnd2, Pillow, and others needed to run the project.

4. Set Up Manifest.db
Make sure you have a valid Manifest.db file from an iTunes backup. This file is essential for extracting real file names based on hash IDs. Place this file in a directory accessible to your project.

You can specify the path to your Manifest.db file within the code where necessary.

5. Run the Application
Start the application by running the main.py file:
python main.py
This will launch the GUI, allowing you to explore iTunes backup files, view file information, and perform search operations.

6. Icons Directory (Optional)
If you want to customize the look of the application with icons, place any required icons in the icons directory inside your project folder. Ensure that the paths in the code match the file locations.


Tabii, işte iTunes Backup Explorer projeniz için daha özenli yazılmış bir "Kullanım" bölümü:

## **Usage**
Once the iTunes Backup Explorer is up and running, you can use it to explore and analyze iTunes backup files. Below is a step-by-step guide to using the application's main features:

1. Opening a Backup File
Launch the application by running main.py.
Use the Upload button to load an iTunes backup file from your computer. The app will automatically extract device and backup information, which will be displayed in the Information section.
2. Viewing Device Information
Once the backup file is loaded.
This section displays essential details such as device model, iOS version, backup date, and more, all extracted from the Info.plist file of the backup.
3. Exploring Files
Click on the Files button to browse through the backup’s file system.
The app will show files in a structured view, categorized by folders such as Documents, AppData, etc.
File names will be displayed as their real names (instead of hashed names) by referencing the Manifest.db database.
4. Viewing Installed Apps
Navigate to the Apps section to see a list of installed applications from the backup.
This section will provide a detailed overview of app-related data stored within the backup.
5. Search Functionality
Use the search bar at the top of the app to quickly find files by name.
The search feature highlights and selects the exact file within the categorized structure, making it easy to locate specific files without manually browsing through each folder.
6. File Export
Once a file or app is selected, you can easily export it to a specified directory for further use or analysis.
This allows you to recover specific files from the backup and store them locally.
7. Handling Errors
If the application cannot locate certain files (e.g., icons or the Manifest.db file), it will notify you with an error message.
Double-check the file paths and ensure all necessary files are in the correct locations before proceeding.
Tips:
For optimal performance, ensure that the Manifest.db file from the backup is correctly placed and linked in the project. This is essential for displaying real file names.
You can add custom icons to enhance the UI by placing them in the icons directory.

## **License**
This project is licensed under the MIT License. By using this software, you agree to the following terms:
MIT License

Copyright (c) 2024 [Eda Yiğit]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
