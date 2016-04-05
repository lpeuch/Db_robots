# Db_robots

This database aims to gather as many robots as possible. Most of the robots are services oriented. 

The database is composed of multiple tables :

###robots
 1. robot_id / int (prim. key)
 2. name / varchar(25)
 3. created_by / varchar(35)
 4. year / int 
 5. origin / varchar(50)
 6. website / text
 7. usage_1 / varchar(25)
 8. usage_2 / varchar(25)
 9. usage_3 / varchar(25)
 10. description / text
 11. size / varchar(40)
 12. weight / varchar(30)
 13. price / varchar(40)

###humanoid
 1. robot_id / int (foreign key)
 2. category / varchar(15)
 3. human_imitation / boolean
 
###drone
 1. robot_id / int (foreign key)
 2. robor_nb / int
 3. blade_nb / int
 4. type / varchar(20)
 
###biorobot
 1. robot_id / int (foreign key)
 2. animal / int
 3. plant / int

###exoskeleton
 1. robot_id / int (foreign key)
 2. carrier / boolean
 3. leg_replacement / boolean
 4. supported_weight / integer

###mobility
 1. robot_id / int (foreign key)
 2. type / varchar(10)

###fictive
 1. robot_id / int (foreign key)
 2. show_type / varchar(15)
 3. show_theme / varchar(25)
 4. robot_type / varchar(20)
