AntiChatSystem Documentation
Version: 2.1
Developer: Harked
Last Updated: 2024/09/29

Table of Contents



            Overview
The AntiChatSystem monitors all in-game chat in real time, detecting inappropriate language, issuing warnings, and applying temporary or permanent bans. Fully customizable and scalable, the system ensures a cleaner chat experience for your game while also sending logs to a Discord webhook for admins to review.


            Features

Real-time Chat Monitoring
Warning and Ban System
Custom Warning/Ban Messages
Word and Phrase Detection
Automated Temporary and Permanent Bans
Dynamic Warning and Ban Durations
Customizable Violation Thresholds
Warning Reset System
Advanced User Whitelisting/Blacklisting
Logging and Notifications
User Interface (UI) Integration
Detailed Logs via Webhooks
Multi-language Support
Rate Limiting to Prevent Spam
Admin Bypass for Testing
High Scalability for Large Servers


          System Setup
Download Script: Download and insert the AntiChatSystem script into ServerScriptService.
Connect Chat Service: Use game:GetService("Chat") to ensure all messages are monitored.
Webhook Setup: Create a Discord webhook, copy the URL, and paste it into the script.
Configure Word Filter: Edit the word filter in the script to add/remove banned words.
Whitelist Admins: Add trusted UserIDs to the whitelist section in the script.
Test: Use an alt account to test, ensuring warnings/bans are issued properly and logs appear in Discord.



          Configuration

Customizing Word Filters: Edit the bannedWords array in the script to add or remove inappropriate words.
Example: local bannedWords = {"badword1", "badword2"}
Setting Warning/Ban Durations: Edit the variables for warning reset (default 48 hours) and ban length (default 1 hour).
Modifying Ban Messages: Edit the banMessage variable in the script.
Example: local banMessage = "🚫Banned by Fatality🚫 You have been banned for 1 hour for chat rule violations."
Logging: Paste your Discord webhook URL into the script to enable logging.


            FAQs
Q: Can I change the ban duration?
A: Yes, adjust the duration in the configuration section.
Q: How do I customize the word filter?
A: Add/remove words in the bannedWords array.
Q: Can I receive real-time notifications of bans?
A: Yes, set up a Discord webhook for instant logging.




      Future Improvements

7. Future Improvements
Machine Learning Detection: Adding ML algorithms to detect more advanced chat violations.
Role-Based Bans: Allowing different ban types (e.g., mute vs. kick).
Appeal System: Let players appeal bans automatically via a form.
