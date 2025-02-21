# Inventory Management Application

## Overview
The **Inventory Management App** is an Android mobile application developed to allow users to create and manage their inventory. It will send the users a notification when the amount of an item is low in stock, and a text message if an item is deleted. This project was originally developed as part of the **CS-360: Mobile Architect & Programming** course at SNHU. It reflects key software design and engineering principles.

This repository documents the enhancements made to the app as part of **Category One Enhancement: Software Engineering and Design** for the **CS-499: Computer Science Capstone**. This enhancement aligns with the following course outcomes.

2. Design, develop, and deliver professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts.
3. Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution while managing the trade-offs involved in design choices.
4. Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals.
5. Develop a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources.

---

## Features

### **Original Project**
1. **Login and Sign Up Process**
    - Users are able to login or sign up for the app. If they do not have log in then they can sign up.

2. **Main Screen**
    - The app uses the RecylceViewer to display the user's inventory, if there is nothing in their inventory then they will be shown a No Data screen.

3. **Add Page**
    - Users are asked to enter the item infromation, if any infromation it will pass in default values of item name= 'No Name', sku= 'N/A' and amount=1. Once they press the Add Item button it will take them to the home page, now showing the item(s) added.
  
4. **Update/Delete Item Page**
    - The user can either update any or all values of the item or they can choose to delete it. Once the item is updated or deleted, the system will update the main page to reflect the changes.

5. **Delete All Function**
    - The user can select the three dots and select the delete all option. If the user deletes all of the entries the system will update and show the 'No Data' screen.

6. **SMS Notification**
    - The system has an SMS function that sends the user a text message anytime they update or delete an item. If the user has no phone number then there is no way for the user to recieve the messages.
      
### **Areas of Enhancement**
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

## Conclusion
The Inventory Management application after the enhancements offers a better user experince. The application has been updated to prevent sudden termination. Prior to the enhancements leaving a field blank in any field resulted in the app stopping. Through the creation of the InputValidation class the system prevents those errors. By updating the notification methods allows for a less intrusive user experience overall. Lastly the login/sign up process now allows users to log out if they want to, but ensures that they stay signed in even if they re-open the app. 

---

## Enhanced App Overview
A video overview can be watched on Youtube by going to this link: <a href="https://youtu.be/TxFq2dgIbdI" class="repo-button" target="_blank"> Inventory Management Overview Video </a>

## Screenshots
These images show the various pages the user can access through the use of the Inventory Management Application.

<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Login%20Screen.png" width="25%">
<p>Image that shows the systems login screen.</p>

<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Sign%20Up%20Screen.png" width="25%">
<p>Image that shows the systems sign up screen.</p>

<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Main%20Screen%20at%20Initialization.png" width="25%">
<p>This is a image of what the user will see from the home screen when the app is initialized for the first time and when they have no items in their inventory</p>

<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Add%20Item%20Screen.png" width="25%">
<p>This is a image of what the user will see from the Add Item screen when they press the floating action button</p>

<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Main%20Page%20with%20Item.png" width="25%">
<p>This is a image of what the user will see when there is an item or list of items in their inventory</p>

<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Update%20Screen.png" width="25%">
<p>This is a image of what the user will see when they want to update an item from their inventory</p>

<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Delete%20Item%20Confirm.png" width="25%">
<p>This is a image of what the user will see when they want to delete an item from their inventory. If they select yes then it will delete the entry from the inventory list</p>

<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Delete%20All%20Option.png" width="25%">
<p>This image shows the Delete All function that can be accessed from the main page</p>

<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Delete%20All%20Confirm.png" width="25%">
<p>This image shows the Delete All confirmation box. If the user selects yes then the main page will be empty and show the 'No Data' Message</p>

<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Notification.png" width="25%">
<p>This is an example of what a Low Inventory notification will look like if an item's amount is less than or equal to 1</p>

## Acknowledgements

This project was developed originally for **CS-360: Mobile Architect & Programming** and later enhanced in **CS-499: Computer Science Capstone** at SNHU. 
