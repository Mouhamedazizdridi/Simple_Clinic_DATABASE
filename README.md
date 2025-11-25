# 🏥 Simple Clinic Database – Relational Schema

This project contains a relational database schema for a **Simple Clinic Management System**, designed based on the requirements provided.  
The goal is to model patients, doctors, appointments, medical records, prescriptions, and payments in a clean and normalized relational structure.

---
![Clinic Relational Schema](clinic_relational_schema.png)


## 📌 Project Overview

The database schema supports the following core functionalities:

### 👨‍⚕️ Doctors
- Each doctor has:
  - Unique identifier
  - Name
  - Specialization
  - Date of birth
  - Gender
  - Contact information (phone, email)
  - Address

### 🧑‍⚕️ Patients
- Each patient has:
  - Unique identifier
  - Name
  - Date of birth
  - Gender
  - Contact information (phone, email)
  - Address

### 📅 Appointments
- Each appointment includes:
  - Unique identifier
  - Patient (FK)
  - Doctor (FK)
  - Appointment date & time
  - Appointment status

**Supported appointment statuses:**
- Pending  
- Confirmed  
- Completed  
- Canceled  
- Rescheduled  
- No Show  

### 📄 Medical Records
- For every attended appointment, a medical record is stored.
- Each medical record contains:
  - Unique identifier
  - Patient (FK)
  - Doctor (FK)
  - Appointment (FK)
  - Description of visit
  - Diagnosis
  - Prescribed medication
  - Notes

### 💊 Prescriptions
- Each medical record may have **at most one** prescription.
- A prescription includes:
  - Unique identifier
  - Medical record (FK)
  - Medication name
  - Dosage
  - Frequency
  - Start & end dates
  - Special instructions

### 💳 Payments
- Payments are made **per appointment**.
- Each payment contains:
  - Unique identifier
  - Appointment (FK)
  - Patient (FK)
  - Payment method
  - Payment date
  - Amount paid
  - Additional notes

---

## 🧩 Relational Schema Preview

The complete schema can be found in the PNG file in this repository.

---

## 🛠 Tools Used
- **ERDPlus** – Used to create the ER diagram and relational schema.
- **PNG Export** – Included for easy viewing.

---

