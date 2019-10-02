

Step 2: Let is now write the RDD to Sequence file format using the saveAsSequenceFile method as shown below.

scala> seqRDD.saveAsSequenceFile(“IdeaProjects/Spark/chapter_10/seqOut”)

You may run a cat command from another terminal to check if the save was successful, but the file will not be human readable as shown in the screenshot below.

$ cat IdeaProjects/Spark/chapter_10/seqOut/part*

 
 
We know that the save was successful by looking at SEQ at the beginning of the file. We can also see that the key type is of Text and the value type is of IntWritable.

Step 3: Let us now read this Sequence file we just saved. Reading Sequence files is a bit different to what we have been doing so far. While reading the Sequence file, we need to specify the key and value data types also.

scala> val seqData = sc
.SequenceFile(“IdeaProjects/Spark/chapter_10/seqOut/part-00000”
,classOf[org.apache.hadoop.io.Text]
,classOf[org.apache.hadoop.io.IntWritable])

 

Since this is a Hadoop file format, we need to specify the data types in Hadoop. We have specified the Text and IntWritable types as the types for keys and values since our keys are of String and values are of Int.