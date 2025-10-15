# 🎟 Ticket Reservation System

## 🧭 Overview
The *Ticket Reservation System* is a web-based and desktop-enabled application designed to efficiently manage *train ticket reservations. It offers users a smooth experience for **registration, login, train search, and booking management* through an intuitive interface.

The backend is powered by *Flask (Python)* and integrates seamlessly with both *Oracle* and *MySQL* databases for optimized data handling and reliability.

---

## 🚀 Key Features
- *User Registration:*  
  Allows new users to register by providing their username, password, phone number, and address.

- *Authentication System:*  
  Secure login functionality verifies user credentials with the database.

- *Booking Management:*  
  Users can search for available trains based on source and destination stations and make reservations easily.

- *Database Integration:*  
  - *Oracle Database* handles user and train schedule data.  
  - *MySQL Database* supports additional management and transaction details.

- *Multi-Interface Support:*  
  - *Web Interface:* Developed using HTML and CSS.  
  - *Desktop GUI:* Implemented using Tkinter for enhanced usability.

---

## 🧩 Technologies Used
| Component | Technology |
|------------|-------------|
| *Backend Framework* | Flask (Python) |
| *Databases* | Oracle (cx_Oracle), MySQL (mysql.connector) |
| *Frontend* | HTML, CSS, Tkinter |
| *Programming Language* | Python 3.x |

---

## 💻 Code Snippets

### 🔹 Backend Connection to Oracle
```python
import cx_Oracle

def connect_to_oracle():
    try:
        connection = cx_Oracle.connect('system/Srinivas17@XE')
        print("✅ Connected to Oracle Database")
        return connection
    except cx_Oracle.Error as e:
        print(f"❌ Error: {e}")
