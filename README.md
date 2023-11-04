
# MIST 4610 Group Project 1




## Team Name:
39217 Group 2



## Team Members:
1. Jenny Chen [@jennyc5](https://github.com/jennyc5)

2. Mathews Fluker [@mathewsfluker](https://github.com/mathewsfluker)

3. Justin Goldman [@justingoldman25](https://github.com/justingoldman25)

4. Connor Hawkins [@conehawk](https://github.com/conehawk)

5. Nixxon Idaewor [@NnixxonUGA](https://github.com/NnixxonUGA)

6. Aude-ellen Nangle [@audeellen](https://github.com/audeellen)



## Problem Description:
We have been tasked to  build a relational database for our client the "Atlanta Thunder Hawks". The client is powered through the use of Chat GPT to construct the answers to any questions we may have about the database. The database  must accurately reflect the organization's needs and host information about the sports club,  its activities, requirements, and expectations.










## Conversation with ChatGPT:

We asked: 


Pretend you are the owner/operator of an American football club needing to build a relational database. You hired some students from the MIST 4610 class at the University of Georgia to create the database for you. They need to know more about your organization to identify which entities, attributes, and relationships are important for you. Start by describing your business as a real client.



ChatGPT responded:

As the owner/operator of an American football club, my organization, let's call it the "Georgia Thunderhawks," is a professional football team based in the state of Georgia. We participate in a recognized American football league, such as the NFL, NCAA, or a regional league like the Georgia Football Association. Our primary objective is to excel in the sport, win championships, and provide an exciting and memorable experience for our fans. We are also committed to player development and community engagement.

To help the students from the MIST 4610 class at the University of Georgia create a relational database for our football club, here's some information they'll need:



Entities:

Players: This entity should include details like player names, positions, date of birth, height, weight, and player statistics (e.g., touchdowns, tackles, passing yards, etc.).

Coaches: Information about our coaching staff, including names, positions, coaching history, and contact information.

Staff: This entity can encompass non-coaching staff such as trainers, medical personnel, and administrative personnel, including their contact information and roles.

Games: Information about each game, including date, opponent, location, and final score.

Fans: Data about our fan base, including names, contact information, season ticket holders, and fan engagement statistics.

Sponsors: Information about our sponsors, including their names, contact information, and sponsorship agreements.

Facilities: Details about our training facilities and stadium, including location, capacity, and maintenance schedules.




Attributes:

For the Players entity, attributes can include jersey numbers, college drafted from, and contract details.

For the Coaches entity, attributes can include coaching certifications and performance evaluations.

For the Games entity, attributes can include game duration, weather conditions, and a list of the plays run during the game.

For the Fans entity, attributes can include social media engagement metrics, attendance records, and merchandise purchases.

For the Sponsors entity, attributes can include sponsorship level, contract start and end dates, and the value of the sponsorship.

For the Facilities entity, attributes can include maintenance logs, seating types, and historical records.



Relationships:

Players are related to Games through their participation in each game.

Coaches are related to Players through coaching and mentorship. 

Staff members are related to Facilities through their roles in maintaining and operating these spaces.

Games are related to Fans, as the games are attended by fans.

Sponsors are related to the Club through sponsorship agreements.

Facilities are related to Games, as they serve as venues for the games.

The students can design a relational database that captures all these entities, attributes, and relationships, enabling us to manage player and team performance, fan engagement, and various operational aspects of our football club effectively. This database will help us make data-driven decisions, enhance the fan experience, and ultimately lead to success on and off the field.



## Data Model:
After spaeking with our client we felt as though we had enough information to begin constructing our relational database. Below is a picture of our relational database:

![Screen Shot 2023-11-02 at 11 46 27 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/45da5bdb-f6c6-4b7d-8551-5ae946248fe7)

Staff members each belong to one facility that they work in. The staff is described by their name, job title, and their phone number. Each facility has multiple Staff members and each Facility is described by its location, capacity, and the time at which maintnience is done to the facility. Each facility hosts multiple games, yet only one game can be played in one facility at a time. 

Each Game is described by numerous attributes such as the date, the score of the ThunderHawks and the weather of the game. Each Game hosts multiple sponsorships which come at a price and a tier. Each Sponsor can have many Sponsorships, and Sponsors can be described by their company name and email. 

Within each game there are several downs. Each down is described by the yards that were gained on that play. Each Down can only host one Play but a Play can have multiple Downs. The Plays table hosts information about the name of the Play and the type of Play that it is. 

Games also host many Tickets but there can only be one individual ticket to one individual game. Tickets are described by their price and seat number. Fans can have multiple tickets, however, only one unique ticket can exist for each fan. Each Fan is given a profile listing their name and phone number as well as the status of their tickets. 

Each Game also has many Game statistics, such as pass yards, rush yards and touchdowns. Players can record many Game Statistics and each player is described by their name, position, and jersey number amongst other things. Each Player has multiple Training Sessions during the week that have a Coach present. During each Training Session the Duration and the player's Max Heart Rate is recorded. Coaches can also be present at multiple training sessions. Each coach is described by their Name, Title, and the Number of Certificates that they have obtained.




## Data Dictionary:

![Screen Shot 2023-11-03 at 3 13 14 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/4447b3ad-8842-4965-a35b-e5aff2727526)

![Screen Shot 2023-11-03 at 3 14 57 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/0448d94c-6b5e-4508-b254-1cfe0b3e1cd0)
![Screen Shot 2023-11-03 at 3 16 01 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/8d755374-37a5-410f-85a4-1f30a55f18a3)
![Screen Shot 2023-11-03 at 3 16 56 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/bdcddde3-9a1e-4ab8-99d4-57d7215ca131)
![Screen Shot 2023-11-03 at 3 17 32 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/985ef443-78d3-49a7-979e-22cba82b74f2)
![Screen Shot 2023-11-03 at 3 18 48 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/a475e99c-c696-4f14-bee9-2fbf4e6b7cf0)
![Screen Shot 2023-11-03 at 3 19 22 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/327d2d88-72a1-48ed-a04c-53fdbc5b769d)
![Screen Shot 2023-11-03 at 3 20 08 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/ec0b743e-3700-4719-a234-9f8e536141bb)
![Screen Shot 2023-11-03 at 3 21 51 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/f0e0dbff-b28e-48eb-bbc2-431ea50925ed)














## Queries:

![Screen Shot 2023-11-03 at 4 11 58 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/a6500d73-58d0-4639-bc72-f709eb0c8128)

Query 1: TopPlayers

Instruction: List the names of players who make more than $900,000 per year and how many touchdowns they scored in total

Significance: Query 1 lists the names of players who have a salary of more than $900,000. This is important to  Coaches because they may use this information as a way to motivate their players. They will be able to identify who their top earners, analyze their performance and motivate them to continue playing well in order for them to maintain that salary or earn more in the future. 

Query: 
CREATE PROCEDURE TopPlayers()
SELECT touchdowns, CONCAT(Players.fName, " ", Players.lName) AS 'Player Name' , Players.salary AS 'Players Salary'
FROM Players
JOIN Game_Statistics ON Players.playerID = Game_Statistics.Players_playerID
WHERE salary > 900000
GROUP BY `Player Name`, `Players Salary`, touchdowns;
 
CALL TopPlayers;


Result:
![Screen Shot 2023-11-03 at 3 34 53 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/d100a36c-6dbf-4c50-bda9-6327978aab9a)






Query 2: LowEarningPlayers()



Instruction: Write a query to list out the names, and salaries of the players who make below the AVERAGE salary of their team

Significance: The team wants to see who on the team is being paid below average to assess pay raises and potential cuts. If a player is paid below average, they could also be used to trade with another team to free up cap space.

Query: 
CREATE PROCEDURE LowEarningPlayers()
SELECT CONCAT(Players.fName, " ", Players.lName) AS 'Player Name' , Players.salary AS 'Players Salary'
FROM Players
WHERE salary < (SELECT AVG (salary) FROM Players)
ORDER BY `Players Salary` DESC;

CALL LowEarningPlayers;



Result:
![Screen Shot 2023-11-03 at 3 37 01 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/886c6c06-83cf-4fc8-860c-97699dcfecec)




Query 3: EuroLargeStadiums()

Instruction: Write a query that lists facilities in Europe with a capacity exceeding 10,000 seats. Order by least to most seating capacity.

Significance:
A manager is analyzing the football market in Europe and is interested in regional facilities with commercial significance.

Query: 
CREATE PROCEDURE EuroLargeStadiums() SELECT facilityID, location, capacity FROM Facilities
WHERE capacity > 10000 AND location IN ("London", "Moscow", "Paris", "Rome", "Berlin")
ORDER BY capacity;

Results:
![Screen Shot 2023-11-03 at 3 28 21 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/525357a2-14e1-4373-bda2-e24b4a624226)




Query 4: CoachesLongTraining()

Instruction:
Write a query that lists coaches whose training sessions are, on average, longer than the average training session. Order by shortest to longest average session.

Significance: An analyst is worried that training for too long could cause injury to players. He wants to know which coaches’ training sessions are longer than the average session.

Query: 
CREATE PROCEDURE CoachesLongTraining()
SELECT CONCAT(Coaches.fName, " ", Coaches.lName) AS `Coach Name`, AVG(durationMinutes) AS `Average Training Session Duration (minutes)` FROM Coaches
JOIN Training_Session ON Coaches.coachID = Training_Session.Coaches_coachID
JOIN Players ON Training_Session.Players_playerID = Players.playerID
GROUP BY `Coach Name`
HAVING AVG(durationMinutes) > (SELECT AVG(durationMinutes) FROM Training_Session)
ORDER BY `Average Training Session Duration (minutes)`ASC;

Results:
![Screen Shot 2023-11-03 at 3 30 45 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/e26987f8-c25a-497d-91f5-5080d6589444)




Query 5: StrengthandConditioning()

Instruction: 

List out all the Strength and Conditioning coaches' information and their respective facilities and locations.


Significance: The team is conducting an audit on its facility staff and needs to know the information of the coaches and the facilties in whch they coach. 

Query: 
CREATE PROCEDURE StrengthandConditioning()
SELECT CONCAT(fName, ", " ,lname) AS `Strength and Conditioning Coach`, phoneNumber, Facilities.location
FROM Staff
JOIN Facilities on Staff.Facilities_facilityID = Facilities.facilityID
WHERE jobTitle = "Strength and Conditioning Coach"
GROUP BY fName, lname, Facilities.location, phoneNumber;

CALL StrengthandConditioning();



Result:

![Screen Shot 2023-11-03 at 3 42 03 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/b3646d59-a2f3-428a-a0ae-18e359b1a78c)




Query 6: AvgStatsbyPosition()

Instruction: List out the average workout time associated with each player and their average stat lineup.  

Significance: The coaches are conducting a study to find out if there is a correlation between minutes worked out and the amount of stats put up in games associated with Players by position.

Query: 

CREATE PROCEDURE AvgStatsByPosition()
SELECT
    Players.position AS `Position`,
    CONCAT(Players.fname, ", ", Players.lname) AS `Player Name`,
    AVG(Training_Session.durationMinutes) AS `Average Training Time`,
    AVG(Game_Statistics.passYards) AS `Average Pass Yards`,
    AVG(Game_Statistics.rushYards) AS `Average Rush Yards`,
    AVG(Game_Statistics.touchdowns) AS `Average Touchdowns`
FROM
    Players
JOIN
    Training_Session ON Players.playerID = Training_Session.Players_playerID
JOIN
    Game_Statistics ON Players.playerID = Game_Statistics.Players_playerID
GROUP BY
    `Position`, `Player Name`
ORDER BY
    `Position`, `Player Name`;
    
CALL AvgStatsByPosition()

![Screen Shot 2023-11-03 at 3 43 35 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/e1feb32c-30ee-438f-ac26-f27f49afd49a)




Query 7: LargestSponsorshipDeals()

Instruction:
Find the largest sponsorship deal amounts, their start dates, and sponsoring companies' names in alphabetical order

Significance:
Understanding who are the biggest corporate sponsors for a team is essential for the football teams’s financial planning process. It helps the management understand their revenue streams from sponsorships and make better informed financial decisions such as budget allocation for different parts of the team from marketing to facility upkeep fees. Additionally, understanding the deal start dates enables the the team to plan for sponsorship contract renegotiations and extensions with them well in advance. It ensures that sponsorships remain a stable source of income. Taking a look at this data can also help prioritize which corporate sponsors to focus in on when corporate sponsorship contracts are up for renewal and ensuring that throughout the term, they are prioritized with their ads. 

Query: 

CREATE PROCEDURE LargestSponsorshipDeals()
SELECT company, startDate, Sponsorships.adPrice AS LargestDealAmount
FROM Sponsors
JOIN Sponsorships ON Sponsors.sponsorID = Sponsorships_sponsorID
WHERE Sponsorships.adPrice = (SELECT MAX(adPrice) FROM Sponsorships)
ORDER BY company ASC;

CALL LargestSponsorshipDeals();



Results:
![Screen Shot 2023-11-03 at 3 48 03 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/98b5f84f-33d3-481f-8192-7417c5f737d4)




Query 8: WeatherImpactOnPerformance()

Instruction: List the average number of Pass Yards and Touchdowns and the weather that coincides with the game. 

Significance:
The coaches are interested in seeing how the weather impacts performance on their games. Specifically, the are looking into the way that rain impacts player performance as they are considering building a new stadium with a roof. 

Query:
CREATE PROCEDURE WeatherImpactOnPerformance()
SELECT weather AS "Weather", COUNT(gameID) AS "# of Games", ROUND(AVG(passYards),2) AS "Pass Yards", ROUND(AVG(touchdowns),2) AS "Touchdowns"
FROM Game_Statistics
JOIN Games ON Game_Statistics.Games_gameID = Games.gameID
GROUP BY weather
ORDER BY COUNT(gameID) DESC;

Result: ![Screen Shot 2023-11-03 at 4 01 54 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/21044558-deed-4e06-8ba8-a2dac33f1fee)




Query 9: FindLowestFacilityAttendanceRate()

Instruction: What is the attendance rate, as a percentage, for each facility where games have been held, and how do these facilities compare in terms of attendance rate, from the lowest to the highest? Also include the facility’s maximum capacity value, ID number, and location.

Significance:
This query is crucial for finding out which facilities and their locations have the lowest attendance rates. This helps the management and marketing teams better understand the local population’s opinions of their team and better position themselves for better marketing campaigns to cultivate a larger fan following in these locations. 
This data can influence game scheduling decisions like scheduling less high-profile games at these venues. 

Query:
![Screen Shot 2023-11-03 at 5 55 15 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/e129c019-f923-4da5-a20d-3208af1397ff)


Result:![Screen Shot 2023-11-03 at 5 55 24 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/a709656b-0741-40d2-a209-dd9e6099edb9)




Query 10: SponsorsWithoutSponsorships()

Instruction: List the company and email of the sponsors who do not yet have sponsorships

Significance: This query will give the football team insights on which teams to reach out to regarding sponsorhips. This will help the football team maximize revenues by maximizing the use of their relationships with Sponsors. 

Query:
CREATE PROCEDURE SponsorsWithoutSponsorships()
SELECT company, email
FROM Sponsors
WHERE NOT EXISTS (SELECT * FROM Sponsorships WHERE Sponsors.sponsorID = Sponsorships.Sponsorships_sponsorID);

Result:

![Screen Shot 2023-11-03 at 4 00 51 PM](https://github.com/mathewsfluker/MIST4610Project1/assets/149734955/5fc44a53-d644-4777-81ca-a760e8de15ab)









Database information: 

Name of the database: ns_F2339217Group2

All of this data and information can be accessed in the ns_F2339217Group2 SQL database server.


