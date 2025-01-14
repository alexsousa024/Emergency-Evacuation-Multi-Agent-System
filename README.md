# Multi-Agent Emergency Evacuation System
# Overview
This project involves the development of a multi-agent system designed to manage and coordinate emergency evacuations in large buildings or complexes. Using frameworks such as **SPADE**, the system simulates the interactions between various agents, including occupants, emergency responders, and building management systems, to ensure a safe and efficient evacuation during emergencies.

# Features
Agents and Roles
Occupants:

Knowledgeable Occupants: Aware of the building structure and capable of calculating routes autonomously.
Non-Knowledgeable Occupants: Rely on assistance from other agents or occupants to navigate.
Building Management System (BMS):

Activates alarms and provides real-time updates to other agents.

# Emergency Responders:

Firefighters: Extinguish fires and assist occupants in need.
Security Agents: Patrol the building, guide occupants to the safest exits, and coordinate evacuation routes.
Technologies Used
Python: Core implementation of the system and agent behaviors.
SPADE/JADE: For creating and managing multi-agent interactions.
Pathfinding Algorithms:
Dijkstra's Algorithm: Used by security agents for optimal route calculation.
Bresenham's Algorithm: Guides occupants to visible exits.
# Project Structure

project/
├── BuildingManagement.py     # Manages building systems and alarms
├── environment.py            # Defines the simulation environment
├── fire.py                   # Models fire behavior and spread
├── FiremanAgent.py           # Defines firefighter agents
├── interface.py              # Handles user interaction and simulation visualization
├── main.py                   # Main script to initialize and run the simulation
├── OccupantAgent.py          # Defines occupant agents
├── SecurityAgent.py          # Defines security agents
├── Urgent and Emergency Action Plan by Slidesgo.pdf # Detailed project presentation\

# Functionality and Interaction
Emergency Workflow
The Building Management System detects a fire and activates the alarm.
Occupants:
Knowledgeable: Navigate to the nearest exit.
Non-Knowledgeable: Request help from firefighters or other occupants.
Security Agents:
Provide optimal routes to occupants.
Monitor and report on evacuation progress.
Firefighters:
Extinguish fires and respond to help requests.
Communication Protocols
Agents use direct messages to share:
Fire location.
Optimal evacuation routes.
Requests for assistance.
Evaluation and Results
Simulated Scenarios:

Tested with varying building sizes and agent counts.
Results recorded over 20 trials for each configuration.
Findings:

Smaller buildings: High efficiency and lower fatality rates.
Larger buildings: Increased fatalities due to:
Difficulty locating non-knowledgeable occupants.
Limited effectiveness of patrols by security agents.
Conclusion:

The system demonstrates realistic evacuation scenarios with agents prioritizing survival and cooperation.
Results validate the effectiveness of the multi-agent approach, especially in smaller settings.
Installation
Prerequisites
Python 3.8+
Libraries: matplotlib, numpy, networkx
