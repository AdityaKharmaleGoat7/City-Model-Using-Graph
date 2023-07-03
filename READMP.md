
# City Model using Graph Algorithm

This code implements a city model using graph algorithms in C++. The city model represents a network of cities connected by roads, and provides functionality to find the shortest path between cities, identify bridges in the network, and find the minimum spanning tree.

Contributors:
- Aditya Kharmale
- Shreyash Bhanage
- Harshavardhan Tompe
- Vatsal Singhala

## Usage

The code allows you to interact with the city model through a menu-based interface. The available options are as follows:

1. Find shortest path: Find the shortest path between two cities.
2. Find bridges: Identify the bridges in the city network.
3. Find minimum spanning tree: Find the minimum spanning tree of the city network.
4. Find minimum distance between two cities: Find the minimum distance (number of cities) between two given cities.
5. Display City Map: Display the list of cities and their neighbors in the city network.
0. Exit: Quit the program.

To use the code, follow these steps:

1. Compile the code using a C++ compiler.
2. Run the compiled executable.
3. Choose an option from the menu by entering the corresponding number.
4. Follow the instructions on the screen to provide input (e.g., city names).
5. View the results displayed by the program.

## City Model Implementation

The city model is implemented using the following classes:

### City Class

The `City` class represents a city in the city model. It has the following attributes:
- `name`: The name of the city.
- `neighbors`: An unordered map representing the adjacency list of neighboring cities and their corresponding weights (distances).

### CityModel Class

The `CityModel` class represents the city model and provides various functionalities. It has the following methods:
- `addCity(const string& cityName)`: Adds a new city to the city model.
- `addConnection(const string& city1, const string& city2, int weight)`: Adds a connection (road) between two cities with a given weight.
- `findShortestPath(const string& startCity, const string& endCity)`: Finds the shortest path between two cities using Dijkstra's algorithm.
- `findBridges()`: Finds all the bridges (critical connections) in the city model using a modified version of Depth-First Search (DFS) algorithm.
- `findMinimumSpanningTree()`: Finds the minimum spanning tree of the city model using Kruskal's algorithm.
- `displayCityMap()`: Displays the list of cities and their neighbors in the city model.

The `CityModel` class uses various data structures such as unordered maps, priority queues, and vectors to store and process the city model.

## License
Feel free to use and modify the code for your own projects.
