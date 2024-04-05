# Group 2 MIST 4610 Project 1

## Group Name:
21479 Group 2

## Team Members:
1. Leonardo Hodis (@Leonardo-Hodis)
2. Chris Bohr (@ChrisBohr)
3. Alphin Philip
4. Prathu Garg (@Prathulu)
5. Indhu Madineni (@indhu0614)

## Problem Description:
The given task is to model and build a relational database that stores useful and necessary information for the manager of a basketball club. The main entities in the model are the Players and Teams entities. "Players" refers to each of the individuals that participate in games and "Teams" refers to the grouping of specific players together. For each player, there is a record of their contract, game statistics, medical history, and brand deals. Moreover, all teams have distinct sponsorships, coaches, practices, games, etc. Our goal is to effectively and efficiently model these various relationships, create sample data, and use said data to populate all of the entities and their attributes. Additionally, we need to construct functioning queries on this data in order for us to obtain valuable insight about how the club operates 
in a manner that is relevant from a managerial perspective.

## Data Model:
This data model is based on the structure of a hypothetical basketball club. The 'Players' entity represents each of the individuals that play on the basketball teams. Each player has a single contract and each contract is designated for a single player, so we placed a one-to-one relationship between these two entities.

Apart from the 'PlayerContracts' entity, the 'Players' entity has three other branches extending from it. The 'Medical Records' entity represents the health and patient history of each player. It includes information on types of injuries, when they occurred, whether they have recovered, and their expected return date to the team. Each player can have multiple medical records, such as records from different healthcare providers, but each medical record will only correspond to a single player. Hence, we established a one-to-many relationship between the 'Players' and 'Medical Records' entities. Similarly, we put a one-to-many relationship between 'Players' and 'Brand Deals' since one player can have brand deals with multiple brands. 

The 'PlayerStats' entity stores information about the performance of each player during their games, such as the number of points, assists, and rebounds they amassed. Each player will have more than one set of statistics that are unique to them. These sets are gathered after every game, so there is a one-to-many relationship between the 'Players' and 'PlayerStats' entities as well as a one-to-many relationship between the 'Games' and 'PlayerStats' entities.

The 'Teams' entity consists of the various teams within the club which are made up of many different players. Similar to the one-to-one relationship between the 'Players' and 'PlayerContracts' entities, each team has its own coach and each coach is in charge of one team. All coaches also have their own contracts. Additionally, teams have different sponsporships and merchandise to promote themselves and raise money for things like equipment. 

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/b5dcc7e5-c2d9-452e-b911-145fa265ff2b)


## Data Dictionary: 

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/7945ed0b-a217-4b94-b016-3b8f12971d0c)

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/97ee8c12-8523-4add-a154-73f196704616)

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/4514eb6d-4ad9-4565-b006-669bbd61fd06)

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/02f9409f-be98-435a-89fb-aa378fc69ce3)

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/cbddb860-344c-4d20-a3fa-991990cdd5c0)

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/8e5cabb2-f74d-42bc-be30-010784bcb493)

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/3036c07d-26f7-4b69-92e9-62213b0b8c16)

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/d89df06e-b84e-43fa-891b-1f140263f498)

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/e7d1b45d-fd88-4795-a34c-fe8599b1a2a3)

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/19279708-957a-4a32-bcc6-2190f83dcab4)

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/66d9f794-ac0b-4041-bd45-69bb398f02a7)

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/8f12e0c8-5044-4ea6-8db5-b7f06205079c)

## Queries:
1.) List of all players with their teams.  


Description: A manager can use this information to quickly see the roster of players and their respective teams, which is fundamental for organization and team management.

Query 1 lists each individual player with their respective team. Query 1 allows managers to automatically list players and their teams in alphabetic order rather than having to manually scan the roster for each individual player. A manager can use this information to quickly see the roster of players and their respective teams, which is fundamental for organization and team management.

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/8c59d08c-ce70-4671-aa11-42468495e985)

2.) Total amount spent on player contracts 

Description: This helps a manager understand the financial commitments of the organization to player salaries, which is crucial for budgeting and financial planning.

Query 2 displays the total amount of how much was spent on each players contract. This allows the managers to see the financial commitment of each player on the sports league relative to their salaries. This query will be very useful in future budget allocations as well as general financial planning.

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/2a179dbe-1e5a-4fbb-ba50-fed4366e38ce)

