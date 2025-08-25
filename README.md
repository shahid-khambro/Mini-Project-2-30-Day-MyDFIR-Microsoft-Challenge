# Mini-Project-2-30-Day-MyDFIR-Microsoft-Challenge

# Objective: Simulate a suspicious email, then walk through how a SOC analyst would investigate and respond.

# outline 

Simulate a suspicious email

Tools Used 

Explorer 

Quarantine

Email headers

walk through how a SOC analyst would investigate and respond




# Simulate a suspicous Email 

# How to Launch a Phishing Simulation

To create and deploy a simulated phishing email, please follow these steps:
1.	Navigate to the Microsoft 365 Defender portal at https://security.microsoft.com 
2.	In the left-hand navigation menu, select Attack simulation training.
3.	Click on the Simulations tab.
4.	Click the + Launch a simulation button to begin the creation and deployment process.

   <img width="901" height="275" alt="creating simulation" src="https://github.com/user-attachments/assets/05241c65-33fc-4ce7-8c5c-6e7dbade7903" />

complete the ckecklist step by step and finish the simulation setting 
**Reviw the Simulation **

<img width="852" height="331" alt="review simulation" src="https://github.com/user-attachments/assets/b106883e-2f44-4713-a964-c8bacbb60536" />

**simulation launched**

<img width="827" height="278" alt="launched simulation (mini project 2)" src="https://github.com/user-attachments/assets/7a6c0c4f-6069-4ba5-9587-fdcc8afd91a3" />


**When a user click on the email and login into the phishing email **
<img width="809" height="296" alt="phishing landing page (mini project 2)" src="https://github.com/user-attachments/assets/099e56cd-4931-4af1-a622-a308367be022" />

<img width="470" height="404" alt="phishing landing page 2 (mini project 2)" src="https://github.com/user-attachments/assets/75d8e7e2-afd0-465c-9ccc-0d124c778991" />

# walk through how a SOC analyst would investigate and respond.

#How to Review User Clicks on Phishing Simulations
1.	Navigate to the Microsoft 365 Defender portal at https://security.microsoft.com.
2.	In the left-hand navigation menu, select Explorer (also known as Threat Explorer).
3.	Apply the necessary filters to find your simulation campaign. For the most precise results, use the View menu and select Phish delivery and user clicks
<img width="834" height="259" alt="user click" src="https://github.com/user-attachments/assets/e926b2d1-0624-4b15-b755-bd2aaa656145" />

<img width="943" height="182" alt="phishing landing page 4 (mini project 2)" src="https://github.com/user-attachments/assets/80c5dfca-7939-4c21-87ed-b851eadd36b2" />


**Are suspicious emails being held in quarantine before they can reach users?**

**How to check quarintine email **

To review emails that have been blocked and isolated by Microsoft 365's protection systems, follow these steps:
1.	  Navigate to the Security Portal:
      Go to https://security.microsoft.com and sign in with your administrator credentials.
2.	Access the Quarantine Section:
      In the left-hand navigation menu, expand Email & collaboration.
      Click on Review > Quarantine.
3.	Review and Filter the Quarantine List:
    You will now see a list of all quarantined messages.
    Use the filters at the top to find specific messages. You can filter by:
      o	Received time: Set a date range.
      o	Subject: Search for words in the email subject line.
      o	Sender address: Find emails from a specific sender.
      o	Recipient address: Find emails sent to a specific user.
      o	Quarantine reason: (e.g., Bulk, Phish, Malware, Spam)
4.	Take Action on Messages:
    Select one or more messages from the list.
    Click on the Take action button to:
      o	View message: See the email headers and content.
      o	Release email: Deliver it to the intended recipient's inbox (you can optionally add a trust policy for the sender).
      o	Download email: Save the email as an .eml file for analysis.
      o	Delete email: Permanently remove it from quarantine.

<img width="778" height="283" alt="quaratine email project 2 " src="https://github.com/user-attachments/assets/3b758302-7a22-4b57-b5e7-3aa18da68050" />



**now also check how many user are compromised on clicking the malicious phishing email **
<img width="946" height="359" alt="phishing landing page 3 (mini project 2)" src="https://github.com/user-attachments/assets/815f2d79-2d4b-4172-953f-b85fda94fcc5" />


**Now furhter checkout the How many links are in the database and in which how many are found **
<img width="567" height="237" alt="phishing landing page  5 (mini project 2)" src="https://github.com/user-attachments/assets/0f0e0a58-b4cb-44e1-b407-acdef4051481" />

