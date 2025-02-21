# Animal Database and Dashboard

## Overview
The **Animal Database and Dashboard** is a involves a python script that creates, reads, updates, and deletes information from the Animal MongoDB database. It also has a dashboard that retrieves data from the database and displays it on a datatable along with a pie chart of the animals by breed, and a map with the location of the first animal. It also includes a README file for the stakeholders so they may reproduce the system or install it. The enhancements align with industry best practices for scalable and efficient database solutions while improving the system's usability, scalability, and maintainability.

This repository documents the enhancements made to the system as part of **Category Three Enhancement: Databases** for the **CS-499: Computer Science Capstone**. This enhancement aligns with the following course outcomes.

1. Employ strategies for building collaborative environments that enable diverse audiences to support organizational decision-making in the field of computer science.  
2. Design, develop, and deliver professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts.  
3. Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution while managing the trade-offs involved in design choices.  
4. Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals.

---

## Features

### **Original Project**
The original project was created on Linux, and used the MongoDB dashboard to create the animal database. The driver class and dashboard were created using Jupyter Notebook to run the system.
1. **MongoDB Database**
    - The animal database was created using the command prompt, and was managed using the command line.
2. **Python Driver Class**
    - Drier class that is used to connect to the animal database, and has the create, read, update, and delete functions.
3. **DASH Dashboard**
    - The dashboard is created using DASH. It consists of a interactable datatable, a pie chart, and a map with the location of the first animal in the data table.

### **Enhancment(s)**
1. **Re-create the MongoDB Database**
    - Created the animal database by using MongoDB Compass, which allowed for easier management of the database.
2. **Testing and Error Handling**
    - A testing class was created to ensure proper functionality of the system, as well as added error handling to the driver class to ensure the system would notify users of any issues.
3. **Dashboard Visual Improvements**
    - Updated the dashboards layout to have a better design, while also adding filter options to the data table.
---

## Portfolio Content

- **Source Code**
    - 'Original Linux Project Files': Files needed to run the project on a Linux system.
    - 'Enhancement Three Project Files': Files needed to run the project on a Window system.
- **Documentation**
    - 'Original README Linux': System documentation explaining how to install the system on Linux.
    - 'Enhancement Three README Windows': System documentation explaining how to install the system on Windows.
    - 'Enhancement Three Narrative': Narrative explaing the enhancements, and how they aigned with the course outcomes.
---

## How to install/run

1. Dowload the zip file to your local machine, and unzip it
2. Open the project in **Visual Studio**
3. Follow README document to complete necessary dependencies installation
4. Run the Dashboard.ipynb file and click on the link produced to view the dashboard
---
## Screenshots

<img src="https://github.com/jcervantesortiz1/SNHU-Capstone/blob/main/Images/Enhancement%203%20Dashboard.png" width="100%">
<p>This image shows users what they will see once the system dashboard is initiated. There is an interactable data table, a pie chart, and a map with the location of the first item in the table</p>

## Conclusion
The Grazios Salvare Dashboard is now able to be accessed on a Windows device. Through the use of the new testing class we can ensure that the database connections are done properly. The systems README documentation is also updated to ensure users are able to install it on their local system. Furthermore since the dashboard only has access to retrieve data from the database, there are no security threats.
## Acknowledgements

This project was developed originally for **CS-340: Client/Server Development** and later enhanced in **CS-499: Computer Science Capstone** at SNHU. 
