# ClaimChampions
# Claim Assistant Capgemini – Copilot Studio Solution

This repository contains the exported solution from Microsoft Power Platform featuring the "Claim Assistant Capgemini" agent, designed to automate the vehicle claim process using AI and Azure services.

## Overview

The agent was developed using Microsoft Copilot Studio (formerly Power Virtual Agents) and automates end-to-end vehicle insurance claim interactions, including greeting users, collecting claim details, uploading images and police reports, and escalating to human support when needed.

## Included Components

### Bot Topics

- **Greeting** – Welcomes the user  
- **Goodbye** – Ends the conversation  
- **StartOver** – Restarts the chat  
- **Fallback** – Handles unrecognized input  
- **Signin** – Captures and validates user data (e.g., CPF or ID)  
- **Search** – Looks up customer information  
- **UploadImage** – Allows users to upload accident images  
- **ReadPoliceReports** – Processes police reports using OCR  
- **Escalate** – Escalates the case to a human agent  
- **ThankYou**, **ResetConversation**, **MultipleTopicsMatched** – Supporting interactions  

### Power Automate Workflows

- Flows triggered by the agent  
- Connectors to external APIs and Azure services  

## Integrated Services

- **Azure OpenAI** – Provides natural language generation for a conversational experience  
- **Azure Functions** – Executes custom backend logic such as renaming files with timestamps  
- **Azure Blob Storage** – Stores uploaded files like accident images and police reports  
- **Power Automate** – Orchestrates logic, API calls, and backend integration  
- **AI Foundry (Azure)** – Processes accident image analysis (e.g., damage detection, vehicle classification) with computer vision and AI agents  

## How to Import

1. Go to [https://make.powerapps.com](https://make.powerapps.com)  
2. Select the target environment  
3. Navigate to **Solutions > Import Solution**  
4. Upload the provided `.zip` file from this repository  
5. Publish all customizations  

## Notes

- This solution is exported as **Unmanaged**, so you can edit it after importing.  
- Azure credentials (OpenAI, Blob Storage, Functions, AI Foundry) must be configured manually inside Power Automate flows.  

---

Developed as an intelligent claims automation assistant for Capgemini.
