# GROUP 7

###  FOOTBALL DATABASE MANEGEMENT SYSTEM

### 1. CLUB 
|Field Name|Canonical Name|Description|Data Type|Key|Source|
|--|--|--|--|--|--|
|club_name|Club Name|Stores the name of the club|varchar(20)|PK|
|facilities_id|Facilities ID|stores the facilities information of the club|int(5)||FK|
|city|City|Stores the city where the club hosts|varchar(20)||
|email_address|email address|Stores email address of the club|varchar(64)|
|mobile_number|phone number|stores the phone number of the club|int(11)||
|club_points|team points|stores the points the team has|int(3)|
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



### 5. Games / Matches

|Field Name|Canonical Name|Description|Data Type|Key|Source
|--|--|--|--|--|--|
|match_id|Match ID|Stores an ID of the match|int(3)|PK||
|game_start_date|date game starts|stores the date that game is occurred|date|
|time|time|stores the time the game starts|varchar(10)||||
|home_team|Home team|stores the name of the hosted team|varchar(20)||FK|
|away_team|Away team|stores the name of the guest team|varchar(20)||FK|
|stadium|Stadium|stores the name of the stadium|varchar(20)||FK
|referee_id|Referees id|stores the referee information for that match|int(5)||FK|
|result|Result|stores the scores of that game|varchar(5)|||



### 6. Referees
|Field Name|Canonical Name|Description|Data Type|Key|Source
|--|--|--|--|--|--|
|referee_id|Referees ID|stores an ID of that referee|int(5)|PK|
|contract_id||Contract ID|stores a contract ID of that referee|varchar(7)||FK|
|referee_first_name|Referee's first name|stores referee's first name|varchar(15)|||
|referee_last_name|Referee's last name|stores referee's last name|varchar(15)|||
|dob|Date of birth|Stores date of birth of referee|date|||
|nationality|Nationality|stores a nationality of that referee|varchar(64)||


### 7. Ranking Board / Leaderboard
|Field Name|Canonical Name|Description|Data Type|Key|Source
|--|--|--|--|--|--|
|team_rank|Team Rank|stores the rank of teams|varchar(4)||
|team_name|team name|stores the team name to be able to get that team's points|varchar(20)|FK||


### 8. Player Statistics
|Field Name|Canonical Name|Description|Data Type|Key|Source
|--|--|--|--|--|--|
|player_id|Player ID|stores an id of a player|varchar(10)||FK|
|red_card|Red Card|numbers of red card that this player have received|int(2)||
|yellow_card|yellow Card|numbers of yellow card that this player have received|int(2)||
|goals|Goals|numbers of goals that this player have scored|int(4)|||
|assists|Assists|numbers of assists that this player have made|int(4)|

### 9. Goals
|Field Name|Canonical Name|Description|Data Type|Key|Source
|--|--|--|--|--|--|
|goal_id|goals ID|stores goal id|int(3)|PK|
|match_id|Match ID|stores match id|int(3)||FK|
|player_id|player ID|stores player id|int(3)||FK|

### 10. Assits
|Field Name|Canonical Name|Description|Data Type|Key|Source
|--|--|--|--|--|--|
|assist_id|Assits ID|stores assits id|int(3)|PK|
|match_id|Match ID|stores match id|int(3)||FK|
|player_id|player ID|stores player id|int(3)||FK|


### 11. Yellow Card
|Field Name|Canonical Name|Description|Data Type|Key|Source
|--|--|--|--|--|--|
|yellow_id|yellow card ID|stores yellow card id|int(3)|PK|
|match_id|Match ID|stores match id|int(3)||FK|
|player_id|player ID|stores player id|int(3)||FK|


### 12. Red Card
|Field Name|Canonical Name|Description|Data Type|Key|Source
|--|--|--|--|--|--|
|red_id|red card ID|stores red card id|int(3)|PK|
|match_id|Match ID|stores match id|int(3)||FK|
|player_id|player ID|stores player id|int(3)||FK|
