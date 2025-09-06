# 📊 Attendance & Payroll Dashboard (Angular Frontend)

This is the **frontend web application** for the IoT-based biometric attendance and payroll system.  
It connects with a **Spring Boot + PostgreSQL backend** and an **ESP32 + R307S Fingerprint Sensor IoT device**.

---

## 🚀 Features

- **Dashboard**
  - Total Employees, Present Today, Absent Today, Monthly Payroll
  - Charts for attendance trends and salary distribution

- **Employee Management**
  - Add / Edit / Delete employees
  - Store employee details (name, age, fingerprint ID, daily wage)

- **Attendance Logs**
  - Track daily check-in / check-out
  - Filter by employee or date
  - Show status (Present / Absent / Late)

- **Salary Management**
  - Auto calculate salary based on attendance
  - Monthly payroll reports
  - Export as PDF / Excel

---

## 🛠️ Tech Stack

- **Frontend**: Angular 17, Angular Material, Chart.js (ng2-charts)
- **Backend (separate repo)**: Spring Boot + PostgreSQL
- **IoT**: ESP32 + R307S Fingerprint + DS3231 RTC + OLED Display

---

## 📂 Project Structure

biometric-attendance-system/
 ├── README.md                 # Main project description
 ├── frontend/                 # Angular Dashboard
 │   └── attendance-payroll-frontend/
 ├── README.md
 ├── angular.json
 ├── package.json
 ├── tsconfig.json
 ├── src/
 │   ├── index.html
 │   ├── main.ts
 │   ├── styles.css
 │   ├── app/
 │   │   ├── app.component.ts
 │   │   ├── app.component.html
 │   │   ├── app-routing.module.ts
 │   │   ├── core/
 │   │   │   ├── models/
 │   │   │   │   ├── employee.model.ts
 │   │   │   │   ├── attendance.model.ts
 │   │   │   │   └── salary.model.ts
 │   │   │   └── services/
 │   │   │       ├── employee.service.ts
 │   │   │       ├── attendance.service.ts
 │   │   │       └── salary.service.ts
 │   │   ├── modules/
 │   │   │   ├── dashboard/
 │   │   │   │   ├── dashboard.component.ts
 │   │   │   │   ├── dashboard.component.html
 │   │   │   │   └── dashboard.component.css
 │   │   │   ├── employee/
 │   │   │   │   ├── employee.component.ts
 │   │   │   │   ├── employee.component.html
 │   │   │   │   └── employee.component.css
 │   │   │   ├── attendance/
 │   │   │   │   ├── attendance.component.ts
 │   │   │   │   ├── attendance.component.html
 │   │   │   │   └── attendance.component.css
 │   │   │   └── salary/
 │   │   │       ├── salary.component.ts
 │   │   │       ├── salary.component.html
 │   │   │       └── salary.component.css
 │   │   └── shared/
 │   │       ├── navbar/
 │   │       └── sidebar/

 ├── backend/                  # Spring Boot API
 │   └── (Spring Boot files...)
 ├── iot/                      # ESP32 Fingerprint Code
 │   └── (ESP32 Arduino code...)
 └── docs/                     # Extra docs (DB schema, diagrams)


