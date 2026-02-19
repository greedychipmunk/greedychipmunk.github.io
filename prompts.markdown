---
layout: default
title: "Prompts"
permalink: /prompts/
---

# Prompts

## Useful and effective prompt ideas

Please teach a software engineer who is new to Letta and Mem0 how to efficiently self-host both applications. Please suggest novel and creative monetization strategies. Please discuss how this combination can support the following use cases:
- an e-commerce application selling apparel through a third party printer.
- an e-commerce application selling digital planners
- a mobile HIIT workout application
- a productivity application that set goals and tracks progress

---

Please explain in detail every concept to an absolute beginner. Please define all jargon and key terms. Please include analogies and silly mnemonics to aid in understanding and remembering complex concepts. Outline which machine learning algorithm (along with any relevant Python libraries and methods) I should use for specific predictive tasks. Please suggest novel and creative monetization strategies. Also suggest money-making projects that I can start today that will impress hiring managers at top companies.

---

## System design: Instagram

Explain the concepts of horizontal scaling and load balancing as if teaching a system design interview beginner. 
- Use the photo upload process versus feed retrieval as concrete examples for where these patterns are critical.
- Describe how scaling applies differently to the relational database metadata versus the distributed object storage for images.
- Contrast the caching policy used for read operations with the write through update mechanism described.
- Detail the role of the dedicated feed generation service and why it runs on a schedule instead of dynamically per request.
- Structure the explanation by strictly separating all components involved in the read path versus all components involved in the write path before discussing shared elements.
- Calculate the total data storage needs based on the initial 10 million user scale estimate provided in the discussion.
- Conclude by summarizing the three most critical trade-offs an interviewer might challenge a candidate on regarding this Instagram design.

---

## System design: 

Explain the system design concepts using simpler analogies suitable for an audience new to software architecture principles. 
- Detail the process of handling image uploads including transcoding and storage using layman terms.
- Describe how geographical information is partitioned using geo sharding to quickly find local users.
- Describe the backend architecture required for private messaging threads including secure exchange of messages and media.
Include a summary of the scale estimates specifically detailing the projected storage needed for profile photos and daily message volume.
- Illustrate the backend sequence triggered when two users swipe right on each other to finalize and confirm a successful match.
- Detail why the system maintains separate User IDs and Profile IDs during profile creation and management as discussed in the profile structure.
- Explain the necessary backend logic to support and track a Super Like interaction between users.
- Elaborate on the filtering logic within the recommendation service used to exclude inactive users based on login time.
- Describe the rationale for treating system monitoring and logging as a secondary component for this design session.
- Detail the design implications for integrating the subscription system for premium features.
- Explain the specific storage and delivery pipeline utilized when users exchange photos or videos within a private messaging thread.
- Outline the entire system design process starting from initial requirements gathering through database selection and API structure summary

---

Structure the explanation as a step-by-step walkthrough of a single message transmission and receipt cycle. 
- Detail the initial steps describing how the sending user connects to the service infrastructure.
- Focus specifically on the sequence of events that generate the 'Delivered' and 'Read' receipt indicators for the sender. Analyze the encryption protocols used to secure data transmission between users.
- Discuss the dedicated storage architecture used when handling large binary attachments like images or videos.
- Summarize the core architectural decisions that prioritize low latency for real time text delivery over immediate delivery receipt finality.
- Detail how the system tracks and broadcasts the presence status of users across distributed servers.
- Detail the initial steps describing how the sending user connects to the service infrastructure.
- Compare the complexity of the fan out process for one to one messages versus sending updates across large participant groups.
- Elaborate on how end to end encryption impacts the logging and receipt generation mechanisms discussed earlier.
This entire technical flow must be explained using analogies suitable for someone new to cloud infrastructure concepts.

