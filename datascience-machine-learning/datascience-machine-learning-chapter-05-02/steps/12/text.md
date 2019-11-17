Quite soon we're going to get to one of the cooler parts of machine learning, at least I think so, called decision trees. But before we can talk about that, it's a necessary to understand the concept of entropy in data science.

So entropy, just like it is in physics and thermodynamics, is a measure of a dataset's disorder, of how same or different the dataset is. So imagine we have a dataset of different classifications, for example, animals. Let's say I have a bunch of animals that I have classified by species. Now, if all of the animals in my dataset are an iguana, I have very low entropy because they're all the same. But if every animal in my dataset is a different animal, I have iguanas and pigs and sloths and who knows what else, then I would have a higher entropy because there's more disorder in my dataset. Things are more different than they are the same.

Entropy is just a way of quantifying that sameness or difference throughout my data. So, an entropy of 0 implies all the classes in the data are the same, whereas if everything is different, I would have a high entropy, and something in between would be a number in between. Entropy just describes how same or different the things in a dataset are.