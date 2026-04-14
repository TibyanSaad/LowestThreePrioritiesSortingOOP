# Sort and Serve (Object-Oriented Java Program)

## Overview
This project is an **object-oriented refactor** of the original *Sort and Serve* program.  
It accepts both **STDIN (interactive input)** and **CLI arguments** to process complaint priorities. The program sorts the priorities using either **Selection Sort** or **Bubble Sort** and returns the **lowest three priorities** for the intern queue.

## Features
- Accepts input via:
  - **Command Line Arguments (CLI)**: `java InternQueueSorter --algorithm=selection 10,8,2,6,4`
  - **Standard Input (STDIN)**: asks user for algorithm choice and priorities
- Validates input format (must be comma-separated integers)
- Provides two sorting strategies:
  - **Selection Sort** (default)
  - **Bubble Sort**
- Returns the **three lowest priorities** after sorting

## Core Classes
1. **InternQueueSorter**  
   - Main of the program  
   - Combines and runs all classes and methods  
   - Handles CLI and STDIN input  

2. **BubbleSort**  
   - Implements the bubble sort algorithm  
   - Sorts priorities in ascending order  

3. **SelectionSort**  
   - Implements the selection sort algorithm  
   - Sorts priorities in ascending order  

4. **InputParser**  
   - Validates input format  
   - Ensures priorities are comma-separated integers  
   - Converts input into an integer array  

5. **ComplaintService**  
   - Checks the priorities array  
   - Ensures at least 3 priorities are provided  
   - Returns the **lowest three priorities**  

## How to Run (Windows CMD)
1. Navigate to your project folder:
   ```cmd
   cd C:\Users\YourName\SortAndServeOOP\src
2. Compile the program:
   ```cmd
   javac InternQueueSorter.java
3. Run the program with an algorithm (if algoritm not specified selection sort is default):
   ```cmd
   java InternQueueSorter --algorithm=selection 10,8,2,6,4
   java InternQueueSorter --algorithm=bubble 10,8,2,6,4
   java InternQueueSorter 10,8,2,6,4
