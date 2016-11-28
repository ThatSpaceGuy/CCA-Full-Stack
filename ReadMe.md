Cluster-Cluster Aggregation Overview
------------------------------------
Cluster-Cluster Aggregation is a good model for the behavior of aerosol particles. This full-stack application will include alternate cluster development discovery. This means that one will be able to make a change in the history of the cluster development to see how things could have gone if a single change was made.

Program Overview
----------------
1) Seed a grid with a given number of "particles" in random positions
2) Choose a random particle and move it in a random direction (Up, Down, Left or Right)
3) If a particle come into contact with another particle it will stick to the other particle and the two particles will then move as a cluster.
4) This behavior continues until only one cluster remains
5) This full-stack app will also keep track of the movement history, allowing a user to retrace the development of the clusters in the program.

Versioning Plan
---------------
* 0.1 - ReadMe & html/js/css/server/heroku handshakes - initial commit
* 0.2 - Basic ReadMe completed
* 0.3 - Seed grid with particles
* 0.4 - Scan grid for any particles seeded together (these start as clusters)
* 0.5 - Store coordinates for checking of aggregation for each particle/cluster
* 0.6 - Move a random particle/cluster
* 0.7 - Check whether the particle/cluster has aggregated any new particles/clusters
* 0.8 - Update information for cluster with new aggregated particle/cluster information
* 0.9 - Update information for checking of aggregation on the newly grown cluster
