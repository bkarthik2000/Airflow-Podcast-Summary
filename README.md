# Project Overview

In this project, we'll create a data pipeline using Airflow.  The pipeline will download podcast episodes and automatically transcribe them using speech recognition.  We'll store our results in a SQLite database that we can easily query.

We have alternative tech stacks to do this project but we prefer Airflow for following reasons:
* We can schedule the project to run daily
* Each task can run independently, and we get error logs
* We can easily parallelize tasks and run in the cloud if we want to
* We can extend this project more easily (add speech recognition, summaries, etc) using Airflow


**Project Steps**

* Download the podcast metadata xml and parse
* Create a SQLite database to hold podcast metadata
* Download the podcast audio files using requests
* Transcribe the audio files using vosk


File overview:

* `podcast_summary.py` - the code to create a data pipeline
* `steps.md` - a description of the steps you'll need to follow to complete the project.  



## Installation

To follow this project, please install the following locally:

* Airflow 2.3+
* Python 3.8+
* Python packages
    * pandas
    * sqlite3
    * xmltodict
    * requests
    * vosk
    * pydub



