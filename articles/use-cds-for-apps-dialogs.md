---
title: "Use Common Data Service dialogs for guided processes (Deprecated) | MicrosoftDocs"
description: "Dialogs are the synchronous or interactive processes that collect and process information by using step-by-step scripts to direct users through a process"
ms.custom: ""
ms.date: 10/31/2017
ms.reviewer: ""
ms.topic: "article"
ms.service: flow
ms.assetid: d17f8ae2-854b-4f67-a115-5a03d4f0b8ce
caps.latest.revision: 25
author: "msftman"
ms.author: "deonhe"
manager: "kvivek"
search.app: 
  - Flow
search.audienceType: 
  - flowmaker
  - enduser
---
# Use Common Data Service dialogs for guided processes (Deprecated)
[!INCLUDE [view-pending-approvals](includes/cc-rebrand.md)]

[Dialogs are deprecated](/dynamics365/get-started/whats-new/customer-engagement/important-changes-coming#dialogs-are-deprecated). You should replace dialogs with business process flows or canvas apps. More information: [Replace dialogs with business process flows or canvas apps](replace-dialogs.md) 

Dialogs are the synchronous or interactive processes in Common Data Service that collect and process information by using step-by-step scripts to direct users through a process. For example, you can create dialogs to act as a guide for your service representatives for case resolution and case escalation. Similarly, you can create dialogs for standardizing sales processes such as opportunity qualification and lead scoring.

## Differences between workflows and dialogs

The following table provides information about the differences between Common Data Service workflows and dialogs.  


| Workflows     |    Dialogs      |
|---------------|--------------|
|                                                                                                  Can be either started by a user or can be automated.                                                                                                   |                                                                                          Must be started by a user.                                                                                          |
|                                  Are asynchronous or real-time processes, and do not require user input to run to completion. Asynchronous processes run in the background while real-time processes run immediately.                                   | Are real-time processes that require user input to run to completion. When you run these processes, a wizard-like interface is presented to you so you can make appropriate selections to run the processes. |
|                                                    The entity that stores the details about a running asynchronous workflow is `AsyncOperation` while a `Process` is used for a real-time workflow.                                                     |                                                       The entity that stores information generated by a running dialog is the `ProcessSession` entity.                                                       |
|                  Triggers are supported for workflows. For a list of supported triggers, see [Supported Types, Triggers, and Entities for Processes](/dynamics365/customer-engagement/developer/supported-types-triggers-entities-actions-processes).                   |                                                                                   Triggers are not supported for dialogs.                                                                                    |
  
### See also
[Replace dialogs with business process flows or canvas apps](replace-dialogs.md)