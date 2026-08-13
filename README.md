spring-hazelcast-example:

docker compose up -d

setelah service Up semua:
<img width="940" height="144" alt="image" src="https://github.com/user-attachments/assets/1b4f7e04-1201-48e5-9dca-1d92323544a9" />


buat Database:

"CREATE DATABASE HAZELCAST;"

"USE HAZELCAST;"

CREATE TABLE dbo.customer ( id INT IDENTITY(1,1) NOT NULL, name VARCHAR(100) COLLATE SQL_Latin1_General_CP1_CI_AS NOT NULL, email VARCHAR(150) COLLATE SQL_Latin1_General_CP1_CI_AS NULL, created_at DATETIME2 DEFAULT GETDATE() NULL, CONSTRAINT PK_customer PRIMARY KEY (id) );

Run ---> mvn spring-boot:run

Url Swagger Spring:
http://localhost:8383/swagger-ui/index.html
<img width="1883" height="1053" alt="image" src="https://github.com/user-attachments/assets/bf18fe39-bdb4-4593-920a-c13c71d9f1fb" />



Url Hazelcast Management:
http://localhost:7070

Hazelcast Management Centre
<img width="940" height="405" alt="image" src="https://github.com/user-attachments/assets/0e385622-9a2e-4a8d-8ccb-c34f72bfa5a0" />


Hazelcast Map cache
<img width="940" height="425" alt="image" src="https://github.com/user-attachments/assets/7e3a5bf0-bfcc-4ae7-b662-426fafc55102" />

