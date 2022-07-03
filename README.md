# Custom-Initiatives

# Recommendations from Microsoft Defender for Cloud
- These recommendations are coming from the Azure Security Benchmark policies

# How to create custom initiatives for Storage Accounts?
- Create an Azure storage account
- Go to Azure Policy Service and create an initiative

# Create initiative
- Add policy definitions 
- Select policies related to storage


# Assign the initiative onto your subscription


# Add custom initiatives created within Microsoft Defender for Cloud
- The initiatives added will be used to compare against your resources and provide recommendations


# Microsoft Defender - Security Alerts
1. Notifications can be generated if there are threats detected on resources.
2. For Enhanced Security features ONLY
3. When there are multiple alerts, Defender for Cloud can create a security incident that is based on the related alerts.
4. Alerts will get classified - High , Medium , Low , and Informational

# Example - Security Alerts
- If a new user resets an admin credentials for a virtual machine, a security alert will be generated on Microsoft Defender for Cloud


# Microsoft Defender - Workflow Automation
- We can trigger a workflow automation via logic apps to remediate or implement the recommendation.


# Use Case: Deploy Azure Logic Apps to remediate a vulnerability using the recommendation
- Trigger the logic app where the logic app sends an email to you regarding an alert.
- Within Logic App Designer - create a blank logic app

# Create the logic app 
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177019544-ca5656dc-dc7e-4838-97b2-17055460ee19.png" height="75%" width="75%" alt="Azure LAW"/>

<p/>

# Select the Azure Security Center Recommendation trigger or Microsoft Defender for Cloud
- Search for "recommendation" - select Security Center Recommendation - it will create a connection.
- Microsoft Defender was previously known as Azure Security Center

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177019557-dd576833-dfca-48f1-9639-59d270e476c5.png" height="75%" width="75%" alt="Azure LAW"/>

<p/>

# Create a new step and create outlook connector 
- Select the "Send an email" trigger and authenticate with outlook email 
- Enter the email address you want the alert to be sent to.
- Select Dynamic content - properties and properties display name
- Save the workflow.

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177019615-18ff3f36-e34b-4b48-9f79-5f92e30a1929.png" height="75%" width="75%" alt="Azure LAW"/>

<p/>


# Go to Microsoft Defender for Cloud and add the workflow automation.
- Click save.
- Wait about 15-20 minutes for an email providing a security recommendation.
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/177019565-d2081a14-168f-4d72-8398-85814716ba68.png" height="75%" width="75%" alt="Azure LAW"/>

<p/>

