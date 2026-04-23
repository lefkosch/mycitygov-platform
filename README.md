#MyCityGov
===
A web-based citizen services platform inspired by gov.gr, developed as a team project at Harokopio University of Athens.

## Overview
MyCityGov is a full-stack application that allows citizens to submit requests, report issues, and manage appointments with municipal services through a centralized platform.

## Technologies
- Java (Spring Boot)
- H2 Database
- Docker Compose
- Swagger / OpenAPI
- JWT Authentication
- MinIO (S3 Storage)

## Features
- Citizen request submission
- Issue reporting
- Appointment management
- Role-based access control (Citizen, Employee, Admin)

## My Contribution
- Implemented and managed data persistence using H2 database
- Developed and integrated the MockGovService for user validation
- Contributed to backend development using Spring Boot

## How to Run
---

Clone the repository:

```shell
git clone https://github.com/lefkosch/mycitygov-platform.git
```

---

Run the example:

```shell
cd mycitygov-platform
docker compose up -d --build # Windows / MacOS / Linux
```
After the build you open/close the program with the following commands
```shell
docker compose up -d
docker compose down
docker compose down -v #If you want to restart the whole program and delete the DB etc...
```
---
URLs :

- Open in browser: [localhost:8080](http://localhost:8080)

- For the DataBase: [localhost:8080/h2-console](http://localhost:8080/h2-console)

- For the S3(MinIO): http://localhost:9001/login

- Swagger UI: http://localhost:8080/swagger-ui/index.html 



---
To gain access to the DB:
```shell
Username: sa
Password:
Copy to Url: jdbc:h2:file:/data/mycitygov2db
```


---
To gain access to the S3(Minio):
```shell
Username: minioadmin
Password: minioadmin
Url: http://localhost:9001/login
```
---
Προτεινόμενα στοιχεία για την εγγραφή προκειμένου να λειτουργήσει και το Mock Gov Service
```shell
ΑΦΜ: 999999999
ΑΜΚΑ: 99999999999
Ονομα: Dimitris
Επώνυμο: Gkoulis
```

---
Staff Accounts
```shell
For the ADMIN
Email: admin@mycity.gov
Password: Admin1!234
```
```shell
For the first EMPLOYEE (KEP)
Email: employee1@mycity.gov
Password: Emp1!23456
```
```shell
For the second EMPLOYEE (TECHNICAL_SERVICE)
Email: employee2@mycity.gov
Password: Emp2!23456
```
```shell
For the third EMPLOYEE (SOCIAL_SERVICE)
Email: employee3@mycity.gov
Password: Emp3!23456
```
```shell
For the forth EMPLOYEE (FINANCIAL_SERVICE)
Email: employee4@mycity.gov
Password: Emp4!23456
```
```shell
For the fifth EMPLOYEE (ENVIRONMENT_SERVICE)
Email: employee5@mycity.gov
Password: Emp5!23456
```
---
