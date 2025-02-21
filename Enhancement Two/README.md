# Grazioso Salvare Pet Management System

## Overview
The **Grazioso Salvare Pet Management System** is a Java based system that gives various users the ability to add a dog or monkey to the system. The user is also able to reserve an animal, see all the animals in the system, and remove animals from the system. This project was originally developed as part of the **IT-145: Foundation in Application Development** course at SNHU. It reflects key algorithmic and structural principles.

This repository documents the enhancements made to the app as part of **Category Two Enhancement: Algorithms and Data Structures** for the **CS-499: Computer Science Capstone**. This enhancement aligns with the following course outcomes.

3. Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution while managing the trade-offs involved in design choices.

4. Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals.
---

## Features

### **Original Project** 
1. **Class Structure**
    - All of the system logic is in the Driver.java class as well as the main method.
      
2. **Insecure Coding**
     - There is nothing to prevent invalid data to be passed in. Things like empty lines, and invalid characters will cause the system to crash.
       
3. **ArrayList Data Storage**
     - There are two ArrayLists to hold the dog and monkey objects. The system must itterate through the entire ArrayList when searching for an animal.

### **Enhancment(s)**
1. **Updated Class Structure**
    - Moved all of the system logic to a new Logic.java class, leaving only the main method and the menu method in the Driver.java class.
2. **Secure Coding**
    - Added secure coding practices to ensure that the system doesn't crash when an invalid character is input.
3. **Updated to a HashMap Storage System**
    - Updated the system to use a HashMap that uses the Name as the key. This means that each animal must be uniquely named.
      
---

## Portfolio Content
- **Source Code**
    - 'Original Project File': Contains the original project files
    - 'Enhancement Two Project File': Contains the enhanced project files
- **Screenshots**
    - Visuals of the programs functionalities
- **Documentation**
    - Narrative explaining the enhancements, and how they aligned with the course outcomes listed.
---

## How to install/run
1. Download project zip file
2. Unzip
3. Open Eclipse IDE and run the Driver.java file
   
---
## Screenshots
<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Enhancement%202%20Updated%20Data%20Structure.png" width="100%">
<p>This is the updated class structure for the system. It consists of five total classes, with the main method being in the Driver class.</p>

## Acknowledgements

This project was developed originally for **IT-145: Foundation in Application Development** and later enhanced in **CS-499: Computer Science Capstone** at SNHU. 
