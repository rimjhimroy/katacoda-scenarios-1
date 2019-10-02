If you do not want the last iteration to be included, you can use the keyword until instead of to. For example,

scala> :paste
//Entering paste mode (ctrl-D to finish)

for ( i <- 1 until 5) {
	val sum = i + i
	println(sum)
}







 
Loops

Functions
Collections

 
We can also use an if statement within the for loop as shown below.

scala> :paste
//Entering paste mode (ctrl-D to finish)

val friends = List(“Chandler”, “Monica”, “Rachel”, “Ross”, “Joey”, “Phoebe”)
for(friend <- friends if friend == “Chandler”){
println(s“The king of sarcasm is $friend”)
}


In the above example, we are looping through the list of collection called friends, with an if condition. We filter out all the items except for one element and substitute the variable in the print statement. Please see that we are using double equals operator to compare two strings.