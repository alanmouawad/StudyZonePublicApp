# Study Zone Manager Pro

A high-performance, cross-platform desktop management system tailored for educational hubs, libraries, and co-working spaces. Designed to optimize facility tracking, automate administrative tasks, and provide secure session logging.

---

## Key Features

* **Real-Time Seat & Zone Tracking:** Monitor space utilization instantly, improving operational efficiency and reducing front-desk overhead.
* **Automated Data Migration & Deployment:** Built-in automated workflow ensuring seamless database initialization within secure user environments.
* **Secure Trial-License Management:** Features hardware-independent time validation logic and encrypted system logs to protect application integrity.
* **Dynamic Billing Engine:** Streamlines payment tracking, administrative reports, and operational audit trails.

---

## Built With (Tech Stack)

* **Backend / UI Framework:** C# | .NET 7.0/8.0
* **Database Engine:** SQLite (Embedded)
* **Encryption Standard:** AES Encryption for secure trial state storage
* **Deployment Tooling:** WiX Toolset v4 (MSI Installer Generation)

---

## Architecture & Data Strategy

To fully comply with modern operating system permission boundaries (preventing `Access Denied` crashes within restricted folders like `C:\Program Files`), the application isolates its environment configurations:
* **Application Binaries:** Securely managed by the Windows installer pipeline.
* **Database & Assets Space:** Initialized dynamic `.db` resources natively copy over to the user's secure storage environment (`Documents/StudyZoneManager`) on the initial launch sequence.

---

## Getting Started

### Prerequisites
* [.NET SDK 7.0 or higher](https://dotnet.microsoft.com/download)
* Visual Studio Code (with *C# Dev Kit* Extension) or Visual Studio 2022.

### Local Installation & Development Run

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/StudyZoneManagerPro.git](https://github.com/YOUR_USERNAME/StudyZoneManagerPro.git)
   cd StudyZoneManagerPro/studyzoneapp
