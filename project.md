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
|club_winning_match|winning match|stores the numbers of winning match of that team|int(2)||
|club_losing_match|losing match|stores the numbers of losing match of that team|int(2)||
|club_drawing_match|drawing match|stores the numbers of drawing match of that team|int(2)||
|club_financial|club's money|stores how much does the club currently have|int(11)|


### 2. PLAYERS 
|Field Name|Canonical Name|Description|Data Type|Key|Source|
|--|--|--|--|--|--|
|player_id|player ID|stores the id of a player|varchar(10)|PK|
|contract_id|contract id|stores the contract id of a player|int(10)||FK|
|player_stats_id|player's statistic id|stores the id of statistic of a player|int(10)||FK|
|club_name|Club name|stores the name of the club which this player is playing for|varchar(20)||FK|
|first_name|player's first name|stores the first name of the player|varchar(10)|||
|last_name|player's last name|stores the last name of the player|varchar(10)|
|position|player's position|stores the position that player plays|varchar(20)|||
|mobile_number|phone number|stores the phone number of a player|int(11)|



### 3. COACH
|Field Name|Canonical Name|Description|Data Type|Key|Source|
|--|--|--|--|--|--|
|coach_id|coach ID|stores the id of the coach|varchar(10)|PK|
|contract_id|contract ID|stores the id of coach's contract||
|coach_team|coach team|stores the team name that this coach is belong to|varchar(20)||FK|
|coach_first_name|coach's first name|stores the first name of the coach|varchar(10)||
|coach_last_name|coach's last name|stores the last name of the coach|varchar(10)||
|title|title|stores the title of the coach in a team|varchar(11)||



### 4. FACILITIES 
|Field Name|Canonical Name|Description|Data Type|Key|Source|
|--|--|--|--|--|--|
|facilities_id|facilities or equipment id|stores an id of facilities or equipment of a team|int(5)|PK|
|gym_rooms|gym training rooms|stores number of training rooms that club has|int(2)||
|recovery_center|recovery center|stores number of recovery centers that club has|int(2)||
|training_ground_name|training field's name|stores a training fields of a club|varchar(20)||
