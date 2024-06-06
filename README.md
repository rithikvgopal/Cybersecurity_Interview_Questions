# Cybersecurity_Interview_Questions

These are few question I am preparing for my upcoming Cybersecurity Analyst interview. 
Sharing this with you as you guys can prepare and excel the interview. 
All the best to everyone!!!

### [1. How do you configure rules within a SIEM to identify potential security incidents? Please provide an example.](#Answer_1)
### [2. Describe a situation where you had to fine-tune an alert to reduce false positives. What steps did you take?](#Answer_2)
### [3. Walk me through the incident response process you followed for a specific security incident at a previous job. What tools did you use?](#Answer_3)


### Answer_1

Situation - In my previous role as a cyber security analyst at the XYZ company, we observed an increase in the number of security incidents caused by sophisticated phishing attacks.
These attacks were able to bypass the initial defense in place.

Task - My task was to create SIEM rules that would detect these sophisticated attacks at an early stage and provide data to the incident response team to act swiftly. 

Action - So the first thing I did was to analyze the previous phishing events and identify key indicators - pattern or signature among them, like multiple failed logins, Login from IP not registered under the user, or change in IP location, etc. 
Once I had enough data, I created rules such as triggering an alert when there are 5 login attempts within a 10-minute window with the same IP address and another one when the IP location of the user is not the same as that of previous login events or if the login attempts happened at unusal timings. 
Once these rules were created, I performed tests to ensure the effectiveness of the rules. I finetund it based on the results received as well as the feedback from the incident response team. 

Result - In the initial month, the initial response team was able to identify 3 phishing attacks swiftly change the credentials for the compromised account and provide education to the affected users.

### Answer_2

Situation - In my previous role, I was responsible for managing the SIEM and monitoring the firewall logs to safeguard from potential security threats. There were many false positives, especially due to the legitimate port scanning activities. This flood led to many false positive security alerts overwhelming the incident response team and  creating alert fatigue. 

Task - My task was to fine-tune the existing SIEM rules to reduce the false positives, without compromising in detecting the legitimate security threats. There was a need to increase the effectiveness of the rules.

Action - The first thing I did was conducted a thorough analysis of the false positive alerts to understand their common characteristics. I reviewed several weeks' worth of logs to identify patterns and determine why legitimate activities were being flagged. I Collaborated with the network team to understand normal network traffic patterns, including legitimate scanning activities related to network monitoring tools and routine maintenance tasks. Once I had the required data i moved on the modify the SIEM rules to include additional context and exceptions. For instance, I adjusted the threshold for triggering an alert based on the number of ports scanned within a specific timeframe and excluded known safe IP addresses associated with our internal network monitoring tools.
Implemented the changes in a test environment to monitor the effectiveness of the new rules. This involved simulating both legitimate and malicious scanning activities to ensure the rules were accurately differentiating between the two. After deploying the refined rules to the production environment, I continued to monitor the alerts closely. I held regular meetings with the incident response team to gather feedback and made further adjustments as necessary.

Result - I monitored the alert for two weeks and conducted regular meeting with the incident response team to understand the effectiveness of the fine-tuned alert. The finetuning of the rule led to a decrease of 70% in the number of false positives. This allowed the incident response team to focus on genuine threats and respond more effectively. Additionally, the improved accuracy of our alerts helped enhance our overall security posture and increased the team's confidence in the SIEM system.


### Answer_3

Situation - In my previous role as a cybersecurity analyst, we came across a situation where one user reported suspicious activities in their account, which led us to discover malware infection in a few of the endpoints. The malware appears to be designed to perform data exfiltration. 

Task - My task was to support the incident response team in analyzing the malware and performing the mitigation steps to prevent the spread of the malware. 

Action - We followed the NIST incident response framework, which has steps: Preparation, Identification, containment, eradication, recovery, and lessons learned. 

  Preparation 
  - It was ensured the incident response team had up-to-date contact information and clearly defined roles.
  - Verified the required resources were available and working properly for use.
 Identification
  - Using the SIEM(Splunk) to analyze the logs to correlate the events with the reported suspicious activities.
  - Employing the EDR(crowdstrike) to scan the endpoints to identify the presence of malware in them.
  - Verifying the indicators of compromise(IOCs) such as unusual network traffic, unauthorized access, etc.
 Containment
  - Isolating the affected devices from the network to avoid the spreading of malware.
  - Creating network segmentations to avoid the spread of malware.
  - Blocking malicious IP addresses and domains at the firewall and proxy levels.
 Eradication
  - Performing a forensic analysis using tools such as Encase to understand the scope of the infection and the affected files from the malware.
  - Removing the malware with the help of anti-virus and anti-malware tools such as Malwarebytes. 
  - Updating the system and performing patches to secure if the malware had exploited vulnerabilities.
 Recovery
  - Recovering the system from clean backups to ensure there is no malware residue.
  - Closely monitoring the system to check if there are any signs of re-infection.
  - Communicate with the users to reset their credentials and improve their security awareness.
 Lessons learned
  - Conducted a post-review of the incident to discuss what went well and what should be improved.
  - Documented the incident and the response actions taken to update the response plan.
  - Providing additional training to associates to identify phishing attacks etc in the first place.

Results - The security incident was swiftly tackled by the incident response team and the other teams associated such as SOC, email gateway, network, etc. The malware was contained and eradicated, and no data was exfiltrated. The affected devices were restored with minimal downtime and the lessons learned were used to enhance the incident response plan and the security posture.  
 
### Answer_4
### Answer_5
