# 🏦 Bank Management System

![Java](https://img.shields.io/badge/Java-OpenJDK%2023-orange?logo=java)
![GUI](https://img.shields.io/badge/GUI-Java%20Swing-blue)
![Database](https://img.shields.io/badge/Database-MySQL-lightgrey)
![Status](https://img.shields.io/badge/Project-Complete-brightgreen)

A **Java-based desktop banking application** built using **Java Swing**, **MySQL**, and **JDBC**. This system simulates core banking features such as user registration, deposit, withdrawal, and balance inquiry — all within a modern desktop GUI.

---


## 📸 Screenshots

Signup Form 

 ![Screenshot 2025-07-06 011724](https://github.com/user-attachments/assets/7b91407d-377f-46b4-a8c8-81c553c51452)
 Deposit Window
 
 ![Screenshot 2025-07-06 011757](https://github.com/user-attachments/assets/445e22ab-d554-4938-9c06-00c3748c85f0)


---

## 🚀 Features

- 👤 User Registration (3-step signup)
- 🔐 Secure Login & Authentication
- 💰 Deposit & Withdraw Functionality
- 📋 Balance Enquiry
- 🧾 Transaction History (Mini Statement)
- 🎨 Graphical User Interface (Java Swing)
- 🛢️ Data Storage with MySQL
- 📂 Modular File Structure for Scalability

---

## 🧱 Tech Stack

| Layer        | Technology               |
|--------------|---------------------------|
| 💻 Language   | Java (OpenJDK 23.0.1)     |
| 🖼 GUI        | Java Swing                |
| 🔗 DB Access | JDBC                      |
| 🗃 Database   | MySQL                     |
| 📦 JARs Used | `mysql-connector-java-8.0.28.jar`, `jcalendar-tz-1.3.3-4.jar` |

---

## 🗄️ Database Tables

### 🛢️ Database Setup

```sql
-- Create the database
CREATE DATABASE bankSystem;

-- Select the database
USE bankSystem;
-- Table: signup
CREATE TABLE signup (
  form_no VARCHAR(30),
  name VARCHAR(30),
  father_name VARCHAR(30),
  DOB VARCHAR(30),
  gender VARCHAR(30),
  email VARCHAR(60),
  maritial_status VARCHAR(30),
  address VARCHAR(60),
  city VARCHAR(30),
  pincode VARCHAR(30),
  state VARCHAR(30)
);
SELECT * FROM signup;

-- Table: signuptwo
CREATE TABLE signuptwo (
  form_no VARCHAR(30),
  religion VARCHAR(30),
  category VARCHAR(30),
  income VARCHAR(30),
  education VARCHAR(30),
  occupation VARCHAR(60),
  pan VARCHAR(30),
  aadhar VARCHAR(60),
  seniorcitizen VARCHAR(30),
  existing_account VARCHAR(30)
);
SELECT * FROM signuptwo;

-- Table: signupthree
CREATE TABLE signupthree (
  form_no VARCHAR(30),
  account_type VARCHAR(40),
  card_number VARCHAR(30),
  pin VARCHAR(30),
  facility VARCHAR(200)
);
SELECT * FROM signupthree;

-- Table: login
CREATE TABLE login (
  form_no VARCHAR(30),
  card_number VARCHAR(50),
  pin VARCHAR(30)
);
SELECT * FROM login;

-- Table: bank
CREATE TABLE bank (
  pin VARCHAR(10),
  date VARCHAR(50),
  type VARCHAR(50),
  amount VARCHAR(20)
);
SELECT * FROM bank;


---


## 🧩 Project Structure

```text
Bank-Management-System/
├── bank/
│   ├── management/
│   │   ├── system/
│   │   │   ├── Login.java
│   │   │   ├── Signup.java
│   │   │   ├── Signup2.java
│   │   │   ├── Signup3.java
│   │   │   ├── Deposit.java
│   │   │   ├── Withdrawl.java
│   │   │   ├── BalanceEnq.java
│   │   │   ├── FastCash.java
│   │   │   ├── Connn.java
│   │   │   └── main_Class.java
│   └── icon/ (UI images like ATM, bank logo)

## 🛠️ How to Run the Project

Follow these steps to run the **Bank Management System** successfully on your local machine.

---

### ✅ Prerequisites

- 💻 Java (OpenJDK 23 or compatible JDK)
- 🐬 MySQL Server
- 🛠️ IDE (IntelliJ IDEA / Eclipse / NetBeans)
- 📦 External JARs:
  - `mysql-connector-java-8.0.28.jar`
  - `jcalendar-tz-1.3.3-4.jar`

---

### 📁 Project Setup

1. **Clone the Repository**
   git clone https://github.com/aayusoni31/Bank-Management-System.git
2. **Open the Project in Your IDE**
   Launch your preferred Java IDE (e.g., IntelliJ IDEA, Eclipse, NetBeans)
3.**Open the cloned project folder as a new project**
    Add External JARs to the Project
    mysql-connector-java-8.0.28.jar
    jcalendar-tz-1.3.3-4.jar
4.**Set Java SDK**
    Make sure your project uses Java 17 or later
    Preferably use OpenJDK 23.0.1



After adding JARs and setting SDK, rebuild the project

Run a test file (e.g., Signup.java) to confirm setup works
