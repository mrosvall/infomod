# infomod
 Source code updated 2011 for [An information-theoretic framework for resolving community structure in complex networks Martin Rosvall and Carl T. Bergstrom,  PNAS 104, 7327 (2007)](http://dx.doi.org/10.1073/pnas.0611034104).

## Run

Compile with `make` 
Run with `./infomod 345234 MultiphysChemBioEco40_unweighted_undir.net 10`  

In this example, `./infomod` is the name of the executable, `345234` is a random seed (can be any positive integer value), `MultiphysChemBioEco40_unweighted_undir.net` is the network to partition (in Pajek's `.net` format), and `10` is the number of attempts to partition the network (can be any integer value equal or larger than 1).   

The code writes the results to two plain text files. The partition file with extension `.clu`, which gives the cluster assignments, can be used together with the original network to show the clusters in Pajek (import both files and use the command Draw->Draw-Partition in Pajek). The file `.mod` is an enumeration of all members of each cluster. Please send an e-mail to martin.rosvall@umu.se if you encounter any problems.
