# HealthApp

**HealthApp Management System** is a comprehensive healthcare management system built with ASP.NET Core and Razor Pages. It enables hospitals and clinics to manage appointments, users, and digital prescriptions efficiently, while supporting real-time notifications and modern role-based access.

---

## 📁 Project Structure

This solution is organized into the following main projects:

### 🔹 HealthApp.Razor
- Frontend built with Razor Pages
- Patient, Doctor, and Admin dashboards
- Authentication & Authorization with Identity
- Appointment booking and management interface
- Prescription issuance and viewing
- Responsive UI using Bootstrap

### 🔹 HealthApp.Domain
- Core domain models: `Doctor`, `Patient`, `Appointment`, `Prescription`, `DoctorPatient`
- Role-based user logic using `ApplicationUser`
- Business rules and shared logic

### 🔹 HealthApp.Tests
- Unit tests for backend logic and service validations
- Ensures system reliability and code coverage

---

## 🚀 Key Features

### 🗓️ Appointment Management
- Schedule, approve, cancel, and complete appointments
- Doctor-specific appointment dashboards
- Status tracking and role-based actions

### 👥 User Management
- Role-based login for Admin, Doctor, and Patient
- Identity-based authentication
- Secure registration and login flows

### 💊 Prescription Handling
- Doctors can issue prescriptions digitally
- Patients can view prescription history
- Secure data relations between doctors and patients

### 📬 Notifications (Planned)
- Email notifications for appointment updates
- Integration with RabbitMQ for messaging (planned)
- Real-time feedback and alerts (future feature)

---

## 🧰 Tech Stack

### Backend
- ASP.NET Core (.NET 9.0)
- Entity Framework Core with SQLite
- Identity for authentication
- MediatR and AutoMapper (if extended)

### Frontend
- Razor Pages (CSHTML + C#)
- Bootstrap 5
- Vanilla JavaScript & jQuery

### Infrastructure
- SQL or SQLite database
- RabbitMQ (optional)
- Swagger (if added in API layer)

---

## ⚙️ Getting Started

### 🔧 Prerequisites
- [.NET 9 SDK](https://dotnet.microsoft.com/en-us/download)
- SQLite (or SQL Server)
- Visual Studio 2022 or later



### 📦 Installation

Clone the repository:
bash

git clone https://github.com/your-username/HealthApp.git
cd HealthApp
Restore dependencies:


bash

dotnet restore

Build the solution:

bash

dotnet build

⚙️ Configuration
Database:
Check and update the connection string in HealthApp.Razor/appsettings.json if needed (e.g., for SQLite or SQL Server).

Email & RabbitMQ :
If integrating RabbitMQ or email notifications later, configure them under your appsettings.json or secrets.json.

▶️ Running the Application
Launch the Razor Pages frontend:

bash

cd HealthApp.Razor

dotnet run

Then open in your browser:
arduino

https://localhost:5101
