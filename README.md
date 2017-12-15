Luma Technical Interview

Problem Definition	1
Interview Task	1
Weighting Categories	2
Demographic	2
Behavior	2
Patient Model	2
Deliverables	2

Problem Definition

A busy hospital has a list of patients waiting to see a doctor. The waitlist is created sequentially (e.g. patients are added in a fifo order) from the time the patient calls.  Once there is an availability, the front desk calls each patient to offer the appointment in the order they were added to the waitlist. The staff member from the front desk has noticed that she wastes a lot of time trying to find a patient from the waitlist since they’re often not available, don’t pick up the phone, etc.  She would like to generate a better list that will increase her chances of finding a patient in the first few calls. 

Interview Task

Given patient demographics and behavioral data, create an algorithm that will generate an ordered list of patients who will most likely accept the appointment offer.  You will need to process a set of historical patient data to compute a score for each patient that (1 as the lowest, 10 as the highest) that represents the chance of a patient accepting the offer off the waitlist.  Take in consideration that patients who have little behavior data should be randomly added to the top list as to give them a chance to be selected. 

Weighting Categories
Demographic
age  (weighted 10%)  
distance to practice (weighted 10%)

Behavior
number of accepted offers (weighted 30%)  
number of cancelled offers (weighted 30%)  
reply time (how long it took for patients to reply) (weighted 20%)  
Patient Model
ID
Age (in years)
location
Lat
long
acceptedOffers (integer)
canceledOffers (integer)
averageReplyTime (integer, in seconds)
Deliverables
The code should be written as a Node.js as a library that anyone can import and use. It should contain documentation and unit tests that show your understanding of the problem. Once you’re finished, submit a PR to this repo. 

