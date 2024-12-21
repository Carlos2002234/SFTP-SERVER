# Project Name : PowerShell Command Encoding Detection and Analysis in Azure Sentinel

## Overview
This project uses Azure Sentinel to detect encoded PowerShell commands on devices. The query identifies events with encoded PowerShell flags, extracts and decodes base64 strings, and summarizes unique decoded commands. The results trigger incidents, activating a playbook that sends an email with detailed information for further investigation

Example:
This project helps to create analytic rules in Azure Sentinel to monitor specific activities and generate incidents based on certain queries.

---

## Prerequisites
Before you begin, ensure you have met the following requirements:

- Azure subscription
- Azure VM to run Powershell Script
- Appropriate permissions to create analytic rules and run PlayBooks

---

## Steps to Set Up

### Step 1: Create a New Analytic Rule
1. Navigate to **Azure Sentinel**.
2. Choose **Analytics** from the menu options.
3. Choose **Scheduled** query rule from the menu options.
4. Configure the rule to generate incident
