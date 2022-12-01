# **Software Requirements Specification**


# **for**


# Volunteer Management System

<p style="text-align: right">
<strong>Version 1.0 approved</strong></p>


<p style="text-align: right">
<strong>Prepared by Andrei Vivar, Raiden Yamaoka and Nduonyi Jack Ukitetu</strong></p>


<p style="text-align: right">
<strong>Weabois</strong></p>


<p style="text-align: right">
<strong>November 25, 2022</strong></p>


**Table of Contents**


[TOC]


**Revision History**


<table>
  <tr>
   <td><strong>Name</strong>
   </td>
   <td><strong>Date</strong>
   </td>
   <td><strong>Reason For Changes</strong>
   </td>
   <td><strong>Version</strong>
   </td>
  </tr>
  <tr>
   <td>Everyone 
   </td>
   <td>11/25/22
   </td>
   <td>Document Creation
   </td>
   <td>1.0
   </td>
  </tr>
</table>




1. 
**Introduction**


    1. 
**Purpose**
The purpose of this SRS is to describe the software requirements specifications for the first version of the Volunteer Management System. This system provides administrators and managers an environment where they can manage new volunteers and volunteer requests in a single organized system. This version contains the basic functionalities for users. This document describes the purpose, requirements, and functionalities of the system. 



    2. 
**Document Conventions**
N/A



    3. 
**Intended Audience and Reading Suggestions**
This document is written for software developers, programmers and testers, in order to help them in developing and troubleshooting the system.



    4. 
**Product Scope**
This application provides an environment for administrators and managers to manage volunteers and requests. It provides the following benefits:



* It has scheduler for volunteers per week
* It has a forecast feature for next week’s projection of volunteers and requests.
* It reports the health agencies about health issues of the senior people.
* It tracks volunteer’s performance.
* It creates/edits senior and volunteer profiles. 



    5. 
**References**
_N/A_

_	_



2. 
**Overall Description**
The intended features upon release of the first iteration include, a dispatching system for volunteers, a care request system for those that need aid and a tracking system for both other systems to provide details and analytics for each system.  This will benefit the city that is using the system as well as all the overworked care aids and the population of those that need car aids.  Dispatching the volunteers to requests will alleviate stress and unnecessary work for care aids, provide aid to those in need and overall create a happier state of living for all those involved.



    6. 
**Product Functions**
Three major functions are:



* Creating new volunteer profile
* Assigning new volunteers
* Generating Daily Report



    7. 
**User Classes and Characteristic**s

<table>
  <tr>
   <td><strong>User Class Name</strong>
   </td>
   <td><strong>User Type</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>Volunteers
   </td>
   <td>Direct
   </td>
   <td>Directly interacts with the person that requires aid/care.  Provides reminders and updates to senior people for appointments.  Provides updates to the SPCC if there are any rising health issues.  Define their own volunteer activities and personal details.  
   </td>
  </tr>
  <tr>
   <td>SPCC
   </td>
   <td>Direct
   </td>
   <td>Receive calls from senior people that need assistance and input their details to the system.  Able to change data if it needs to be updated later.  
   </td>
  </tr>
  <tr>
   <td>System Administrators
   </td>
   <td>Direct
   </td>
   <td>Manage all volunteers.  Report issues with any volunteers to them, also is reported to by volunteers.  Submit new volunteer profiles to do a background check and verify educational certificates after they have completed the initial screening. Approve or deny new volunteers.  Reassigns volunteers based on severity.  
   </td>
  </tr>
  <tr>
   <td>School Administrators
   </td>
   <td>Direct
   </td>
   <td>Request volunteer aid with teaching.  Does not provide any details on students, simply requests the aid and pair volunteers with students
   </td>
  </tr>
  <tr>
   <td>Senior People
   </td>
   <td>Indirect
   </td>
   <td>Call and provide data to SPCC as well as provide them data.  Receive updates on important information such as appointments.
   </td>
  </tr>
  <tr>
   <td>Health and Safety Agencies
   </td>
   <td>Indirect
   </td>
   <td>Contacted by the SPCC when a senior person is having major health issues that do not require a hospital.  
   </td>
  </tr>
  <tr>
   <td>False Volunteers
   </td>
   <td>Dis-favoured
   </td>
   <td>We need qualified and valuable volunteers, anyone providing false information or invalid information will be rejected by system administrators.  
   </td>
  </tr>
  <tr>
   <td>Children/Students
   </td>
   <td>Dis-favoured
   </td>
   <td>Parents do not want their children interacting with the system.  Receive help from the volunteers.
   </td>
  </tr>
