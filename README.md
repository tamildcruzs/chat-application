  
SOFTWARE
REQUIREMENT SPECIFICATION
FOR CHAT      APPLICATION   AND WEBSITE




 

 
1.	Introduction 
2.	
2.1	Purpose :

This document describes the software requirements of WhatsApp, an online instant mobile messaging app that allows you to exchange messages through the same internet data plan that you use for email and web browsing. It can be used on any kind of device, such as iPhone, Blackberry, Android, Windows Phone and Nokia. 


2.2	Document Conventions: font: 

2.3	Intended Audience and Reading Suggestions 


The document is intended for all the stakeholder customer and the developer (designers, testers, maintainers). The reader is assumed to have basic knowledge of Mobile operating systems, database and user account. Knowledge and understanding of UML diagrams is also required. 







2.4	Definitions 

• User Account 
An account is used to store the information about the users such as phone number and username on a network server. It allows the user to change their status, exchanging the photos and videos over the network using their mobile data and operating system. 
• Mobile Operating System 
A mobile operating system, also known as a mobile OS, is an operating system that is specifically designed to run on mobile devices such as smartphones, PDAs, tablets and other handheld devices.  
• Database 
A database is a collection of information that is organized so that it can easily be updated by the new details of the users. 
   
2.5	Project Scope 

WhatsApp is an online instant messaging application that integrates user’s contacts from their phonebook with the application and enables exchange of messages and documents free of cost over the internet. It also allows the user to do voice/video call at the normal internet speed rate and let the user to change his/her status whenever he/she wants to.

 
2.6	References
  
i https://web.whatsapp.com/%F0%9F%8C%90/en  
ii http://www.uianduxdesign.com/ux-designs/whatsapp-user-interface-and-user-experiencedesign.html   
iii https://www.whatsapp.com/   


3.	Overall Description 

3.1	Product Perspective 

Whatsapp does not work independently. It works together with the web server, internet connection, the mobile OS and the smartphones. 
Communication interface: Whatsapp communicate with the internal memory of devices via a communication network. 
Software interface: The messages sent via the communication network are specific to the target application user on the receiving side. 
Hardware interface: The software will run on the smart devices with the installation of the application and proper verification of user. 
User interfaces 
User: Once the application is installed in the device, it goes through the user’s contact list, and list up the contacts which are using the same application and show to send a push invitation for the 
   
unregistered users to connect and chat on WhatsApp. A user enters his or her phone number, and can then change the phone number and verify the same. 
Security Manager:  The security manager takes the responsibility of the security of the authentication of the user and to encrypt/decrypt its messages using suitable algorithms in the network channel. 
Maintainer: The maintainer is responsible for adding new features to the application and launch the latest updates in the world in order to make the application efficient.  


3.2	Product Features 

The WhatsApp application should work 24 hours. The application identifies a customer by his/her phone number. It collects information about the contacts of the user, communicates between the different people, allow the user to reform their status and profile photos, sends instant messages and data to the other users of WhatsApp (e.g., pictures, messages, videos, documents, audio messages) , user can communicate to the other user of the same application by (voice/video) calling them from WhatsApp, can see their last seen detail, user can create groups and can broadcast message in group to the other users of group, users can hide their details from other users like their profile picture , status, last seen, users can block users and also can spam other users, users can save their chat, and they can also star the important messages. The app provide its own software on various app stores.

  
3.3	User Classes and Characteristics 

Characteristics: There are several users of WhatsApp: 
Users are simply the members of the general public with having their details on the application and using it with no special training. 
Security Manager need to have specialized education or experience regarding the same. 
Maintainers must be experienced network administrators, to be able to connect new ATMs to the network.  


3.4	Operating Environment 

The hardware, software and technology used should have following specifications:  
• Ability to connect to the Wi-Fi or mobile network.    
   
• Ability to exchange data over the network  
• Processor with minimum speed of 500 MHz  
• Ability to use camera, gallery, microphone and other services of mobile. 
• Ability to take input from user  
• Device must have 512MB RAM or above   



3.5	Design and Implementation Constraints
 
• Installment of application 
Validate Phone Number:  • Validate for phone number authentication  
• Validate that the number belongs to the same person or not.  
• If number is correct, send message code to the number for verification.   
Validate for Change Phone Number:  • Validate that the new number is of the same user or not.  
• If number is correct, send message code to the number for verification.

   
2.6Assumptions and Dependencies 

• Hardware never fails.  
• Phone memory never be out of space.  
• Proper connectivity of network.   
  
   
3.Specific Requirements 

3.1 Functional Requirements 

The functional requirements of WhatsApp are listed below:-
  