3.) Current brand deals 

Description: A manager can assess the value and number of active brand deals, an important aspect of revenue stream analysis.

Query 3 displays all of the current active brand deals as well as how much they are valued at. This query conveniently organizes the brand deals so the managers will not have to manually sift through their sponsorships. This query allows managers to analye their current brand deals as well as make decisions on future brand deals which is an important aspect of revenue stream analysis.

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/f9f8f833-4e02-4cfb-b8aa-6b64123cbb17)

4.) Retrieve all equipment types and their count. 

Description: Managers need to keep track of the equipment inventory to ensure that there are enough supplies for training and matches.

Query 4 displays each type of equipment as well as their count. Query 4 allows managers to keep track of the equipment inventory to ensure that there are enough supplies for training and matches. This query helps in inventory management and future procurement planning.

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/ad1fc273-8202-4f1a-836f-c95ffdab1563)

5.) Average attendance per game 

Description: Understanding the average attendance can help a manager gauge fan engagement and the success of marketing efforts for game days.

Query 5 displays how many tickets have been sold respective to each game. This query allows managers to automatically compare how many seats there are and how many tickets are being sold. Understanding the average attendance can help a manager gauge fan engagement and the success of marketing efforts for game days. 

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/a554e12f-e0ec-46c5-b6f1-e3fcdca8507d)

6.) Players with injury status and expected return dates

Description: Managers need to be aware of the health status of players to make informed decisions about team lineup and player workload.

Query 6 displays each player with an injury as well as what the expected date they will be able to return is. Query 6 allows managers to see which players will be unavailable for certain periods of time all in one place, rather than having to look at each player individually.  Managers need to be aware of the health status of players to make informed decisions about team lineup and player workload.

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/98bade27-c66d-4a4a-ad5e-4de2b9aabc5b)

7.) Teams with more away than home wins 

Description: Identifies teams with stronger performance in away games, which could indicate resilience and inform strategic decisions regarding training and preparation for different venues.

Query 7 displays all the teams that have more wins when they play away games versus when they play home games. This query saves managers the time of having to manually separate which games are which for each team. Query 7 identifies teams with stronger performance in away games, which could indicate resilience and inform strategic decisions regarding training and preparation for different venues. 

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/72ebbab8-93b1-40f4-9467-6f66af149676)

8.) Total merchandise sales per team 

Description: Merchandise sales are a significant source of revenue. By knowing the sales per team, managers can assess the popularity and marketability of each team and decide where to focus marketing efforts.

Query 8 displays the total merchandise sales of each team. This query organizes all the teams sales in order rather than having the user need to manually compare each team side by side. Merchandise sales are a significant source of revenue. By knowing the sales per team, managers can assess the popularity and marketability of each team and decide where to focus marketing efforts. 

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/e934f3bd-001d-451b-81c0-39024df8f538)

9.) Most effective players based on points per game 

Description: This query identifies players who are scoring above the average points per game, which is essential for a manager to understand who the key contributors are on the court and to potentially use this information for starting lineups or in player development programs.

Query 9 displays which players are the most efficient and have the highest points per game. Managers can use this query to organize the stats for all the players rather than having to calculate the points per game for each individual player. This query identifies players who are scoring above the average points per game, which is essential for a manager to understand who the key contributors are on the court and to potentially use this information for starting lineups or in player development programs.

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/2ceab114-0e2e-4a1d-bc04-bc7018492f9d)

10.) Total points scored by players per team 

Description: High total points can indicate a strong offensive team, while lower points might highlight a need for strategic or player changes.

Query 10 displays the sum of all the points scored by the players on each team. Managers can organize these stats rather than having to manually calculate this for each of their teams. This query is essential for managers to analyze the overall performance of their teams in terms of scoring. High total points can indicate a strong offensive team, while lower points might highlight a need for strategic or player changes. 

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/c4db2a5d-5abe-460f-bc3b-38828d06b76f)

## Matrix

![image](https://github.com/alphinphilip1/MIST4610-Project-1/assets/166083116/8d2501b4-8bcb-4bfa-8664-90d9f21c31d0)




















