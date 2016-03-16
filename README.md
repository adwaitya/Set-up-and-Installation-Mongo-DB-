# Set-up-and-Installation-Mongo-DB-
Step -1. Download mongoDB from http://mongodb.org/ 
(Note : choose your operating system.


Step -2:After Extract the zip file install it 

Step -3. Copy your installation folder "C:\Program Files\MongoDB\Server\3.2\bin"  and set this path in environment variable for run mongo from command promt.

Step -4 Create one folder C:data\db\
Step: 5: Under C:data\db\ path create one mongo.confg.txt file 

Step  6: write the following things to mongo.confg.txt file

systemLog:
    destination: file
    path: c:\data\log\mongod.log
storage:
    dbPath: c:\data\db
	
	AND Save this file under  "C:data\db\"
Step :7 For start the mongo db . Type mongo "mongod --dbpath C:\data\db"

Step :8 For Create the new database open another cmd prompt and type "mongo"

You will see something in comand promt like this
c:\mongo\bin>mongo
MongoDB shell version: 2.4.5
connecting to: test

Step :9 create new database type "use test"

Step :10 Insert data into database use following command

db.usercollection.insert({ "username" : "testuser1", "email" : "testuser1@testdomain.com" })
