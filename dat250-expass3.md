# Erlend Skutlaberg

## Technical problems
I didn't really encounter any technical problems. The exe was easy to install, and the <br>
shell worked perfectly.

## Screenshots

### Validation of installer
![alt text](/pic/mongoDbVal.png "SHA256 checksum validation")

### Exercise 1: Insert
![alt text](/pic/mongoDBInsert.png "Insert screenshot")

### Exercise1: Query in MongoDB Compass
![alt text](/pic/MDBQueryCompass.png "Query in MongoDB compass")

### Exercise 1: Update documents
![alt text](/pic/MongoDB_updateDoc.png "Update documents")

### Exercise 1: Deleting documents
![alt text](/pic/delete_docs.png "Delete documents")

### Exercise 1: Chunk Write
![Alt text](/pic/MongoDBChunkWrite.png "Chunk write")

### Exercise 2: Map-reduce
![Alt text](/pic/mapreduce.png "mapreduce")

## Map-reduce reasoning
The map-reduce store the collection within the database. It is handy to get a different representation of the data, in this instance,<br>
an overview of num_orders, total items sold and the average items sold for each item in the database. <br>
One of the greatest things about map-reduce is that we can re-use it later if we get more orders in the database, which <br>
can update the collection we already have, keeping it updated at all times. <br>

The collection obtained is shown below
[!Alt text](/pic/mapreduce_result.png "map-reduce result")
Here,  we got the columns "_id", "count", "qty"(quantity) and "avg"(average). <br>
From the result, it seems like the store sells most oranges, where each customer on average buys 9 oranges. <br>
The least sold item is pears, even though the average quantity bought is 10 (but only 1 customer). <br>
This overview can help a store determine which items they need to stock up on, and which they don't need <br>
too many of. In this case, we don't really have enough data to determine what items we need to stock up on. <br>
For instance, if the average quantity of pears holds, then we don't need too many customers before they sell a lot. 