</table>




    8. 
**Operating Environment**
The system will be used remotely while being highly secure and reliable as the targeted audiences are not experienced in the use of the network. Therefore, simplicity is a major role. It will be a free website and app for everyone no matter their income to access it. The users are located close together as it will be only for the city so a small server can be used that requires only one time zone. The System can be accessed through the web and phone application, the city center will also facilitate the program for people without digital devices.

All data will be stored on a server in the city center which will be a combination of all data collected by the system. The accessing time will depend on how busy the system is but an average of 3 seconds as a response time. Users would be able to tolerate service interruptions but an emergency line is always online to provide the necessary aid. Security controls are needed such as passwords and 2FAs are required to set up an account.



    9. 
**Design and Implementation Constraints**
LI-1: As the system is mainly intended for volunteer opportunities, a job search feature is a feature that could be considered that we do not plan on adding.

LI-2: A lack of messaging feature on the app/website. Some people may not want direct communication with the volunteer or client, so all communication will be done at the user’s discretion, except for the first communication as this will be done by the system by giving both parties a time and place for the requested care.



    10. 
**User Documentation**
N/A



    11. 
**Assumptions and Dependencies**
AS-1: Potential volunteers will have their police certificate checked through a background check system. 

AS-2: Potential volunteers have minimum educational skills. 

DE-1: Shortage of daily care workers who support the senior people

DE-2: Due to background checks, the process of assigning volunteers can take a long time.

DE-3: Incentives that can motivate more people to work voluntarily.



3. 
**External Interface Requirements**


    12. 
**User Interfaces**