FUNCTIONAL REQUIREMENT 1: 
User Registration • Description: After installing the application, the person must be prompted to register their valid phone number. If user skips this step, application should be closed. The user’s phone number will be the unique identifier of his/her account on WhatsApp and will be verified by a text message or by a call. 
• Input: Valid phone number and username. 
• Processing: Storing the data of user. 
• Output: Account created. 
• Authorization: The authorization starts after a user has entered his/her phone number in the application.  
FUNCTIONAL REQUIREMENT 2: 
Adding New Contacts  • Description: The application should auto-detect all contacts from the user’s phone book who are using the same application or not. If any of the contacts have user accounts with WhatsApp, those contacts must automatically be added to the user’s contact list on WhatsApp and the remaining users should be shown as invite option that sends a regular text message to those contacts asking them to join WhatsApp along with a link to the WhatsApp application on any app-store.    

FUNCTIONAL REQUIREMENT 3: 
Convey a Message  • Description: The registered person should be able to send and receive instant message to/from any contact on his/her WhatsApp contact list. The person should be notified by a single tick when message is successfully delivered to the recipient and notified by double tick when message is received by recipient and displayed by blue tick when message is seen by the recipient. 
• Input: The message to the user. 
• Processing: Delivery of message. 
• Output: Display the tick after delivering the message and display a blue tick when message is seen by the recipient.  

FUNCTIONAL REQUIREMENT 4: 
• Description: The user will be able to make a voice/video call to another user and talk to each other over the network in few Mb of data.  
FUNCTIONAL REQUIREMENT 5:
 Deliver Attachments  
• Description: The person should be able to send or receive instant photographs or videos, documents, audios, videos, images, contacts and location to another person.  
The formats for Images that the application support: .jpg, .jpeg, .png  
The formats for Videos that the application support: .avi, .mp4, .flv, .gif  
The formats for Audios that the application support: .mp3   
The size limit for attachments per message should not exceed 16MB. 
• Input: Image, video, audio, document, location and contacts 
• Processing: Sending of the data. 
• Output: Display the ticks.  
FUNCTIONAL REQUIREMENT 6: 
Broadcast Message  
• Description: User should be able to create groups of contacts which will not let the group member know that they are in broadcast group. User should be able to broadcast messages to these groups which will be sent individually. 
• Input: Messages, image, video, audio, document, location and contacts 
• Processing: Sending of the data. 
• Output: Display the tick of delivering data with broadcast symbol. 
   
FUNCTIONAL REQUIREMENT 7: 
Group Message 
• Description: It allow the user to create group of peoples to talk together within the group and share the attachments. 
• Input: Messages, image, video, audio, document, location and contacts 
• Processing: Sending of the data. 
• Output: Display the tick of delivering data.  
FUNCTIONAL REQUIREMENT 8: 
Message Status 
• Description: It helps the user in order to know the status of any particular message of a specific chat to check the status that whether the message is delivered, seen or not along with the time of the same.  
 

FUNCTIONAL REQUIREMENT 9: 
Starred Messages 
• Description: The messages which have been marked as star of any chat will help the user to see the starred messages after while in an easy way rather than finding it in whole message history. 
• Output: Message is highlighted with star symbol.   
FUNCTIONAL REQUIREMENT 10: 
Search Message 
• Description: The user will also get the authority to search a snippet of message in anyone’s chat from the whole chat history. 
• Input: Snippet to be searched. 
• Processing: Searching the text from the whole chat of particular person in descending order of date and time. 
• Output: Highlight the matched words in yellow colour.   
   
FUNCTIONAL REQUIREMENT 11: 
Clear Chat
 • Description: It allows the user to clear the whole chat of any particular person in his/her friend list.  



FUNCTIONAL REQUIREMENT 12:
 Email Chat 
• Description: The user can email any specific conversation with any person in order to keep the chat safe.  

FUNCTIONAL REQUIREMENT 13: 
Mute Chat
 • Description: It helps the user to mute any particular chat for a period of time that will not show the notification of that chat’s messages. 

FUNCTIONAL REQUIREMENT 14: 
Media
 • Description: It shows the user that which Medias we have shared with a particular person over the network such as photos, videos, gifs, documents, audios and links.  

FUNCTIONAL REQUIREMENT 15: 
View Contact
 • Description: It helps the user to view the contact of any particular user of his/ her friend list compromising of profile picture, status, mute, custom notification and phone number.  




FUNCTIONAL REQUIREMENT 16:
 Set Wallpaper 
• Description: WhatsApp gives the facility of having a desirable wallpaper behind the chats according to the user’s choice including solid colour, theme and gallery photos.  

