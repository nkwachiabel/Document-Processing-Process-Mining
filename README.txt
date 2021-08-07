The given data set is in MXML format which represents one of the standard formats for the process mining analysis using the ProM framework. 
The file contains data about a document processing process. The data is grouped into process instances and the file contains 18352 process instances. 
Each process instance has its own unique identifier and is marked for example:


<ProcessInstance id="1" description="Real process instance">
…
</ProcessInstance>

The process instances consist of events which are marked as:
<AuditTrailEntry>
…
</AuditTrailEntry>

Each event has a set of attributes that describes the event, and those attributes are the following:

1. Name of the event: 
<WorkflowModelElement>Register</WorkflowModelElement>

2. Type of the event, which can have two values: start (when the event started) and complete (when the event finished)
<EventType >complete</EventType>

3. Time of event execution: 
<Timestamp>2014-04-02T09:00:48.000+01:00</Timestamp>

4. The user that has executed the activity: 
<Originator>System</Originator>

Automatic activities are marked as System. Data in the remaining users is hidden and they are marked as: group1, group2 etc.