<img width="439" height="184" alt="phishing landing page 6  (mini project 2)" src="https://github.com/user-attachments/assets/a96c4ba1-c776-4cf3-9511-01879affcc92" />

**Check out the Top Url in the phishing email **
<img width="750" height="266" alt="top url" src="https://github.com/user-attachments/assets/e6e3f756-074b-4c30-84f1-402d18b8efe5" />

# Review the Header files and create a final Report 

Incident Report: Phishing Simulation Email Delivery
Report Date: August 25, 2025
Incident ID: SIM-20250825-001
Analyst: Shahid Ali

Findings \
**Recipient:** khambro@khambro.onmicrosoft.com \
**Sender display name**: Security and Compliance Team \
**Sender address:** notification@attacksimulationtraining.com \
**Sender mail from address:** notification@attacksimulationtraining.com \
**Return path:** notification@attacksimulationtraining.com \
**Time received (UTC +05:00):** Aug 25, 2025 1:40 AM /

1. Findings
   
 A message identified as a phishing simulation was successfully delivered to a user's Microsoft 365 inbox. The email, purporting to be from a "Security and Compliance Team," contained a training reminder with embedded links to the security.microsoft.com domain and an ICS calendar attachment. The email was flagged by Microsoft's internal systems as an AttackSimMessage but was deliberately allowed to deliver with a Spam Confidence Level (SCL) of 1, indicating high confidence it was a safe, internal simulation.

3. Investigation Summary
   
      An automated phishing simulation email was sent from the Microsoft Attack Simulation Training platform to an internal user. The email was processed through Microsoft's internal Exchange Online servers and successfully delivered to the user's inbox. No malicious activity was detected because this was a authorized security awareness training exercise. All technical indicators (headers, authentication, X-headers) confirm its legitimate origin from a controlled Microsoft service.

3. Who, What, When, Where, Why, How 
   
•	**Who:** 
    o	Source: The Microsoft 365 Attack Simulation Training platform (notification@attacksimulationtraining.com).
    o	Target Recipient: khambro@khambro.onmicrosoft.com (Internal user).
    o	Involved Systems: Microsoft Exchange Online servers (DB8P195MB0614.EURP195.PROD.OUTLOOK.COM, PAVP195MB2232.EURP195.PROD.OUTLOOK.COM).
    
•	**What:**
    o	A planned phishing simulation email was created and delivered to a user to test security awareness and provide training. The email contained a training assignment notification with links to a Microsoft Security portal and a calendar invitation attachment.
    
•	**When:** 
      o	Time Sent (UTC): August 24, 2025, at 20:40:41.
      o	Time Received (UTC): August 24, 2025, at 20:40:43.
      o	Current Status: This was a single, scheduled event that has concluded. It is not an ongoing attack.
      
•	**Where:** 

      o	The event occurred entirely within the Microsoft 365 cloud environment.
      o	The message traversed internal Microsoft Exchange Online servers and was delivered to the user's mailbox (Inbox/folder).
      
•Why:

This happened as part of a proactive security measure. Organizations use these simulated phishing campaigns to educate employees on identifying phishing attempts, reinforce training, and measure the overall susceptibility of the workforce to social engineering attacks.
        
•  How 

  The simulation was launched by an administrator from the Microsoft 365 Defender portal (likely the Attack simulation training module).
  The Microsoft backend service (substrate.office.com) generated and sent the email, spoofing a legitimate-looking sender to make the simulation realistic.

5. **Recommendations** 
   
    Since this was an authorized simulation, no remediation is required. However, the following steps are recommended to maximize the benefit of the exercise and ensure future simulations run smoothly:
      1.	Review User Response: The security team should review whether the target user opened the email, clicked the links, or opened the attachment. This data is available in the Attack simulation report in the Microsoft 365 Defender portal.
      2.	Provide Targeted Training: If the user interacted with the simulation email, ensure they are assigned the requisite security training to improve their awareness.
      3.	Communicate with the User: If the user reports this email as suspicious, praise them for their vigilance and explain it was a test. If they did not report it, this can be a coaching opportunity.
      4.	Maintain Simulation Schedule: Continue to run these simulations periodically with varying levels of complexity to maintain a high level of security awareness across the organization.
      5.	Verify Reporting Process: Ensure all users know how to report suspicious emails using the built-in reporting tools (e.g., "Report Message" add-in).

**Conclusion**: 

 This incident is a false positive from a security monitoring perspective and represents a legitimate security training activity. No action is needed to mitigate a threat, but follow-up actions should be taken to leverage the simulation for educational purposes.
