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
![alt text](https://github.com/nkwachiabel/Document-Processing-Process-Mining/blob/main/Images/Data%20Overview.jpg?raw=true)
The given set of data contains information about the process of document processing. The process of processing documents contains the following activities: Receiving a Document, Creating a new Case, Investing Document into a new Case and so on. The data set contains information about the event name, event type, time of the event's execution and the participant whose execution the event is related to.

The data is grouped into process instances and the file contains 18352 process instances with 149,693 events and 8 groups of users (7 humans and 1 system). The process contains 10 activites as seen in the image.

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
1. <b>Process flow of the document processing activity:</b> This analysis helped in identifying the actual process flow of the document processing activities with three variants.
   - Variant 1 contains 9,384 and represented 51.13% of all cases. This covers the expected process from <b>Receiving the Document</b> until the <b>End</b> of the document processing activity.
   - Variant 2 contains 4,773 and represented 26.01% of all cases. This Variant only contains 3 activities (i.e., Register, Receiving a Document, Placing documents in an existing Case). The documents that fall into this variant are not invested in a new Case (i.e., <b>Investing Document into a new Case</b> activity is not performed). I believe this is because these documents have been received earlier and have an existing Case for them because they are placed in an existing case (i.e., <b>Placing documents in an existing Case</b> activity) rather than invested in a new case. In addition, the cases in this Variant do not contain the activity <b>Generate and send an outgoing Document</b>. Due to limited information, I can't confirm why this documents are not sent out.
   - Variant 3 contains 4,195 cases and represented 22.86% of all cases. This is similar to Variant 1, with the same activities. The difference was that the cases which falls into this variants had to be reworked on. The rework was done on the <b>Work on the Case</b> and <b>Confirmation of the work on the Case</b> activities. We do not see this as a deviation from the process.
  
2. Most of the time is spent in <b>Confirming of the work on the Case</b> and <b>Marking Case</b> activity. These activities takes an average of 24 and 18 minutes respectively.



# Contribution
Contributions to this repository are welcome! If you encounter any issues or have suggestions for improvement, please open an issue or submit a pull request.

# Contact
For any questions or inquiries, please contact nkwachiabel@gmail.com
