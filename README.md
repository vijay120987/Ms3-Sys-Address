# Ms3-Sys-Address
 Ms3-Sys-Address
MS3 Contact API

Contacts API is used to create contact record in Identification Database. Have created System API to create record in Communication , Address and Identification Database Have created Process API to orchestrate the records Have created Experience API to Pass through the definition

DB Creation :

create table Identification (Id INT AUTO_INCREMENT, FirstName varchar(100), LastName varchar(100), DOB varchar(20), Gender varchar(2), Title varchar(100),PRIMARY KEY(Id))

create table Address (Id INT AUTO_INCREMENT, type varchar(20), number varchar(50), street varchar(200), Unit varchar(10), City varchar(50), State varchar(100),zipcode varchar(10), IdentificationId varchar(10),PRIMARY KEY(Id))

create table Communication (Id IN AUTO_INCREMENT, type varchar(100), value varchar(100), preferred varchar(20),IdentificationId varchar(10),PRIMARY KEY(Id))

How to run :

Extract the Experience , Process , System API code and Import into Anypoint Studio Deploy all the Five Application in to Mule Runtime I have attached Postman collections under src/test/resources/postman/MS3.postman_collection_Exp of ms3-exp-contact-api and execute all requests The Results are captured under src/test/resources/TestDoc/Experience API_Contact.docx of ms3-exp-contact-api
