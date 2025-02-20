# Inventory Management Application

## Overview
The **Inventory Management App** is an Android mobile application developed to allow users to create and manage their inventory. It will send the users a notification when the amount of an item is low in stock, and a text message if an item is deleted. This project was originally developed as part of the **CS-360: Mobile Architect & Programming** course at SNHU. It reflects key software design and engineering principles.

This repository documents the enhancements made to the app as part of **Category One Enhancement** for the **CS-499: Computer Science Capstone**. This enhancement aligns with the following course outcomes.

2. Design, develop, and deliver professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts.
3. Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution while managing the trade-offs involved in design choices.
4. Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals.
5. Develop a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources.

---

## Features

### **Original Project**
1. **Login and Sign Up Process**
    - Users can sign up and log in, but any time the app is closed and re-opened it has them log in again. They dont stay signed in.

2. **Log Out**
   - There is no way for the user to log out, they have to close the app and re-open it to be logged out.

3. **Notification(s)**
   - The system sends the user a text message (if they allow the permission) any time they update an item or delete an item.
  
4. **Input Validation**
    - There is no input validation, which causes the app to crash if the users leaves a field blank when adding or updating an item.

### **Enhancment(s)**
The below enhancements were implemented to improbe usability, stability, and security:

1. **Login and Sign Up Process**
    - Addeed the Android Session Manager to save a user profile once they have successfully logged in. This makes it so that once the user re-opens the app they will be taken to the main page.

2. **Log Out**
    - On the main page there is now a log out button. When the log out button is pressed it will clear the user profile saved to the session manager. They will then be taken back to the log in page. If the user re-opens the app it will bring them to the log in page.

3. **Notification(s)**
    - System will send the user a POST notification when an item's amount is less than or equal to 1.
    - An SMS message will be sent to the phone number on the device if an item is deleted.

---

## Portfolio Content
- **Source Code**
    - 'Original Android Source Files': Files needed to run the original project on the Android Studio IDE
    - 'Enhancement One Android Source Files': Files needed to run the enhanced project on the Android Studio IDE
- **APK**
    - 'Original APK': APK file to run the original project on an Android Mobile Device (Requires Android 14 or newer)
    - 'Enhanced APK': APK file to run the enhanced project on an Android Mobile Device (Requires Android 14 or newer)
- **Screehshots**
    - Visuals of the app's functionalities, and design
- **Documentation**
    - Narrative explaining the enhancements, and how they aligned with the course outcomes listed

---

## How to install/run
### PC
1. Dowload the zip file to your local machine, and unzip it.
2. Open the project in **Android Studio**.
3. Connect a physical device or set up an emulator.
4. Build and run the project.

### Mobile
1. Download APK file onto device
2. Find the file in the File Manger application
3. Allow 'Install Unkown Resources"
4. Click Install
5. Open

---
## Screenshots

## Acknowledgements

This project was developed originally for **CS-360: Mobile Architect & Programming** and later enhanced in **CS-499: Computer Science Capstone** at SNHU. 
