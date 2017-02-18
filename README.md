# Locality Sensitive Hashing
Showcasing the locality sensitive hashing algorithm with shingling, minhashing and banding applied.

Locality sensitive hashing is a fast and memory efficient algorithm to
obtain an estimate of the amount of similar items in a dataset compared to an
exhaustive search. In this repository we discuss our implementation of the locality sensitive
hashing algorithm combined with techniques called banding, shingling and minhashing. We test the algorithm
on a dataset of 103700 users who rated in total 17770 movies, each user rated at least
300 movies. We search for the amount of user pairs that rated movies with a similarity
larger than 0.5. The algorithm returns over 5 runs a median value of 417 user pairs
that match the similarity condition within a median time of 403 seconds on an Intel
Core i5-6300U CPU @2.4 GHz with 8 GB of RAM. The result is found to be off from
the correct value of 1205 user pairs. However in comparison to an exhaustive search,
which would take 106 days, the algorithm is significantly faster.

The dataset used is incorporated in a .npy file: 'user_movie.npy'. The dataset is actually a reduced dataset obtained from the netflix challenge (http://www.netflixprize.com/) we removed the users that rated less than 300 or more than 3000 movies.
Also incorporated in this repository is a report made about the implementation of the algorithm and our results (lsh.pdf).

The algorithm was made for an assignment of the course: Advances in Datamining given by Dr. W. Kowalczyk.
The course was given at Leiden University and is part of the Computer Science Master track.
see: https://studiegids.leidenuniv.nl/courses/show/57329/advances-in-data-mining



If you have any questions, remarks or possible improvements please let us know!
