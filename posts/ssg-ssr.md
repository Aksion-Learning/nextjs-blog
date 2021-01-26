---
title: "How to Make a Composition Service for Twilio Video with Node.js"
date: "2020-12-25"
---

We will build a service that will handle recordings of many video calls. These calls will be processed, their audio files extracted, and finally, uploaded to cloud storage for access by end-users.  
For this purpose, we will use a queueing system which will deal with two different parts. The first part will be responsible for receiving video room metadata as soon as a video call ends.  
The second part will be responsible for processing related audio recordings.
The duration of this second part may be between 30 minutes and 24 hours for each composition.  
This queueing system will take care of the expected delays and failures of each part of the service.

### The Technologies Used to Build the Service:

**Data and File API:**

Twilio for video calls, recording, and composition backups.  
Google Drive for extracted recordings.

**Queue Management:**

Redis for queue management.  
Bull for queueing with NodeJS.  
Taskforce. sh for monitoring queues.
for full article [visit Medium](https://medium.com/@rasha.abdulrazzak/how-to-make-a-composition-service-for-twilio-video-with-node-js-feb2ba851d6b)
