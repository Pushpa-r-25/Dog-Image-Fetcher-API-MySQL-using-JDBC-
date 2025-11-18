# 🐶 Dog API Console Application with MySQL Integration

[![Java](https://img.shields.io/badge/Java-17-orange)](https://www.java.com/) 
[![MySQL](https://img.shields.io/badge/MySQL-8.0-blue)](https://www.mysql.com/)
[![License](https://img.shields.io/badge/License-MIT-blue)](LICENSE)

---

## **Introduction**  
The **Dog API Console Application with MySQL Integration** is a Java-based console application that interacts with the public [Dog API](https://dog.ceo/api/) and a local MySQL database.  

The application allows users to fetch dog breeds, sub-breeds, and random dog images from the internet, and store the retrieved information in a structured MySQL database for future reference.  

This project demonstrates integration of **API handling**, **JDBC connectivity**, and **file management** in Java.

---

## **Objectives**  
- Understand and implement interaction between a Java program and an external API.  
- Store real-time API data in a MySQL database using JDBC.  
- Gain hands-on experience with API communication, database operations, and data persistence.  
- Practice modular and maintainable Java programming.

---

## **Technologies Used**  
- **Programming Language:** Java  
- **Database:** MySQL  
- **API:** Dog CEO Public API ([https://dog.ceo/api/](https://dog.ceo/api/))  
- **Dependency Management:** Maven  
- **Libraries:** MySQL Connector/J, Gson (for JSON parsing)  

---

## **System Overview**  
The system provides a **menu-driven console interface** for users to interact with the Dog API and local database.  

- On program start, it checks the **MySQL database connection**.  
- Users can choose options to **view breeds**, **fetch images**, **save API data to the database**, or **store image URLs in files**.  
- The classes are modular:  
  - `DogAPIHandler` – Handles API calls.  
  - `DatabaseHandler` – Manages database storage.  
  - `SaveFile` – Handles file saving operations.

---

## **Modules Explanation**  

| File | Responsibility |
|------|----------------|
| `MainApp.java` | Main class controlling program flow and user menu. |
| `DatabaseHandler.java` | Handles database connectivity via JDBC and stores data in MySQL tables (`breeds`, `subbreeds`, `images`). |
| `DogAPIHandler.java` | Communicates with the Dog API to fetch breeds, sub-breeds, and random dog images. |
| `SaveFile.java` | Manages saving fetched image URLs into local text or CSV files for offline use. |

---

## **Program Flow**  
1. User runs the program; system checks database connectivity.  
2. Main menu appears with options:  
   - Access Dog API  
   - View Local DB  
   - Save API Data to DB  
   - Exit Application  
3. Accessing Dog API fetches real-time data such as breeds and images.  
4. Users can save image URLs to text or CSV files using `SaveFile`.  
5. Selecting **Save API Data to DB** fetches all breeds, sub-breeds, and image URLs and stores them in MySQL.  
6. Users can view stored data from the database using SQL queries.  
7. Process repeats until the user exits.

---

## **Sample Menu Output**  
