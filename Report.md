![Cover Sheet](assets/Cover%20Sheet.png)

# Presentation
https://www.youtube.com/watch?v=G22axvqy-GQ

# Executive Summary
The business aims to improve its current in-house call management centre (CMC) system to adjust the flow rate to suitable relationship managers (RM). The business has taken into consideration customer complaints. Currently, customers have complained about the poor experiences when being sold travel packages where they were served by a RM who they thought did not have the knowledge for their desired travel package. Additionally, long waiting periods on inbound calls for customers to connect to a RM have also been identified.

This report highlights the 3 main characteristics the improved system will focus on: inbound calls, outbound calls and the supporting profiling tool. It will examine the importance of these characteristics in improving the current system while considering customer complaints. The proposed system will ask each Customer and RM to create profiles using the Profiler Tool to ensure customers will be matched to an appropriate RM. These profiles will then be stored in a database. Inbound calls will be forwarded to the RM through the improved system. However, if no RM is available the system will direct the call to an interactive voice response. Similarly, in any outbound calls where the potential buyer is unavailable, the system will leave a message for that person.

# Contents
1. [Problem Definition](#Problem)
    * 1.1. [Assumptions](#Assumptions)
2. [Business Objectives](#Business)
3. [Stakeholders](#Stakeholders)
    * 3.1. [Empathy Maps](#Empathy)
    * 3.2. [POV Statements](#POV)
        * 3.2.1. [Customer](#POV--Customer)
        * 3.2.2. [Relationship Manager](#POV--RM)
        * 3.2.3. [Branch Manager](#POV--BM)
    * 3.3. [HMW Statements](#HMW)
        * 3.3.1. [Customer](#HMW--Customer)
        * 3.3.2. [Relationship Manager](#HMW--RM)
        * 3.3.3. [Branch Manager](#HMW--BM)
4. [Reflection Statement](#Reflection)
    * 4.1. [Use of Scrum](#Reflection--Scrum)
5. [Modelling](#Modelling)
    * 5.1. [User Stories](#Modelling--Stories)
    * 5.2. [Use Case Diagrams](#Modelling--UseCase)
    * 5.3. [Use Case Narratives](#Modelling--UseCaseNarratives)
    * 5.4. [Activity Diagrams](#Modelling--Activity)
    * 5.5. [Class Diagram](#Modelling--Class)
    * 5.6. [Sequence Diagrams](#Modelling--Sequence)
6. [Analysis](#Analysis)
7. [References](#References)


# 1. Problem Definition <a name="Problem"></a>
The business seeks to enhance the operation of their in-house call management centre (CMC) in order to improve the customer experience. Customers often complain about their experience with the relationship manager (RM), describing them as unknowledgeable about their desired travel package and (when being sold products) expressing disinterest in the product being sold, resulting in lost sales. To improve the customer experience and increase profits, the business should implement an automatic call routing system matching customers to an appropriate RM.

## 1.1. Assumptions <a name="Assumptions"></a>
**Current Process:**
* Customers are complaining about poor experiences when purchasing travel packages
* Customers are complaining about poor experiences when being sold travel packages
* CMC employees receive calls
* CMC employees transfer customers to RMs
* CMC employees transfer customers to some RMs more than others
* RMs sometimes conduct random sales pitches to many customers in order to meet sales numbers
* Customers are waiting for more than a certain period to get answered by an RM just hang up
* Customers are told to call the next day when calling after hours

**Proposed System:**
* CMC employees receive calls when automatic routing is unavailable
* CMC employees receive calls when automatic routing fails to find a suitable RM
* The scripts used for sales pitches are created by the business and stored in a fixed location for the system to access
* Calls that are not answered by RM for a specific package are routed to an automated voicemail system
* Calls received are sorted based on whether customer is an ongoing client or a new Potential client
* A supporting tool to create customer profiles exists, called Profiler Tool.


# 2. Business Objectives <a name="Business"></a>
* Increase response times and reduce abandon rates
* Increase customer satisfaction; customers want fast, positive outcomes. 
* Increase the effectiveness of service recovery programs; ensures the organisation responds directly customer feedback and the business can quickly implement actions to be taken if the system fails.
* Increase forecast accuracy; customers should not wait to be connected to the correct RM
* Increase the probability of successful sales by intelligently matching customers to travel packages
* Match customers to knowledgable RMs; ensure customers are paired up with RMs that have similarities and efficient product knowledge.
* Minimise inbound call costs by reducing per-call handling times
* Reduce customer wait times; customer's shoudn't be placed on hold for too long, the new system aims to make this process easier.
* Reduce customer effort; make the process for inbound calls easier and smooth for customers.


# 3. Stakeholders <a name="Stakeholders"></a>
Stakeholders for the proposed solution are described in the table below.

![Stakeholders](diagrams/Stakeholders.jpg)

## 3.1. Empathy Maps <a name="Empathy"></a>
**Customer:**<br>
![Empathy Map - Customer](/diagrams/emaps/Customer.png)

**Relationship Manager:**<br>
![Empathy Map - Relationship Manager](/diagrams/emaps/RM.jpeg)

**Branch Manager:**<br>
![Empathy Map - Branch Manager](/diagrams/emaps/BM.png)


## 3.2. POV Statements <a name="POV"></a>
### 3.2.1. Customer <a name="POV--Customer"></a>
The customer interested in a travel package needs to connect with a knowledgable person (RM) because otherwise the customer will obtain incomplete or incorrect information, and have an unsatisfying experience.

### 3.2.2. Relationship Manager <a name="POV--RM"></a>
The relationship manager (RM) needs to receive calls from customers interested in a travel package that the RM specialises in because then they can provide complete and correct information.

The relationship manager needs to spend less time transferring calls to more suitable colleagues because that time is wasted.

### 3.2.3. Branch Manager <a name="POV--BM"></a>
The branch manager needs to improve the customer experience because customers are becoming increasingly dissatisfied with the available services.


## 3.3. HMW Statements <a name="HMW"></a>
### 3.3.1. Customer <a name="HMW--Customer"></a>
* HMW connect customers to a knowledgable RM with an appropriate level of cultural understanding?
* HMW connect customers to a complete and correct source of travel package information?

### 3.3.2. Relationship Manager <a name="HMW--RM"></a>
* HMW ensure that RMs receive calls from customers related to their specialised understanding?
* HMW reduce the amount of redundant or unnecessary work performed by RMs?

### 3.3.3. Branch Manager <a name="HMW--BM"></a>
* HMW improve the customer experience?
* HMW improve customer satisfaction?
* HMW ensure customers are sold the appropriate travel package?


# 4. Reflection Statement <a name="Reflection"></a>
The team have conducted interviews with the stakeholders about the current system from their experiences from using the current system. When the team spoke to the customer, they specified that they wanted to speak to the right person that will be able to fulfil their needs, as that appropriate person will be able to match their needs based on the information they provide to that person their speaking with over the phone. The feedback we received from the customer is that the current system has given them a poor experience when purchasing travel packages, also how they are being sold the packages that are available from the travel company is considered to a pain point in their perspective,another thing they mentioned is when they were waiting for more than a certain period of time to speak to the right relationship manager they would just hang up.

## 4.1. Use of Scrum <a name="Reflection--Scrum"></a>
**Sprint Planning:** Sprint planning was conducted each week during the allocated tutorial session. Group members were assigned tasks to complete during the week and we attempted to identify and remove obstacles where possible.

The IT solution report was developed over several weeks with each week adding more content to the report. Please refer to the below table describing when different sections of the report were started. Diagrams were initially presented internally as drafts and then committed and revised on GitHub in later weeks.

| Week | Content |
|:----:|---------|
| 1 | <ul><li>Problem definition</li><li>Assumptions</li><li>Stakeholders</li></ul> |
| 2 | <ul><li>Report structure</li><li>Business objectives</li><li>User stories</li><li>POV and HMW statements</li><li>Draft diagrams</li></ul> |
| 3 | <ul><li>Use case diagrams</li><li>Class diagram</li><li>Competitive advantages and disadvantages</li></ul> |
| 4 | <ul><li>Use case narratives and accompanying diagrams</li><li>Finalise report</li><li>Video presentation</li><li>Executive summary</li></ul> |

# 5. Modelling <a name="Modelling"></a>
## 5.1. User Stories <a name="Modelling--Stories"></a>
| US001 | Priority | Estimate |
|-------|:--------:|:--------:|
| As a customer, I want to communicate with an employee that understands the product I am searching for so that I can make better purchases. | H | High |
| <b>Acceptance Criteria:</b><br> <ul><li>Customer is connected to a RM that understands the desired product</li><li>Customer is connected to a RM that understands contextual knowledge about the product such as cultural traditions</li></ul> |

<br>

| US002 | Priority | Estimate |
|-------|:--------:|:--------:|
| As a customer, I want to comment on my experience with an employee so that I know my opinion matters to the business. | M | Low |
| <b>Acceptance Criteria:</b><br> <ul><li>Customer has the option to rate their experience after each phone call</li><li>Customer has the option to comment on their experience after each phone call</li></ul> |

<br>

| US003 | Priority | Estimate |
|-------|:--------:|:--------:|
| As a customer, I want to create a personal profile so that I can receive personalised service in the future. | L | Low |
| <b>Acceptance Criteria:</b><br> <ul><li>Customer can create a personal profile by communicating with CMC employee</li><li>Customer can update their personal profile at any time</li></ul> |

<br>

| US004 | Priority | Estimate |
|-------|:--------:|:--------:|
| As a relationship manager, I want to connect with customers that I can provide effective service to so that I can create a strong relationship with the customer. | H | Medium |
| <b>Acceptance Criteria:</b><br> <ul><li>RM is connected with customers they are capable of providing effective service to</li></ul> |

<br>

| US005 | Priority | Estimate |
|-------|:--------:|:--------:|
| As a relationship manager, I want to connect with customers that I can provide effective service to so that I do not need to transfer calls as often. | H | Medium |
| <b>Acceptance Criteria:</b><br> <ul><li>RM does not transfer calls as often</li></ul> |

<br>

| US006 | Priority | Estimate |
|-------|:--------:|:--------:|
| As a relationship manager, I want to quickly find product details so that I can respond to questions in a timely manner. | L | Medium |
| <b>Acceptance Criteria:</b><br> <ul><li>RM can search for specific products and product information</li><li>Product information appears within 5 seconds</li><li>Product information is easy to read</li></ul> |

<br>

| US007 | Priority | Estimate |
|-------|:--------:|:--------:|
| As a relationship manager, I want to sell customers products they are interested in so that I make more sales. | H | High |
| <b>Acceptance Criteria:</b><br> <ul><li>System creates product recommendations using purchase history and other customer information that interest the customer</li></ul> |

<br>

| US008 | Priority | Estimate |
|-------|:--------:|:--------:|
| As a relationship manager, I want to create a personal profile with a description of my skills so that I can be matched with customers I can provide effective service to. | H | Low |
| <b>Acceptance Criteria:</b><br> <ul><li>RM can create a personal profile as part of the onboarding process</li><li>RM can update their personal profile at any time</li><li>RM can update their skills at any time</li></ul> |

<br>

| US009 | Priority | Estimate |
|-------|:--------:|:--------:|
| As a branch manager, I want to put customers in a waiting queue when no RM is available so that customers can connect to available RMs as soon as possible. | M | Medium |
| <b>Acceptance Criteria:</b><br> <ul><li>Customers are put in a waiting queue when no RM is available</li><li>Customers are connected with available RMs as soon as the RM becomes available</li><li>Customers are served in order of purchase potential (ties are settled by order of appearance)</li></ul> |

<br>

| US010 | Priority | Estimate |
|-------|:--------:|:--------:|
| As a branch manager, I want RMs to use a script when selling products so that the customer experience is more consistent and effective. | L | Low |
| <b>Acceptance Criteria:</b><br> <ul><li>RM can view product-specific sale scripts when making sales</li></ul> |


## 5.2. Use Case Diagrams <a name="Modelling--UseCase"></a>
**Customer:**<br>
![Customer Calls the Business](diagrams/ucase/Customer.png?)

**Relationship Manager:**<br>
![RM Making Sales](diagrams/ucase/Business.png)

**Profiler Tool:**<br>
![Profiler Tool](diagrams/ucase/Tool.png)

## 5.3. Use Case Narratives <a name="Modelling--UseCaseNarratives"></a>
**US001:**<br>
[US001 Use Case Narrative](narratives/US001.pdf)

**US003:**<br>
![US003 Use Case Narrative](narratives/US003.docx)

**US007:**<br>
![US007 Use Case Narrative](narratives/US007.jpg)

## 5.4. Activity Diagrams <a name="Modelling--Activity"></a>
**US001:**<br>
![US001 Activity Diagram](https://user-images.githubusercontent.com/62576436/83351355-74dff180-a386-11ea-9aa4-5b2ed4751954.png)

**US003:**<br>
![US003 Activity Diagram](diagrams/activity/US003.png)

**US007:**<br>
![US007 Activity Diagram](diagrams/activity/US007.png)

## 5.5. Class Diagram <a name="Modelling--Class"></a>
![Class Diagram](diagrams/Class%20Diagram.png)

## 5.6. Sequence Diagrams <a name="Modelling--Sequence"></a>
**US001:**<br>
![US001 sequence diagram](https://user-images.githubusercontent.com/62576436/83351378-9d67eb80-a386-11ea-8844-e1814871e515.png)

**US003:**<br>
![US003 Sequence Diagram](diagrams/sequence/US003.png)

**US007:**<br>
![US007 Sequence Diagram](diagrams/sequence/US007.jpeg)

# 6. Analysis <a name="Analysis"></a>
The IT solution proposed in this report to improve the operation of the in-house CMC gives the business a competitive edge, compared to similar companies. At present, customers observe a consistent issue with their experiences purchasing products with the business and similar companies: the connected employee is not always capable of providing them with assistance. As a result, customers have the subconscious assumption that this experience cannot be improved. The proposed solution undercuts this assumption, creating a new standard for their interaction with similar companies and, as a result, the business appears to provide better customer service than their competition.

The proposed solution also:
* Automates call flow control
* Reduces the number of delays customers experience in the process
* Reduces the number of employees involved in the process

In reducing the above numbers, the proposed solution reduces costs (reduced call-handling time and administrative costs) and allows employees to work on more value-adding tasks. Also, by streamlining the process, it becomes more suited for further automation.

As described above, the business stands to gain a significant number of customers by being the innovator in customer experience. By not implementing the proposed solution first the business essentially gives up these customers to the competition: the returns from investing into the proposed solution decrease over time, as the risk of competing companies developing similar solutions first increases.

Also, the business has recognised the need to streamline the process and recognised the decreasing quality of their customer experience. The proposed solution is designed to address these concerns, so unless an alternative solution is presented these issues will not be addressed; the customer experience will continue to decline. Considering the scale of the business, it is also possible that some employees will become dissatisfied with their work and leave the business, forcing the business to hire a replacement and introducing more costs. However, it is also possible that some employees will leave the business when they learn their work is being automated.

The business stands to gain a significant number of customers by innovating and implementing the proposed solution before its competitors. In comparison, the negative consequences of implementing the proposed solution are insignificant. It is recommended that the business implements the proposed solution in a timely manner.

# References <a name="References"></a>
* Lucidchart. 2020. [Online]. Available at: https://www.lucidchart.com/ [Accessed 31 May 2020].
* 2020 ‘Lecture 8 - OO Techniques’, 31257, Lecture , UTS, Sydney. [Online]. Available at: https://online.uts.edu.au/webapps/blackboard/content/listContent.jsp?course_id=_41893_1&content_id=_3756258_1 [Accessed 31 May 2020].
