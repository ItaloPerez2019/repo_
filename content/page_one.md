Title: SSL Certification Management Portal Interface
Date: 2019-11-25 22:00
Category: Help Documentation
Tags: Help Documentation
Slug: Documentation
Authors: Italo Perez
Summary: This document provides guidance and material which is intended to assist the relevant man- agement or technical staff, whether client or application support team, in implementing a pro- ject specific to requirement. It is also useful background reading for anyone involved in devel- oping or monitoring the Netflix Lemur System for COX.

##How to Update This Document

Each section in this document describes the Technical Concept and Solution Narratives for different functionalities of each screen. Some of the detailed information on technical concepts may be contained in either Excel or Word files embedded in this document at each section.
Note: The document will be updated as needed during the build phase, to form the basis of the final system design document to be handed over to COX Business Operations Team.



##Dependencies

Basic prerequisites needed in order to run Lemur:
• Linux operating system
• Python 3.5 or greater
• PostgreSQL 9.4 or greater
• Nginx Web server


##Login in

Authenticate user while user is opening Lemur application in browser. In case of failed authenti- cation, user is prompted with short login fail message.
System will only ask for the user credentials in case:
• User had failed to login due to improper credentials.
• User Lemur account had been deactivated by admin.
• User had intentionally logged out of the application.
Function also sets the user current state (i.e. login/logout state)
