<div align="center">
   <img src="https://github.com/mbednarek98/VetClinicHub/blob/master/res/logo.png?raw=true" width="200" alt="VetClinicHub Logo" />

  # VetClinicHub

  
  <a href="LICENSE" target="_blank"><img src="https://img.shields.io/badge/license-MIT-green" alt="Package License" /></a>
  <img src="https://dcbadge.vercel.app/api/shield/247463720337276929?style=flat" alt="Discord" />
   [![bachelor](https://img.shields.io/badge/Documentation-5166f7)](https://docs.google.com/document/d/1tTGC0E9Pq_uH_LJ_demoKaWA-QuIdkYSjxOBtCOc710/edit)
</a>


A Java-based Veterinary Clinic Management System utilizing Hibernate and H2 database, streamlined for efficiency and adherence to UML standards.  Designed for comprehensive clinic operations, including client and staff management, appointment scheduling, and financial transactions.
</div>

## ✨ Features
- Using **Hibernate** and **H2**, this application manages data efficiently and securely.
- The system design and code structure follow the **UML** standard for clarity and consistency.
- The data and workflow management of a veterinary clinic are streamlined.

## 🔑 Prerequisites
- JDK 8 [Download](https://docs.aws.amazon.com/corretto/latest/corretto-8-ug/downloads-list.html)
- H2 Database [Download](https://h2database.com/html/download.html)
- IDE: [InteliJ IDEA](https://www.jetbrains.com/idea/download), [Eclipse](https://www.eclipse.org/downloads/) or any Java-compatible IDE

## ⚙️ Installation
### 1. Clone the Repository
```bash 
$ git clone https://github.com/mbednarek98/VetClinicHub.git
```

### 2. Set up the Database Connection
Create a new database with the name, username, and password of your choice. You can use the H2 Console to do this, or any other database management tool.

To connect to the H2 database, you need to edit the  ``hibernate.cfg.xml`` file in ``src`` directory. Replace the placeholders for ``DATABASE_NAME``, ``DATABASE_USERNAME`` and ``DATABASE_PASSWORD`` with your own H2 settings.
```xml
<hibernate-configuration>
    <session-factory>
    ...
        <property name="connection.url">jdbc:h2:~/DATABASE_NAME.h2</property>
        <property name="connection.username">DATABASE_USERNAME</property>
        <property name="connection.password">DATABASE_PASSWORD</property>
    ...
   </session-factory>
</hibernate-configuration>
```
This will allow Hibernate to create and manage the database schema and tables for the project.

## 📕 License

This project is licensed under the [MIT license](LICENSE)
