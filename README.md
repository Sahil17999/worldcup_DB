
# WorldCup-DB Project Summary

## Project Overview
The WorldCup-DB project focuses on managing and querying a database related to the FIFA World Cup. This database stores a variety of data such as the year, round, winner, opponent, winner_goals, and opponent_goals; enabling users to retrieve detailed information and insights about the tournament's history and participants.

## Key Components
- **Database Schema**: The schema includes tables for the teams and games. The teams table contains all distinct teams that participated in the FIFA world cup where a primary key called team_id is set to reference such teams in the games table as winner_id and opponent_id foreign key columns. A detailed description of the steps performed are bellow:
  
## Tasks Summary
- **Database Creation**:
  - Create `worldcup` database.
  - Create `teams` and `games` tables with the specified structure.
- **Data Insertion**:
  - Insert 24 unique teams into the `teams` table.
  - Insert 32 games into the `games` table with appropriate references.
- **Data Querying**:
  - Complete `queries.sh` to match the expected output.

- **Tools and Technologies**: 
  - PostgreSQL Workbench for database design and query testing.
  - Bash scripting to avoid hard coding values in the two tables.
  - Gitpod as a service to utlize their virtual machine with Visual Studio Code to create the project.

- **Challenges and Solutions**:
  - Partitioning the dataset so that it can be redirected into the games and teams table. Utilized bash if/else conditions, variables and the cat command to perform this task.
  - Filtering the tables in a way so that the output matches the expected output text file. Utilized aggregate functions along with the SELECT command to perform the following task.
  
## How to Run
1. Clone the repository and navigate to the project directory.
2. Run `insert_data.sh` to populate the database.
3. Run `queries.sh` to generate the desired outputs.

## File Descriptions
- **games.csv**: Contains World Cup game data.
- **insert_data.sh**: Script to populate the database.
- **queries.sh**: Script to query the database.
- **expected_output.txt**: Contains the expected output for queries.

## Future Enhancement
- **API Development**: Creating an API to allow external applications to interact with the database, enabling broader usage of the data.

## Conclusion
The WorldCup-DB project serves as a comprehensive database management solution tailored to the needs of sports data analysts and enthusiasts. With its well-structured schema, efficient queries, and robust data integrity measures, it provides a strong foundation for any further development or analysis related to the FIFA World Cup.
