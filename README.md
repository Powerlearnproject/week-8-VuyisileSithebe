# Solving an SDG Problem with Data (Choose Your SDG)
Part 1: SDG Selection and Problem Definition
SDG Selection:
 Affordable and Clean Energy

Part 2: Database Design
ERD (Entity-Relationship Diagram):

Design an ERD outlining entities and their relationships. 
SDG 7: Entities might include Households, Solar Panels, Energy Usage, and Installation Records.
Schema:

Write SQL statements to create tables based on your ERD. Example:
sql

CREATE TABLE Patients (
    HouseholdsID INT PRIMARY KEY,
    Name VARCHAR(100),
    Rural INT,
    Urban CHAR(1)
);

CREATE TABLE Diseases (
    HouseholdsID INT PRIMARY KEY,
    Name VARCHAR(100)
);

CREATE TABLE TreatmentRecords (
    RecordID INT PRIMARY KEY,
   Clean energyID INT,
   Affordable energy ID INT,
    CleanenergyDate DATE,
    FOREIGN KEY (HouseholdsID) REFERENCES Households(HouseholdsID),
    FOREIGN KEY (Solar PanelsID) REFERENCES Solar Panels(Solar PanelsID)
);
Sample Data:

Populate the tables with sample data for testing purposes.
Part 3: SQL Programming
Data Retrieval:

Write SQL queries to retrieve relevant data. Example:
sql

SELECT Name, COUNT(DiseaseID) AS NumberOfTreatments
FROM Solar Panels
JOIN Solar Panels ON Patients.Installation RecordsID = Solar Panels.Installation RecordsID
GROUP BY Name;
Data Analysis:

Write SQL queries to analyze data and generate insights. Example:
sql

SELECT Clean energyID, COUNT(*) AS NumberOfCases
FROM Installation Records
GROUP BY Solar PanelsID;
Part 4: Data Analysis Using Excel
