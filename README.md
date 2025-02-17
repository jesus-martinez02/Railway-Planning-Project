# Railway-Planning-Project
This repository contains the code that implements a Mixed-Integer Linear Program for obtaining the least cost solution for the operation of each scenario in the project of the course Railway Planning and Operations at KTH. It also produces a circulation plan for the provided scenario.

In order to make the code run, it is necessary to install the pulp libary (mor info in https://coin-or.github.io/pulp/) and get an academic license of the Gurobi solver (available at https://www.gurobi.com/academia/academic-program-and-licenses/).

The program reads the number of departures, distance, travel time and minutes between consecutive departures for a given train unit from the file 'scenario.csv'. Additionally the program needs 3 more files to run for each scenario:

- The timetable that has to be satisfied, indicating the hour of the departures and the id of the departure for each origin station. Note that the id's for the departures have to be assigned in chronological order, independently of the origin station.
- The demand for each departure id, sorted by departure id.
- The set of different train units that can be used, including seating capacity, fixed costs and variable costs.

