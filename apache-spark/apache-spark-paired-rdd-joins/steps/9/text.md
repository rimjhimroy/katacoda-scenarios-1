

Step 4: Finally, let us use the lookup(key) function to lookup value for a key in our joined RDD.


val look = joined.lookup(25)
println(mappedCol)
 

The result is shown as an ArrayBuffer for all the values of the key.

Task 6 is complete!


