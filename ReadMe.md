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

Variable Parameters
-------------------
* Grid-size x and y (particles have a size of 1x1)
* Initial number of seed particles
* Whether movement can wrap the edges of the screen or not

Program planning
----------------
1) The particles will be stored as an array of objects
2) Each particle will be an object with a number of properties stored there-in:
* Particle coordinates
* Array of coordinates of spaces to check around the particle
3) For a cluster, there will be one particle that serves as the main anchor, any other particles that are attached as part of the cluster will have their coordinates stored in a array within a property of the Anchor Particle's object.
Cluster version of stored properties list:
* Main Anchor coordinates
* Array of coordinates of particles included in the cluster
* Array of coordinates of spaces to check around the cluster

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
* 1.0 - Functional cluster-cluster aggregation behavior ending with one cluster

* 1.1 - Design and set-up SQL database
* 1.2 - Store coordinates for each particle/cluster after a movement is made.
* 1.3 - Ability to query and display history of particle/cluster movement
* 2.0 - Full-Stack storage of particle and cluster movement history

* 3.0 - Change a moment in history and save the new alternate history

* 4.0 - Ability to compare the two histories after a change in one moment using a slider to be able to move forward and backward in history.