FUNCTIONAL REQUIREMENT 17:
 Block User
 • Description: It helps the user in order to block any person whom we don’t know or don’t want to take with a prompt message of confirmation. After blocking a chat, that user will not be able to see our details.  
FUNCTIONAL REQUIREMENT 18: 
Add Shortcut
 • Description: WhatsApp provides it so that we can add the most frequent chat on our home screen rather than opening the WhatsApp all the time and easy to use. 
  
FUNCTIONAL REQUIREMENT 19: 
Status
 • Description: User can be able to change his/her status whenever he/she wants to. It provides the limit of 139 characters including smiley with it. 
 
FUNCTIONAL REQUIREMENT 20:
Profile Picture 
• Description: User can be able to change his/her profile picture whenever he/she wants to. We can use image (.jpg, .png, .jpeg) for the same.  
FUNCTIONAL REQUIREMENT 21: 
WhatsApp Web 
• Description: User can be able to change his/her profile picture whenever he/she wants to. We can use image (.jpg, .png, .jpeg) for the same.  
FUNCTIONAL REQUIREMENT 22: 
Archive Chat 
• Description: It help the user to archive any particular person’s chat into archive list and that chat will not be shown in the user’s chat area and make a tab of archive chats at the last of chat room.   
FUNCTIONAL REQUIREMENT 23: 
Settings
 • Description: It provides the user to customize their settings as per their choice.  
FUNCTIONAL REQUIREMENT 24:
 Accounts Setting
 • Description: It helps the user to set their privacy on last seen, profile photo and status along with the list of blocked contacts and also give the feature of changing the number and delete account.  
      
FUNCTIONAL REQUIREMENT 25: 
Chats Setting
• Description: User can be able to change the application language, font size, wallpaper, chat backup in Google drive over a period of time selected by user, and chat history to email, archive, clear and delete all chats.  
FUNCTIONAL REQUIREMENT 26:
 Notification Setting 
• Description: Users are allowed to customize their notifications by setting conversation tones, notification tone, vibration, popups, light for the single chat and group chat both. It also gives a facility to change the ringtone and vibration for the voice/video call.  

FUNCTIONAL REQUIREMENT 27: 
Data Usage Setting 
• Description: It helps the user to set that which media should be auto-download using mobile data, Wi-Fi and roaming along with the details of sharing of bytes over internet category wise. 

FUNCTIONAL REQUIREMENT 28: 
Contact Setting
 • Description: It provides the user to invite any friend and his/her contact list that whether to show all contacts or the hidden contacts along with it.
  
FUNCTIONAL REQUIREMENT 29:
 About and Help 
• Description: It provides the website URL of FAQ, Contact us, System status, Terms and Privacy Policy, and about the version and licenses of WhatsApp Messenger.   
   
4. External Interface Requirements 
4.1 User Interfaces 
The WhatsApp user interface should be fast and easy to understand, such that most of the new registered users are able to use it without any assistance .
4.2 Hardware Interfaces 
The hardware should have following specifications:  
• Ability to read gallery  
• Ability to exchange data over internet 
• Continuous data connection   
• Ability to take input from user  
• Ability to validate user .

4.3 Software Interfaces 
The software interfaces are specific to the target WhatsApp users. 

5. Other Nonfunctional Requirements 

5.1 Enhancement Requirements 

1. Last Seen: Client has requested that user be able to see the date and time when his/her contact was last using the application. 
2. User Profile: User should be able to set their profile picture and a status limited to 139 characters.  
5.2 Security Requirements/Software Quality Attributes 
5.2.1. Scalability: WhatsApp should be able to provide instant messaging services to 1 billion users at any given time.  
5.2.2. Privacy: Messages shared between users should be end-to-end encrypted to maintain privacy.  
    
5.2.3. Robustness: In case user’s device crashes, a backup of their chat history must be stored on remote database servers to enable recoverability.   
5.2.4. Performance: Application must be lightweight and must send messages instantly.
  
6. Other Requirements
 
Application must work on all mobile and tablet devices. User interface must be consistent on all devices.    
Long Term Plans  
Future plans include providing inline document viewer that lets users view pdf and word attachments within the application chat window itself. Further optimizations can be made to improve performance especially over the network. This includes making most network specific requests as non-blocking background processes. We also aim to expand our infrastructure to include more database servers so as to take back up of user data more frequently.    Maintenance and Support Costs  
Maintenance will be handled by in house team of developers in the first 6 months post application launch. Within this period, we aim to hit our target of 100,000 users. Once this target is achieved, we intend to outsource maintenance and support to a third party who will be trained for 4 months on system maintenance and troubleshooting.    

