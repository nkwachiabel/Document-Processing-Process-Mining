# Document Processing Analysis with Process Mining
This repository showcases a project that leverages process mining techniques to gain valuable insights into the document processing process. By analysing the end-to-end workflow of the process, we can identify bottlenecks and optimise efficiency.


# Project Overview
The goal of this project is to:
1. Utilize process mining to uncover the complete document processing process from purchasing receiving a document to sending out the processed document.
2. Identify inefficiencies and potential process bottlenecks.
3. Generate insights to improve process efficiency.

# Key Features
1. Import and preprocess data downloaded
2. Perform process discovery to create visual process maps and analyse process variations
3. Calculate process performance metrics such as lead time
4. Generate dashboards and visualisations to communicate insights effectively


# Technologies Used
1. Python
2. Pandas
3. Graphviz
4. Jupyter Notebook
5. Matplotlib
6. Microsoft PowerBI

# Data
The given set of data contains information about the process of document processing. The process of processing documents contains the following activities: Receiving a Document, Creating a new Case, Investing Document into a new Case and so on. The data set contains information about the event name, event type, time of the event's execution and the participant whose execution the event is related to.

The data is grouped into process instances and the file contains 18352 process instances.

Each event has a set of attributes that describes the event, and those attributes are the following:

1. case: This is the unique ID of a document/process
2. event: This shows the name of the event that was executed. e.g., register, receiving a document, etc
3. startTime: The time when the event started
4. completeTime: The time when the event was completed
5. description: The description of the event carried out. All events are real process instance
6. org:resource: The anonymised group that has executed the activity. Automatic activities are marked as System while human activities are indicated by their groups i.e., group 1, group 2, etc.

https://doi.org/10.4121/uuid:6df27e59-6221-4ca2-9cc4-65c66588c6eb

### Contributors
University of Sarajevo, Faculty of Electrical Engineering

### Publisher
4TU.Centre for Research Data

This document was gotten from [here](https://data.4tu.nl/articles/dataset/Document_Processing_Event_Logs/12703232)

# Results and Visualisations
Here are some visualisations showcasing the insights obtained from the document processing analysis:



# Contribution
Contributions to this repository are welcome!

# Contact
For any questions or inquiries, please contact nkwachiabel@gmail.com
