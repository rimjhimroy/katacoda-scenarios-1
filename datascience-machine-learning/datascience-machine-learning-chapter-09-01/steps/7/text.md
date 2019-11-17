You always start your Spark scripts by getting a SparkContext object, and this is the object that embodies the guts of Spark. It is what is going to give you your RDDs to process on, so it is what generates the objects that you use in your processing.

You know, you don't actually think about the SparkContext very much when you're actually writing Spark programs, but it is sort of the substrate that is running them for you under the hood. If you're running in the Spark shell interactively, it has an sc object already available for you that you can use to create RDDs. In a standalone script, however, you will have to create that SparkContext explicitly, and you'll have to pay attention to the parameters that you use because you can actually tell the Spark context how you want that to be distributed. Should I take advantage of every core that I have available to me? Should I be running on a cluster or just standalone on my local computer? So, that's where you set up the fundamental settings of how Spark will operate.