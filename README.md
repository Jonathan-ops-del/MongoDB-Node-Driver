MongoDB Node Driver

The purpose of this project is to demonstrate on how to connect the MongoDB Database with Nodejs using the MongoDB Native Driver. In this project, we will create a database on MongoDB called "fruitsDB". In this database, we will insert a collection - called "fruits". Within this collection, we will add 3 seperate fruit documents with the properties: "name", "score", and "review". This will be apart of the Create Operation of CRUD. You will also be able to see the Read Operation demonstrated where you can access the documents in your Nodejs.

You will notice this project has 3 branches, and you will require all 3 branches in order to follow the steps to this project. The first branch is the "master" branch, the second branch is the "createOnly" branch, and the third branch is the "readOnly" branch. To begin this project, you will clone the code into your preferred Code Editor. Your default branch will be the "master" branch. Make sure to checkout to each branch in the code editor terminal by entering "git checkout createOnly" and then "git checkout readOnly" to give you access to all 3 branches from the cloned project. Double check to see if you have all 3 branches after the checkouts by entering "git branch" in the terminal and you should see all 3 branches in the terminal.

You will work through all 3 branches to see how we are able to connect to the MongoDB Database, insert documents into the database, and read the documents from the database using MongoDB Node Driver.

Before beginning this project, please make sure you have your HyperTerminal open and have the MongoDB Database running, by entering "mongod" in the HyperTerminal. Once the database is running on the HyperTerminal, open a second tab and enter "mongo" to have access to the mongo shell.

Once you have cloned the project, you will start from the master branch. Make sure to install the dependencies when working in each branch by using npm install. In the master branch once you have installed the dependencies, you can run "node app.js" in the code editor terminal. Once this is running successfully, you will see "Connected successfully to server" in the console. This demonstrates that the server is now connected to the MongoDB database. The database in this project is called - "fruitsDB."

Now you can checkout to the second branch called "createOnly". Once the dependencies are installed using npm install, you can then run "node app.js" in the code editor terminal. Once successfully completed, you will see the following message in the console - "Inserted 3 documents into the collection". You have now inserted 3 documents , 3 seperate fruit objects, into the database. If you go to the HyperTerminal tab where your mongo shell is open, you can now enter in "show dbs" and you will see your fruitsDB database. Once you see this in the shell, you can now enter in "use fruitsDB". You will now have access to the fruitsDB database. In your fruitsDB database, you can enter in "show collections" in the shell and you should find your fruits collections. By entering in "db.fruits.find()" in the shell you will be able to see the fruit documents that were inserted into your fruits collection in the fruitsDB database.

You may now checkout to the third branch, "readOnly". Once the dependencies are installed using npm install, you can then run "node app.js" in the code editor terminal. Once completed successfully you will see the following below in your console: 

Found the following records
[
  {
    _id: new ObjectId("64d18e4ee98f413b119b0768"),
    name: 'Apple',
    score: 8,
    review: 'Great fruits'
  },
  {
    _id: new ObjectId("64d18e4ee98f413b119b0769"),
    name: 'Orange',
    score: 6,
    review: 'Kinda sour'
  },
  {
    _id: new ObjectId("64d18e4ee98f413b119b076a"),
    name: 'Banana',
    score: 9,
    review: 'Great Stuff!'
  }
]

You are now able to read the array of documents in your fruits collection from your fruitsDB database in your Nodejs project.

