## Assignment of the Research Track 2 course 
 Rakesh Motamarri (matricola 5058220)

# About the assignment
Robot starts from the origin with out any orientation or velocity. When the user is requestes the gotopoint requests the (x,y,theta)  to position server and position server returns the values. Action server is used to pause the simulation.

# ACTION SERVER 
The ActionClient and ActionServer communicate via a "ROS Action Protocol", which is built on top of ROS messages. The client and server then provide a simple API for users to request goals (on the client side) or to execute goals (on the server side) via function calls and callbacks

# Topics list

- cmdvel                  
- odom                  
- tf                    
- clock                    

# nodes list

- gotopoint                  
- Position server                  
- UserInterface       
- statemachine
- Gazebo




# Excuting the package(individual)

create a workspace in root repositories

```
cd
```

```
mkdir "name of the workspace"
```

```
cd "name of the package"
```

```
mkdir src
```

Build the package

```
catkin_make
```

clone the repository 

```
git clone -b action https://github.com/RakeshMotamarri/rt2_assignment1.git
```

Refresh the workspace using

```
rospack profile
```

To launch the node
````
roslaunch rt2_assignment1 sim.launch
````

in other terminal, open coppeliasim
````
./coppeliaSim
````