<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.jpg). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](![image](https://user-images.githubusercontent.com/103209983/204953539-b652dcc1-6a1e-43a0-b6fe-c24d6ec4d5aa.png))




    13. 
**Hardware Interfaces**
The communication protocol used between the system and the remote database shall be

an ODBC connection secured using level 4 encryption standard.



    14. 
**Software Interfaces**


<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image2.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](![image](![image](https://user-images.githubusercontent.com/103209983/204953507-ac26012e-ef05-4f5c-8110-d9e606600dfa.png))


- The system shall retrieve information about the senior from the SPCC database. It also confirmed validated volunteers from Background Check Systems.



<p id="gdcalert3" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image3.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert4">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](![image](https://user-images.githubusercontent.com/103209983/204953566-1d43a33e-1191-4536-8b1b-e58c94d25ca2.png))




    15. 
**Communications Interfaces**
_N/A_



4. 
**System Features**


    16. 
Create New Volunteers

    4.1.1	Description and Priority


        _	_In this system, one of the major features is to create new volunteers. In order for the whole process to start, a requirement is to create a profile for the new volunteer, making this feature a high priority. 


    4.1.2	Stimulus/Response Sequences


        _	_A stimulus that can happen while creating new volunteer profiles is when nothing happens in the creation process; a blank screen after registering or when it skips information inputs.


    4.1.3	Functional Requirements


                REQ-1:	Functional requirements of the “Create New Volunteers” use case


<table>
  <tr>
   <td><strong>volunteer.Create</strong>
   </td>
   <td><strong>Creating a new volunteer</strong>
   </td>
  </tr>
  <tr>
   <td><strong>.Register</strong>
   </td>
   <td>Volunteers shall provide details and information to create an account.
   </td>
  </tr>
  <tr>
   <td><strong>.Check</strong>
   </td>
   <td>If the volunteer is not already registered and their information is sent to the security check
   </td>
  </tr>
  <tr>
   <td><strong>.Senior</strong>
   </td>
   <td>The system provides the volunteer with available and related volunteer opportunities. From the database of opportunities provided by places that need volunteers.
   </td>
  </tr>
  <tr>
   <td><strong>.Return</strong>
   </td>
   <td>If there are no available options, the systems offer additional suggestions for opportunities or give them an option for notification of related works.
   </td>
  </tr>
</table>




    17. 
Assign Volunteers


        1. 
Description and Priority

        	After creating a new volunteer profile, newly registered volunteers are wanting to be assigned to volunteer jobs that are available. Admins and managers assign jobs that will match the volunteer’s profile. This is also a high priority feature.



        2. 
Stimulus/Response Sequences

        	An issue that can occur on assigning a volunteer is when the volunteer did not pass the initial screening, making the newly created profile invalid. Another issue is when the volunteer changes their mind on applying to do volunteer work.



        3. 
Functional Requirements

                REQ-2:	Functional requirements of the “Assigning a volunteer” use case


<table>
  <tr>
   <td><strong>volunteer.Assign</strong>
   </td>
   <td><strong>Assigning a volunteer</strong>
   </td>
  </tr>
  <tr>
   <td><strong>.Approve</strong>
   </td>
   <td>After the initial screening and interview, if the person applying for the volunteer role meets all requirements, the person is approved and selected to be a volunteer.
   </td>
  </tr>
  <tr>
   <td><strong>.Request</strong>
   </td>
   <td>Senior people go through the SPCC on requesting aid from volunteers.
   </td>
  </tr>
  <tr>
   <td><strong>.Search</strong>
   </td>
   <td>SPCC searches for volunteers through the VMS and input specific needs to filter out volunteers and make it easier to receive aid.
   </td>
  </tr>
  <tr>
   <td><strong>.Notify</strong>
   </td>
   <td>The VMS notifies users managing the volunteers that there are urgent volunteer jobs available. 
   </td>
  </tr>
  <tr>
   <td><strong>.Allocate</strong>
   </td>
   <td>Once notified by VMS, managers allocate volunteer jobs to volunteers with specific needs.
   </td>
  </tr>
</table>




    18. 
**Generate Daily Report**


        4. 
Description and Priorities

        At the end of each day, the system provides the admins and manager an overview of the daily performance of the system. This is a medium priority feature.



        5. 
Stimulus/Response Sequences

        Issues that can occur in this feature are:



* Senior person was not available for their daily call
* Approval from police was help up, so background checks were paused
* Missing required information for the daily report.



        6. 
Functional Requirements

                REQ-3: Functional requirements of the “Generate Daily Report” use case


<table>
  <tr>
   <td><strong>generate.Report</strong>
   </td>
   <td><strong>Generating a daily report</strong>
   </td>
  </tr>
  <tr>
   <td><strong>.Collect</strong>
   </td>
   <td>The system gets the numbers of request made by the Senior through the SPCC
   </td>
  </tr>
  <tr>
   <td><strong>.Location&Date</strong>
   </td>
   <td>If a request is approved, the senior shall provide a valid location and date for the care.
   </td>
  </tr>
  <tr>
   <td><strong>.Available</strong>
   </td>
   <td>After assigning volunteers the number of available volunteers is then collected. 
   </td>
  </tr>
  <tr>
   <td><strong>.Forecast</strong>
   </td>
   <td>The VMS shall then generate a forecast using the number of requests and available volunteers.
   </td>
  </tr>
  <tr>
   <td><strong>.Send</strong>
   </td>
   <td>The VMS shall notify the Mayor office and the database administration with the generated report each day.
   </td>
  </tr>
</table>




5. 
**Other Nonfunctional Requirements**


    19. 
**Performance Requirements**


* The website homepage will load within 1.5 second.
* The website will have a capacity of 3,000 active user at a time.
* The website will have a 90% uptime annual.



    20. 
**Safety Requirements**
_N/A_



    21. 
**Security Requirements**


* The stored senior data will be encrypted to level 4 standard.
* The website will be updated every year.
* The website will be compatible with IOS 16 and Android 12.



    22. 
**Software Quality Attributes**


* **Very fast:**Efficiency, the system shall submit requests (ie. changes pages, logging in, applying for volunteer, etc.) in less than 10 seconds.
* **Easy to learn:**Usability/Learnability, the system shall have a detailed walkthrough when you launch it for the first time
* **Easy to use:**Usability, the system shall have a simple GUI with small amount of options and screens
* **No data exposure:**Functionality/Usability, the system shall maintain data within the database



    23. 
**Business Rules**
_N/A_



6. 
**Other Requirements**
**Appendix A: Glossary**

_N/A_

**Appendix B: Analysis Models**

_N/A_

**Appendix C: To Be Determined List**

_N/A_
