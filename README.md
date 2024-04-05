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
The given task is to model and build a relational database that stores useful and necessary information for the manager of a football club. The main entities in the model are the Players and Teams entities. "Players" refers to each of the individuals that participate in games and "Teams" refers to the grouping of specific players together. For each player, there is a record of their contract, game statistics, medical history, and brand deals. Moreover, all teams have distinct sponsorships, coaches, practices, games, etc. Our goal is to effectively and efficiently model these various relationships, create sample data, and use said data to populate all of the entities and their attributes. Additionally, we need to construct functioning queries on this data in order for us to obtain valuable insight about how the club operates 
in a manner that is relevant from a managerial perspective.

## Data Model:
This data model is based on the structure of a hypothetical football club. The 'Players' entity represents each of the individuals that play on the football teams. Each player has a single contract and each contract is designated for a single player, so we placed a one-to-one relationship between these two entities.

Apart from the 'PlayerContracts' entity, the 'Players' entity has three other branches extending from it. The 'Medical Records' entity represents the health and patient history of each player. It includes information on types of injuries, when they occurred, whether they have recovered, and their expected return date to the team. Each player can have multiple medical records, such as records from different healthcare providers, but each medical record will only correspond to a single player. Hence, we established a one-to-many relationship between the 'Players' and 'Medical Records' entities. Similarly, we put a one-to-many relationship between 'Players' and 'Brand Deals' since one player can have brand deals with multiple brands. 

The 'PlayerStats' entity stores information about the performance of each player during their games, such as the number of points, assists, and rebounds they amassed. Each player will have more than one set of statistics that are unique to them. These sets are gathered after every game, so there is a one-to-many relationship between the 'Players' and 'PlayerStats' entities as well as a one-to-many relationship between the 'Games' and 'PlayerStats' entities.

The 'Teams' entity consists of the various teams within the club which are made up of many different players. Similar to the one-to-one relationship between the 'Players' and 'PlayerContracts' entities, each team has its own coach and each coach is in charge of one team. All coaches also have their own contracts. Additionally, teams have different sponsporships and merchandise to promote themselves and raise money for things like equipment. 

![Screenshot 2024-04-04 at 5 30 14 PM](https://github.com/indhu0614/MIST_GP/assets/165066443/f2696c51-ba17-4f1a-bc0f-0aa15eb62e79)

## Data Dictionary: 
<img width="902" alt="Screenshot 2024-03-30 at 4 31 31 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/04caab77-1f31-4ac9-a504-525aec266f70">

<img width="893" alt="Screenshot 2024-03-30 at 4 32 06 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/39ca2528-21c5-40e1-9b64-fbcce74687a8">

<img width="871" alt="Screenshot 2024-03-30 at 8 50 20 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/4fa35d30-8d81-46cb-8a6d-72be935f10e5">

<img width="602" alt="Screenshot 2024-03-30 at 8 50 32 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/d290ca46-4751-486d-bfb0-bf038139ca23">

<img width="698" alt="Screenshot 2024-03-30 at 4 37 38 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/581ea3be-65b8-4822-9b75-3e8c6978fd1a">

<img width="587" alt="Screenshot 2024-03-30 at 8 53 13 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/21d6692a-3426-4336-856f-0959207fe120">

<img width="588" alt="Screenshot 2024-03-30 at 8 53 19 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/faf92e8c-8524-4913-8f6a-2d1f172e757e">

<img width="685" alt="Screenshot 2024-03-30 at 4 37 49 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/e391799d-31f5-4bbb-af18-c1702066416b">

<img width="589" alt="Screenshot 2024-03-30 at 8 53 28 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/d5314a93-e36c-4f9a-aeed-d371c188422a">

<img width="588" alt="Screenshot 2024-03-30 at 8 53 35 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/888b1e5f-e3c6-4487-b122-62d5a75c2e9d">

<img width="597" alt="Screenshot 2024-03-30 at 8 53 41 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/177e1d9d-85d3-49a8-81e4-a4770a4c1303">

<img width="587" alt="Screenshot 2024-03-30 at 8 53 48 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/ef517d62-3eb6-4caf-99e3-3626303a6fe6">

<img width="590" alt="Screenshot 2024-03-30 at 8 53 53 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/d0ff946b-b4f7-4ba4-ba66-c947ac98abe3">

<img width="588" alt="Screenshot 2024-03-30 at 8 54 00 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/98f65bb7-d46a-4180-be16-2df947660995">

<img width="591" alt="Screenshot 2024-03-30 at 8 54 06 PM" src="https://github.com/indhu0614/MIST_GP/assets/165066443/edff218d-9973-4cb4-bb5d-ddba819b3f93">

## Queries:
