Gowtham_Test
============

Test File

2.2Publisher_UC02 –  RFP Response by Publisher
User Story Number	Use Case Version	Wireframe(Yes/No)	Status
102	1.0	Yes	Approved
Description:	The use case begins when the publisher wants to enter the details for the RFP.
The use case ends when the user has successfully saved or submitted the response to RFP.
Actors:	Publisher
Triggering Event	The user want to enter the response to RFP
Pre-Conditions	1. The user is logged in
2.  The user has received a notification email stating that RFP has been submitted by SSCG.
Post-Conditions	1. RFP response is saved into the system
2. Email notification is sent to the admin users
Requirements and Business Rules	1. User should be presented with the Submitted/Saved RFP field that would allow them to choose the RFP that they want to view/edit. 
All the fields selected for a RFP are Mandatory Fields except description, rationale and Engagement defined.
2. User should be able to attach 3 files along with the response.
File types  [pdf, image files, office suite files like ppt, xls, doc]
Max file size [15 MB]
3. The following Alert Messages that should appear if user has not entered value in the necessary fields.
“Please fill in following fields” and list out the fields that have not been filled in.
4. The RFP’s that  have been received and not edited even once should be shown as new
5. RFP response should not be able to be deleted or edited once, it is submitted, unless it is sent back to them from   SSCG. 
6.  Each publisher can submit multiple response rows but only one set of answers for the questionnaire.
Basic Path:	1)User chooses RFP option
2)All the RFP Proposal submitted by SSCG is displayed
3)User selects a proposal  to enter the rate card details
4)User enters details.
5)To add another row in the same proposal. User choses 
and “New Response Item” option and perform the same step4.  AS 2 User chooses clone  option
6)User attaches files if any. 
7)User publishes the proposal   AS1. Actor click on the save button 
8)Use Case Ends
Alternate Path	AS1:  Actor chooses save option 
1. The RFP response is saved for further editing.

AS 2: User chooses clone option
A new response item is created with same details as the current response item and current response item is saved.

AS3:  User chooses the reset option
The details in the current response items get cleared out

AS4:  User chooses the delete response item
The response item is deleted

Remarks	None

2.3Digital_UC03 – View RFP Responses
User Story Number	Use Case Version	Wireframe(Yes/No)	Status
103	1.0	Yes	Approved
Description:	The use case begins when the user wants to view RFP responses.
The use case ends when the user has view the RFP responses
Actors:	Media Planner, Admin Planner, Super Admin
Triggering Event	The user chooses the view RFP responses
Pre-Conditions	1. The user is logged in
2. At least one publisher has sent their response(s). 
Post-Conditions	User is able to view the RFP responses
Requirements and Business Rules	1.The screen should have the following fields as a Filter Criteria
a.Target Specialty (Very Important Filter Criteria)
b.Publisher
c.Placement Types
d.Section Names
e.Site
f.CPM 
g.CPC
h.Brand
2.All the records will get displayed by default
3.The screen should display the values of the following fields in a row wise manner
a.Brand
b.Publisher
c.Site
d.Placement Type
e.Section Names
f.Target Speciality 
g.CPC –Cost per click 
h.CPM –cost per thousand
i.Previous year CPM/CPC
j.% Change 

4.CPM and CPC should also be filters so that both or each one individually may be shown. If both are shown in the same column then there should be a symbol/colour code to distinguish them.
5.% change is the  difference between CPM for the client between this year and the previous year in %  .
6. RFP response should have a scorecard compiled from the answers to the questionnaire from different publishers.
Basic Path:	1. User chooses the View RFP Responses option
2. User sees the RFP responses submitted by the publishers.
3. User can filter the responses as per his/her choice.
4. Use case ends.
Alternate Path	None
Remarks	None

2.4Digital_UC04 – Edit RFP Responses
User Story Number	Use Case Version	Wireframe(Yes/No)	Status
104	1.0	Yes	Approved
Description:	The use case begins when the user wants to edit RFP response.
The use case ends when the user has successfully edited RFP response 
Actors:	Admin Planner and Super Admin
Triggering Event	The user chooses the edit RFP responses  from the Response Details screen
Pre-Conditions	1. The user is logged in
2. At least one publisher has submitted response to the RFP.
3. User is in the currently viewing the screen that displays the lresponses submitted by the publishers.
Post-Conditions	1. RFP response is edited by the user successfully 
Requirements and Business Rules	1. All the fields except publisher field should be editable
2. No notifications will be sent to the Publisher
Basic Path:	1. User chooses the RFP responses option
2. User edits the fields in the RFP responses.
3. The edited data is saved.
4. Use Case ends
Alternate Path	None
Remarks	None
	
2.5Digital_UC18 –  Send RFP Response back to the Publisher(Digital) [Change Request]
User Story Number	Use Case Version	Wireframe(Yes/No)	Status
	1.0	Yes	Under Review
Description:	The use case begins when the SSCG media user wants to send the RFP Response back to the publisher
The use case ends when SSCG Media user has successfully send a  RFP Response back to the publisher
Actors:	Admin Planner and Super Admin
Triggering Event	When the actor clicks on the change request button 
Pre-Conditions	The user has logged in and has selected a RFP response 
Post-Conditions	The user will be viewing the View RFP Response screen
Requirements and Business Rules	1.User should be able to send change request to a RFP Response back to publisher.
2.Once a change request has been sent for a response, the user should not be able to use it in a schedule or edit it till a revised response is received for it.
3.Publisher receives the email notification that change request has been issued.
Basic Path:	User is viewing the response details
User clicks on “Change Request” button
User enter the comments on the textbox and clicks on the send button
The comments will be saved for the response
Alternate Path	None
Remarks	None

