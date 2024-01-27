# nosql-challenge
Module 12 challenge
I activated conda and opened jupyter notebook to access PyMongo.
I then imported the establishments json file using the MongoImport command code.

Part One: Database and Jupyter Notebook Set Up
Once a connection was made, I created variables and displaying the documents found in the file.

Part Two: Update the Database
I inserted a collection using the information given.
The new collection was missing a RatingValue so I found the Rating Value that corresponded to the "Restaurant/Cafe/Canteen" establishments.
I then removed the Dover establishments and updated datatypes.
Updating datatypes was slighlty troublesome because I was expecting a list of the datatypes, instead the code only returns the updated collection.
I also had to limit the list returned because displaying many collections would create a large file, which would then crash my jupyter notebook 
and not display in github. I did reach out to BCS to figure out an outside solution since I couldn't access my work in jupyter notebook; however, after alot of patience, I was able to enter my jupyter notebook and limit the amount returned, and shrink the file.   

Part Three: Exploratory Analysis
I realized that I had not properly converted the strings to integers, or maybe both notebooks had to be running
so the code in part two could apply to code in part three.
Finding the distance was a bit tricky and therefore I considered using $geonear, but before taking that approach I input the information that I knew such as creating the latitude, longitude and results variable; setting the Rating Value eq:5; Sorting by 1; and adding a limit. Then I applied the calculation to the query section of the code.