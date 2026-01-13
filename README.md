Sports League Management System
Relational Database Design & SQL Implementation

👤 Developer Profile

  Name: Abirami
  Role: Database Designer & SQL Developer
  Location: Christchurch, New Zealand
  Tech Stack: SQL (MySQL/PostgreSQL), ER Modeling, Relational Logic

📌 Project Overview

AthletaBase is a centralized relational database solution built to manage the complex data ecosystem of a professional sports league. From tracking player contracts and team rosters to managing medical staff and multi-million dollar sponsorships, this system provides a high-performance "Single Source of Truth."

🚩 Problem Statement

In modern sports management, data fragmentation is a major hurdle. Team rosters, match schedules, medical records, and sponsorship contracts are often managed in disconnected spreadsheets.

The Challenges:

  Data Inconsistency: Manual entries lead to duplicate records and spelling errors across different files.

  Integrity Failures: No system exists to prevent double-booking referees or assigning players to non-existent teams.

  Slow Reporting: Generating league standings or resource reports requires hours of manual cross-referencing.

🏗️ Implementation Details
1. Conceptual Design

I translated real-world sports rules into a technical blueprint, focusing on:

  Entity Identification: Defined core entities like Teams, Players, Matches, and Sponsors.

  Cardinality: Mapped One-to-Many (One Team to many Staff) and Many-to-Many (Matches involving multiple Teams) relationships.

2. Database Engineering (SQL)

I physically built the system using advanced SQL techniques:

  Schema Architecture: Created tables with optimized data types and Auto-Incrementing Primary Keys.

  Referential Integrity: Implemented Foreign Keys with ON DELETE CASCADE and RESTRICT actions to ensure no "orphan" data exists.

  Normalization: Optimized the database to 3rd Normal Form (3NF) to eliminate redundancy.

3. Data Analytics

I developed complex queries to extract business intelligence:

  Relational Joins: Merging data from 3+ tables to create match-day reports.

  Aggregations: Using COUNT() and GROUP BY to automate league standings and roster counts.

🛠️ Technical Skills Demonstrated

  Database Design: ERD Creation, Logical & Physical Modeling.

  SQL Development: DDL (Table Creation), DML (Data Manipulation).

  Constraints: Primary Keys, Foreign Keys, Unique Keys, and Nullability.

  Reporting: Advanced Querying, Joins, and Aggregate Functions.

🏁 Conclusion

The AthletaBase project demonstrates a scalable approach to sports data. By moving away from flat files and into a structured SQL environment, the league benefits from automated integrity, faster reporting, and a foundation for future growth (such as adding ticket sales or fan analytics). This project reflects my ability to bridge the gap between complex business requirements and efficient technical execution.

📂 Project Structure

    /SQL_Scripts: Contains the full CREATE and INSERT scripts.

    /Diagrams: Includes the ERD visual representation.

    /Queries: A collection of analytical reports for league managers.
