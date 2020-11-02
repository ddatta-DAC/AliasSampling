# AliasSampling

In graph based random walks, sampling of neighbors can be done in many ways. But all of them are not equally efficient. The neighbor sampling process is sampling from a categorical or discrete  distribution. The same issue is also encountered in word2vec, when words need to be sampled as per their frequency of occurrence.

Alias Sampling is a method to perform this in O(1) i.e. constant time. While some initial cost is incurred in setting up the data structures, for a even moderate number of samples - it leads to gain in efficiency.

========================

Whats is the key intuition ?

For a random event with k possible outcomes with uniform likelihood, it is easy and efficient to generate that. e.g. casting a dice which is unbiased.
The key idea is to leverage such a uniform distribution to generate our outcomes, which have non uniform probabilities.


A good tutorial on the details :
https://www.keithschwarz.com/darts-dice-coins/
