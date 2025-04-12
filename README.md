Bilkul bhai! Neeche tumhare liye ek **proper, clean, and GitHub-ready `README.md` file** likh diya hai for your project — `IIT Patna Multi-Modal Transportation Booking System`. Yeh file har section ko clearly explain karti hai, professional tone mein likhi gayi hai, aur easily samajh aati hai.

---

```markdown
# 🚆🚌✈️ IIT Patna Multi-Modal Transportation Booking System

A **C-based command-line application** developed to manage ticket reservations for **Trains**, **Buses**, and **Flights**, all in one place. This project includes a secure login system, dynamic seat management, PNR generation, and file-based data persistence.

> 🛠️ Developed by **Project P20 Team** for the **Problem Solving & Programming (PDS)** course at **IIT Patna**.

---

## 🔐 Key Features

| Feature                            | Status |
|------------------------------------|--------|
| User Signup / Login                | ✅     |
| Password Masking                   | ✅     |
| Captcha Verification               | ✅     |
| Train Ticket Booking               | ✅     |
| Bus Reservation System             | ✅     |
| Flight Reservation System          | ✅     |
| Unique PNR Generation for Flights  | ✅     |
| Ticket Cancellation                | ✅     |
| View Reserved Passengers           | ✅     |
| File-Based Record Storage          | ✅     |

---

## 🧩 Module Breakdown

### 🔒 `master.c` – Main Controller
- User login & signup system
- Password masking (******)
- Captcha verification for authentication
- Launches the selected booking service (Train / Bus / Flight)
- Saves login credentials in `login_data.txt`

### 🚆 `train.c` – Train Booking System
- Book/cancel train tickets
- View available trains and reserved passenger lists
- Static train list with route and charges
- Stores data in `train_data.txt`

### 🚌 `bus.c` – Bus Reservation System
- Book tickets by bus number and route
- Seat availability and route listing
- Reservation stored in `bus_reservation_data.txt`

### ✈️ `flight.c` – Flight Reservation System
- Choose from 20 international countries
- 50 seats per route limit
- Validates email and mobile numbers
- Generates unique 6-digit PNR
- Stores bookings in `passenger_records.txt`

---

## 📂 File Structure

```
📁 IIT_Patna_Transport_Booking_System
├── master.c                     // Main login & controller
├── train.c                      // Train booking module
├── bus.c                        // Bus booking module
├── flight.c                     // Flight booking module
├── login_data.txt               // Stores user credentials
├── train_data.txt               // Train passenger records
├── bus_reservation_data.txt     // Bus ticket data
├── passenger_records.txt        // Flight passenger data
├── README.md                    // Project documentation
```

---

## 🧪 How to Run

> 💻 **Requirements**: A C compiler like GCC

1. **Compile all modules**  
   Make sure all `.c` files are in the same directory.
   ```bash
   gcc master.c -o bookingSystem
   ```

2. **Run the system**
   ```bash
   ./bookingSystem
   ```

---

## 📌 Notes

- The program uses basic `file I/O` for data storage.
- Make sure the `.txt` data files exist (or will be auto-created after first run).
- Captcha must be entered correctly to proceed with login/signup.

---

## 👨‍💻 Developed By

**Project P20 Team**  
_Indian Institute of Technology, Patna_  
Course: Problem Solving & Programming (PDS)  
Semester: 2nd

---

## 📜 License

This project is for educational purposes only and not licensed for commercial use.
