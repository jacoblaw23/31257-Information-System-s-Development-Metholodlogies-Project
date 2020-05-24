# Title
# Acknowledgements
# Executive Summary
# Contents
1. [Problem Definition](#Problem)
    * 1.1. [Assumptions](#Assumptions)
2. [Business Objectives](#Business)
3. [Stakeholders](#Stakeholders)
    * 3.1. [Empathy Maps](#Empathy)
        * 3.1.1. [Customer](#Empathy--Customer)
        * 3.1.2. [Relationship Manager](#Empathy--RM)
        * 3.1.3. [Branch Manager](#Empathy--BM)
    * 3.2. [POV Statements](#POV)
        * 3.2.1. [Customer](#POV--Customer)
        * 3.2.2. [Relationship Manager](#POV--RM)
        * 3.2.3. [Branch Manager](#POV--BM)
    * 3.3. [HMW Statements](#HMW)
        * 3.3.1. [Customer](#HMW--Customer)
        * 3.3.2. [Relationship Manager](#HMW--RM)
        * 3.3.3. [Branch Manager](#HMW--BM)
4. [Reflection Statement](#Reflection)
5. [Modelling](#Modelling)
    * 5.1. [User Stories](#Modelling--Stories)
    * 5.2. [Use Case Diagrams](#Modelling--UseCase)
    * 5.3. [Activity Diagrams](#Modelling--Activity)
    * 5.4. [Class Diagrams](#Modelling--Class)
    * 5.5. Collaboration or Sequence Diagrams
6. [Analysis](#Analysis)
7. [References](#References)
8. [Appendix](#Appendix)


# 1. Problem Definition <a name="Problem"></a>
The business seeks to enhance the operation of their in-house call management centre (CMC) in order to improve the customer experience. Customers often complain about their experience with the relationship manager (RM), describing them as unknowledgeable about their desired travel package and (when being sold products) expressing disinterest in the product being sold, resulting in lost sales. To improve the customer experience and increase profits, the business should implement an automatic call routing system matching customers to an appropriate RM.

## 1.1. Assumptions <a name="Assumptions"></a>
**Current Process**
* Customers are complaining about poor experiences when purchasing travel packages
* Customers are complaining about poor experiences when being sold travel packages
* CMC employees receive calls
* CMC employees transfer customers to RMs
* CMC employees transfer customers to some RMs more than others
* RMs sometimes conduct random sales pitches to many customers in order to meet sales numbers
* Customers are waiting for more than a certain period to get answered by an RM just hang up

**Proposed System**
* Customers create unique profiles according to CMC employee instructions before being transferred to RMs
* CMC employees receive calls when automatic routing is unavailable
* CMC employees receive calls when automatic routing fails to find a suitable RM
* The scripts used for sales pitches are created by the business and stored in a fixed location for the system to access
* Calls that are not answered by RM for a specific package are routed to an automated voicemail system
* Calls received are sorted based on whether customer is an ongoing client or a new Potential client
* A supporting tool to create customer profiles exists, called Profiler Tool.


# 2. Business Objectives <a name="Business"></a>
* Speed Up Responses and Reduce Abandons; fast response times and low abandon rates.
* Boost Customer Satisfaction
* Increase the Effectiveness of the Service Recovery Programmes
* Improve Forecast Accuracy; ensure customers don’t have to wait for an answer, getting the numbers right is essential
* Minimise inbound call costs by reducing per-call handling time
* Reduce customer wait times
* The system effectively matches customer with an RM.
* Reduce Customer Effort

An investigation into the source of customer complaints revealed the following issues:
* RMs were sometimes unable to cope with the large number of travel packages available for purchase
* RMs were sometimes unable to cope with the number of customers being transferred to them; customer put on hold
* RMs were sometimes unable to sell products to customers due to cultural differences
* RMs were sometimes unable to communicate with customers due to language barriers
* RMs were sometimes conducting random sales pitches to many customers in order to meet sales numbers

The business aims to resolve these issues using an IT solution, with the goal being an improved customer experience.


# 3. Stakeholders <a name="Stakeholders"></a>
Stakeholders for the proposed solution are described in the table below.

![Stakeholders](diagrams/stakeholders.png)

## 3.1. Empathy Maps <a name="Empathy"></a>
### 3.1.1. Customer <a name="Empathy--Customer"></a>
![Empathy Map - Customer](/diagrams/empathy_maps/Customer.png)

### 3.1.2. Relationship Manager <a name="Empathy--RM"></a>
![Empathy Map - Relationship Manager](/diagrams/empathy_maps/RM.jpeg)

### 3.1.3. Branch Manager <a name="Empathy--BM"></a>
![Empathy Map - Branch Manager](/diagrams/empathy_maps/BM.png)


## 3.2. POV Statements <a name="POV"></a>
### 3.2.1. Customer <a name="POV--Customer"></a>
The customer needs to talk to the appropriate person over the phone to fulfil their needs as their needs will be filled by a RM whose speciality department matches their needs.

### 3.2.2. Relationship Manager <a name="POV--RM"></a>
The relationship manager needs to receive calls from customers that match their specialities, because they will be able to help customers better as they are familiar with the specific area.

### 3.2.3. Branch Manager <a name="POV--BM"></a>
The branch manager needs to increase customer retention by improving customer experience through the process of assigning calls to RMs which are more suited to their skillset. 


## 3.3. HMW Statements <a name="HMW"></a>
### 3.3.1. Customer <a name="HMW--Customer"></a>
* HMW connect to the correct department when calling?
* HMW know the RM we are matched to matches our needs?

### 3.3.2. Relationship Manager <a name="HMW--RM"></a>
*	HMW receive the calls specifically that match our speciality?
*	HMW make this easier for us ?

### 3.3.3. Branch Manager <a name="HMW--BM"></a>
*	HMW ensure the customers are satisfied with the service received?
*	HMW ensure customers receive the right packages?


# 4. Reflection Statement <a name="Reflection"></a>
The team have conducted interviews with the stakeholders about the current system from their experiences from using the current system. When the team spoke to the customer, they specified that they wanted to speak to the right person that will be able to fulfil their needs, as that appropriate person will be able to match their needs based on the information they provide to that person their speaking with over the phone. The feedback we received from the customer is that the current system has given them a poor experience when purchasing travel packages, also how they are being sold the packages that are available from the travel company is considered to a pain point in their perspective,another thing they mentioned is when they were waiting for more than a certain period of time to speak to the right relationship manager they would just hang up.


# 5. Modelling <a name="Modelling"></a>
## 5.1. User Stories <a name="Modelling--Stories></a>
1) As a branch manager, i want to develop an information system so that i can improve the operation of the in-house call management centre.
2) As a customer i need to fill in some personal details on profiler tool, so that i can create a customer profile.
3) As an RM, i need to fill out a 10 minute profile and skill questionaire, so that my profile can be initialised at hiring.
4) As a customer, i have to create a customer profile so that i can be matched with an RM according to social and cultural segments. 
5) As a Relationship Manager (RM) i want to provide effective service and assistance to customers, so that i can improve performance sales for holiday packages.
6) As a customer i want to be matched with an RM based on performance and product knowledge, so that i can receive adequate information and service.  
7) As an RM i want to educate myself about the new system, so that i can sell packages and serve customers more effectively and efficiently.
8) As a customer, i want to score the RM's service out of 1-10 after my call, so that i can provide feedback about the system.

## 5.2. Use Case Diagrams <a name="Modelling--UseCase"></a>
## 5.3. Activity Diagrams <a name="Modelling--Activity"></a>
## 5.4. Class Diagrams <a name="Modelling--Class"></a>
## 5.5. Collaboration or Sequence Diagrams <a name=""></a>


# 6. Analysis <a name="Analysis"></a>
In the process of developing a new information system to improve the operation of the in house call management cenre (CMC), a number of competitive advantages are gained. The major advantage for the call centre would be improved and smooth operations. Some potential benefits for the call centre include the reduction in inbound call costs by reducing per-call handling time, the ability to carry out more effective and efficient calls, reduction in customer wait times, improved call routing and dynamic call flow control for both inbound and outbound calls, improved customer service, improved RM performance, higher sales of travel packages, increased customer attraction & loyalty, decreased manual labour, reduction in operation/administration expenses, higher profits.
However, whilst there are a number of benefits derived from an upgraded information system, there are also possible adverse effects for the business if its information system project fails.

"Identify and discuss the possible adverse effects for this Business if its information system project fails"
- loss of money, can lost customer base


# References <a name="References"></a>
# Appendix <a name="Appendix"></a>
