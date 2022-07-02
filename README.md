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
- Search for "recommendation" - select Security Center Recommendation - it will create a connection.
- Create a new step so search for an outlook connector where we want to send an email.
- Enter the email address you want the alert to be sent to.
- Select Dynamic content - properties and properties display name
- Save the workflow.
- Go to Microsoft Defender for Cloud and add the workflow automation.
