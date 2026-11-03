# Smart-Route-Planner-using-Graph-algorithms
A C++-based Smart Route Planner that uses graph data structures and Dijkstra's Algorithm to find the shortest routes between cities. Features include city and route management, BFS and DFS traversal, route distance updates, graph statistics, recent route history, and file handling for data persistence.

# Smart Route Planner

A C++ console-based Smart Route Planner that models a road network using graph data structures and helps users find the shortest route between cities. The application supports city and route management, graph traversal, route distance updates, network statistics, and persistent data storage.

## Project Overview

The Smart Route Planner represents cities as vertices and roads as weighted edges in an undirected graph. Each road has a distance (in kilometres), allowing the application to calculate the shortest path between two cities using Dijkstra's Algorithm.

Users can interact with the application through a menu-driven interface to manage the road network and explore different routes.

## Features

- **Add City:** Add a new city to the road network.
- **Add Route:** Establish a bidirectional route between two cities with a specified distance.
- **Display Road Network:** Display all cities and their connected routes.
- **Find Shortest Route:** Calculate the shortest path and minimum travel distance between two cities.
- **Remove City:** Remove a city and all its associated routes.
- **Remove Route:** Remove an existing connection between two cities.
- **BFS Traversal:** Explore the road network using Breadth-First Search.
- **Search City:** Check whether a particular city exists in the network.
- **Update Route Distance:** Modify the distance of an existing route.
- **DFS Traversal:** Explore the road network using Depth-First Search.
- **Graph Statistics:** Display total cities, total routes, average degree, and the most connected city.
- **Recent Route History:** Display the five most recently searched routes.

## Technologies Used

- **Programming Language:** C++
- **Data Structures:**
  - Graph (Adjacency List)
  - Unordered Map
  - Vector
  - Queue
  - Unordered Set
  - Deque
  - Priority Queue
- **Algorithms:**
  - Dijkstra's Shortest Path Algorithm
  - Breadth-First Search (BFS)
  - Depth-First Search (DFS)
- **File Handling:** C++ File I/O

## Project Structure

```text
Smart-Route-Planner/
│
├── include/
│   ├── Graph.h
│   ├── Menu.h
│   └── FileManager.h
│
├── src/
│   ├── Graph.cpp
│   ├── Menu.cpp
│   └── FileManager.cpp
│
├── data/
│   ├── cities.txt
│   └── routes.txt
│
├── screenshots/
│   ├── menu.png
│   ├── add-city.png
│   ├── add-route.png
│   ├── diplay-route-network.png
│   ├── remove-city.png
│   ├── remove-route.png
│   └── shortest-path.png
│
├── main.cpp
└── README.md
```

## Algorithms Implemented

### 1. Dijkstra's Shortest Path Algorithm

Used to calculate the minimum distance between a source city and a destination city.

- Uses a priority queue to process cities with the smallest known distance.
- Updates distances whenever a shorter path is discovered.
- Reconstructs and displays the shortest route.
- Displays the total distance in kilometres.

### 2. Breadth-First Search (BFS)

- Uses a queue to traverse the graph.
- Visits neighbouring cities level by level.
- Uses a visited set to avoid revisiting cities.

### 3. Depth-First Search (DFS)

- Uses recursion to explore connected cities.
- Visits each reachable city before backtracking.
- Uses a visited set to prevent cycles.


## Sample Road Network

The project includes an initial dataset of cities and road connections.

Some cities included are:

- Chandigarh
- Delhi
- Ludhiana
- Panipat
- Kurukshetra
- Ambala
- Bathinda
- Patiala
- Karnal
- Sangrur

Example route data:

```text
Ambala Chandigarh 45
Delhi Panipat 109
Khanna Ludhiana 42
Bathinda Muktsar 55
```

## Data Persistence

The application uses file handling to maintain the road network between executions.

- `cities.txt` stores the list of cities.
- `routes.txt` stores connections and their distances.
- Existing data is loaded when the application starts.
- Updated data is saved when the user exits the application.

## Future Improvements

- Integrate Google Maps or OpenStreetMap APIs.
- Add graphical visualization of the road network.
- Implement estimated travel time calculations.
- Introduce traffic-aware route optimization.
- Develop a GUI or web-based interface.
- Support multiple route preferences, such as shortest distance and fastest travel time.

## Author

**Srishti Mishra**

