# Interactive Log4j2 Console App

A production-grade, interactive Java console application built using Maven that demonstrates decoupled software architecture and advanced asynchronous runtime logging using **Apache Log4j2**.

---

## 🚀 Features

*   **Live Interactive Loop:** Runs a continuous console engine that processes user inputs in real-time.
*   **Dual-Route Logging:** Configured via a customized `log4j2.xml` to route tracking events to both the live terminal console and background rolling file appenders simultaneously.
*   **Decoupled Architecture:** Separates execution responsibilities cleanly across core application drivers (`App.java`) and dedicated execution processors (`EventService.java`).
*   **Optimized Repository Management:** Includes an automated `.gitignore` strategy that filters out heavy build environments, ensuring a clean and light footprint.

---

## 📂 Project Directory Structure

```text
FINAL LOG/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── example/
│   │   │           ├── App.java           # Application entry point and interactive terminal loop
│   │   │           └── EventService.java  # Logic processor handling core console transactions
│   │   └── resources/
│   │       └── log4j2.xml                 # Enterprise-grade dual-routing appender configuration
│   └── test/                              # Unit testing files
│
├── .gitignore                             # Filters target/, logs/, and workspace metadata
└── pom.xml                                # Maven dependency lifecycle configurations
