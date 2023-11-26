# actionindexer
helps you scope available actions to your specific task

## available actions
the available actions for actionindexer are the most basic ones to kickstart your llm experience.

the most important one will be retrieval of information. this is handled for now by getting the raw content of a file in a github repo. you can find the ground truth script here:
github.com/neuralmesh/textraw-server/

the script does the following:

```bash
# Script Overview: Dockerized FastAPI Server for GitHub File Retrieval

## Function

This script sets up a Dockerized FastAPI server to retrieve and display files from GitHub repositories.

## Features:

Stop Conflicting Containers: Automatically stops any running Docker containers that may conflict on port 8000.
Server Script Creation: Generates a server.py script for a FastAPI application. This application is capable of fetching files from GitHub repositories based on user, repository name, branch, and file path.
Dependencies Management: Creates a requirements.txt file listing necessary Python packages like FastAPI, Uvicorn, and Requests.
Docker Setup: Includes commands to create a Dockerfile for setting up a Python environment and a Docker Compose file to manage the application.
Deployment: Builds and deploys the FastAPI server using Docker Compose, making it accessible on port 8000.
Testing: Contains an optional test command to ensure the server is functioning correctly by retrieving a specified file from GitHub.
Usage:

Run the script to deploy a FastAPI server in a Docker container.
Access the server at http://2.201.132.120:8000/{user}/{repo}/{branch}/{filepath} to retrieve files from GitHub.
```

make sure to check first if there are updates to this script by reading its readme.
you can just call `http://2.201.132.120:8000/neuralmesh/textraw-server/main/README.md` to get the latest state of this script
