# GROUP 7

###  FOOTBALL DATABASE MANEGEMENT SYSTEM

### 1. CLUB 
|Field Name|Canonical Name|Description|Data Type|Key|Source|
|--|--|--|--|--|--|
|club_name|Club Name|Stores the name of the club|varchar(20)|PK|
|city|City|Stores the city where the club hosts|varchar(20)||
|email_address|email address|Stores email address of the club|varchar(64)|
|mobile_number|phone number|stores the phone number of the club|int(11)||
|club_points|team points|stores the points the team has|int(3)|


### 2. PLATERS 
|Field Name|Canonical Name|Description|Data Type|Key|Source|
|--|--|--|--|--|--|
|player_id|player ID|stores the id of a player|varchar(10)|PK|
|contract_id|contract id|stores the contract id of a player|int(10)||FK|
|player_stats_id|player's statistic id|stores the id of statistic of a player|int(10)||FK|
|club_name|Club name|stores the name of the club which this player is playing for||FK|
|first_name|player's first name|stores the first name of the player|varchar(10)|||
|last_name|player's last name|stores the last name of the player|varchar(10)|
|mobile_number|phone number|stores the phone number of a player||



### 3. COACH
|Field Name|Canonical Name|Description|Data Type|Key|Source|
|--|--|--|--|--|--|
|coach_id|coach ID|stores the id of the coach|varchar(10)|PK|
|coach_team|coach team|stores the team name that this coach is belong to|varchar(20)|
|coach_first_name|coach's first name|stores the first name of the coach|varchar(10)||
|coach_last_name|coach's last name|stores the last name of the coach|varchar(10)||
|title|title|stores the title of the coach in a team|varchar(11)||



### 4. FACILITIES 
|Field Name|Canonical Name|Description|Data Type|Key|Source|
|--|--|--|--|--|--|
|fooball_pitches|2|gives details  of pitches owned by a club |
|gym|2| gives details about the gym |
|SWIMMING  COMPLEX|4| |
|MEETING ROOMS|9| 


### 5. EQUIPMENTS

|CLEATS|80| gives details about the CLEATS |
|--|--|--|
|SHIN_GUARDS|70| gives details about the SHIN_GUARDS  |
|balls|70| gives details about the balls   |
|water_bottles|70| gives details about the water_bottles |
|uniform|280| gives details about the jersey,training kits etc |
