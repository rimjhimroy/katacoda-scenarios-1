Task 4: Loops
Loops are an essential part of any programming language and it is no different with Scala. Let us now look at the loops concept and write some code to get familiar with them.

Step 1: Let us start the loops concept with the if loop. Fire up the Scala console if you haven’t already and type in the following code.

scala> val numOfKids = 3

scala> if (numOfKids > 2) println (“They are Phoebe Buffay’s kids.”) else println (“Parent unknown!”)

 

As you can see from the screenshot, the console only prints out the statement which is true based on the condition.

You can also write the if loop in the REPL in multiple lines using the paste mode as shown below. From the Scala prompt enter the following command and hit enter.

scala> :paste

This will take you to the paste mode with a prompt to enter your code as shown in the screenshot.


You can now enter Scala code in multiple lines. Once you are done with your code press Ctrl + D to come out of the paste mode and execute the code.

scala> :paste
//Entering paste mode (ctrl-D to finish)

val numOfKids = 3
if (numOfKids > 2) {
println(“They are Phoebe Buffay’s kids.”)
} else {
println(“Parent unknown!”)
}


The code is executed as soon as you have exited from the paste mode and result is displayed as shown in the screenshot above.