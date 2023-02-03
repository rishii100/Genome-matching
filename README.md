# Genome-Matching
The code generates 100 random reads of length 100 from a given genome using the generateReads function. It then uses the naive function to find the exact matches of each read in the genome and calculates the ratio of the number of exact matches to the total number of reads.

## Steps:

1.Import the random module to generate random numbers.
2.Define a function generateReads that takes as input a genome string, a number of reads to be generated (numReads), and the length of each read (readLen).
3.Within the function, initialize an empty list reads to store the generated reads.
4.Use a for loop to generate numReads random starting positions in the genome string.
5.For each starting position, extract a substring of length readLen from the genome and append it to the list reads.
6.Return the list of reads as the output of the function.
7.Generate 100 reads of length 100 using the generateReads function. Store the generated reads in a list called reads.
8.Initialize a counter numMatched to keep track of the number of reads that exactly match the genome.
9.Use a for loop to iterate over each read in the list reads.
10.For each read, call the naive function to find all occurrences of the read in the genome.
11.If the length of the returned list of occurrences is greater than zero, it means that the read matches the genome exactly. Increment the counter numMatched by one.
12.Print the ratio of the number of reads that matched the genome exactly to the total number of reads.
