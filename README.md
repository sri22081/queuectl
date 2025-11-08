# queuectl
 
## QueueCTL – Background Job Queue System

## Overview
QueueCTL is a command-line (CLI) based background job queue system developed in Python using SQLite for persistent storage.  
It allows you to enqueue and manage background jobs, process them using worker processes, automatically retry failed jobs with exponential backoff, and handle permanently failed jobs through a Dead Letter Queue (DLQ).

This project was developed as part of a Backend Developer Internship Assignment.


 ## Features
- Enqueue and manage background jobs  
- Persistent job storage using SQLite  
- Multiple job states: `pending`, `completed`, `failed`, and `dead`  
- Automatic retries for failed jobs  
- Dead Letter Queue (DLQ) for permanently failed jobs  
- Command-line interface for all operations  
- Compatible with Google Colab, Visual Studio Code, and system terminals  



## Job Lifecycle

State | Description |
 pending -  The job is waiting to be picked up by a worker |
 completed -  The job executed successfully |
 failed - The job failed but is still eligible for retries |
 dead - The job has failed permanently and is moved to the DLQ |


## Tech Stack
- Language: Python   
- Database: SQLite  
- Interface:Command Line (argparse)  
- Supported Platforms: Google Colab  


## File Structure
-queuectl.py # Main Python program (core logic)
-README.md # Project documentation
-demo_test.sh 
