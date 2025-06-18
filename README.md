# Learn Trino 🚀  
Cross-Database SQL Analytics Using Trino (MySQL + PostgreSQL)

This project is a hands-on playground for running cross-database SQL analytics using **Trino**, a distributed SQL query engine. It connects to a MySQL and PostgreSQL database and enables joining tables across them *without* traditional ETL pipelines.

---

## 💡 Use Case

**"How can we combine customer data from MySQL and transaction data from PostgreSQL for a complete analysis — without building a complex data pipeline?"**

This lab demonstrates a practical scenario:
- 🧑‍🤝‍🧑 Customer data stored in **MySQL**
- 💸 Order & product data stored in **PostgreSQL**
- 🔗 Joined and queried seamlessly in **Trino**

---

## 📂 Project Structure

trino-learn/
├── docker-compose.yaml
└── trino/
└── etc/
├── catalog/
│ ├── freedb.properties # MySQL connection config
│ └── neondb.properties # PostgreSQL connection config
├── config.properties # Trino coordinator config
├── jvm.config
└── log.properties


---

## 🔧 Setup Steps
1. Clone the Repository
git clone https://github.com/yourusername/trino-analytics-lab.git
cd trino-analytics-lab

2. Configure Database Catalogs (MySQL & PostgreSQL)
    Edit the catalog files inside trino/etc/catalog/:
    - freedb.properties for MySQL
    - neondb.properties for PostgreSQL

    Update each file with your own connection details (Host,Port,Database Name,Username,Password)

3. Start Trino Using Docker Compose
docker-compose up -d

4. Access the Trino Web UI at: http://localhost:8080

---
Feel free to discuss, Cheers 🍻.