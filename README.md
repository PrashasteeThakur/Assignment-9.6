# Assignment-9.6

1.Explain about the different complex data types in pig.

Ans.Different complex data types in pig are
1.Tuple 
• A record that is formed by an ordered set of fields is known as a tuple, the fields can be of any type. 
• A tuple is similar to a row in a table of RDBMS.
  Example − (Raja, 30)
2.Bag 
• A bag is an unordered set of tuples.In other words, a collection of tuples (non-unique) is known as a bag. 
• Each tuple can have any number of fields (flexible schema).A bag is represented by ‘{}’. 
• It is similar to a table in RDBMS, but unlike a table in RDBMS, it is not necessary that every tuple contain the same number of fields or that the fields in the same position (column) have the same type. 
  Example − {(Raja, 30), (Mohammad, 45)}
3.Map 
• A map (or data map) is a set of key-value pairs. 
• The key needs to be of type chararray and should be unique. 
• The value might be of any type. It is represented by ‘[]’ Example: [name#Raja, age#30] 
4.Relation 
• A relation is an outer bag of tuples. 
• The relations in Pig Latin are unordered (there is no guarantee that tuples are processed in any particular order).

2.How can you interact with the shell in Apache pig?

Ans.

3.Explain how pig differs from Map reduce.

Ans.

4.Explain how pig differs from sql.

Ans.In SQL, when users want to do several data operations together, they must either write separate queries, storing the intermediate data into temporary tables, or write it in one query using subqueries inside that query to do the earlier steps of the processing. 
• Pig, however, is designed with a long series of data operations in mind, so there is no need to write the data pipeline in an inverted set of subqueries or to worry about storing data in temporary tables. 
• SQL is designed for the RDBMS environment, where data is normalized and schemas and proper constraints are enforced (that is, there are no nulls in places they do not belong, etc.). 
• Pig is designed for the Hadoop data-processing environment, where schemas are sometimes unknown or inconsistent. Pig does not require data to be loaded into tables first. It can operate on data as soon as it is copied into HDFS.


5.Explain the scalar data types in pig.

Ans.Different scalar data types in pig are 
• int : It is signed 32 bit integer. This is similar to the Integer in java.
•	long : It is a 64 bit signed integer. This is similar to the Long in java.
•	float : It is a 32 bit floating point. This data type is similar to the Float in java.
•	double : It is a 64 bit floating pint. This data type is similar to the Double in java.
•	chararray : It is character array in unicode UTF-8 format. This corresponds to java's String object.
•	bytearray : Used to represent bytes. It is the default data type. If you don't specify a data type for a filed, then bytearray datatype is assigned for the field.

