# Microsoft 365 Bulk User Import, Encryption, and OneDrive Configuration

This project demonstrates the implementation of key Microsoft 365 features, including bulk user import, email encryption, and OneDrive configuration. The tasks include importing users from a CSV file, setting up email encryption for internal communications, and configuring OneDrive for secure file sharing and retention.

---

## Project Overview

### Key Tasks:
1. **Bulk User Import**:
   - Import 10 users from a CSV file using the Microsoft 365 Admin Center.
   - Assign Microsoft 365 E3 licenses to the imported users.

2. **Email Encryption**:
   - Configure Microsoft 365 Message Encryption.
   - Set up a rule to automatically encrypt emails sent within the organization.

3. **OneDrive Configuration**:
   - Restrict external sharing in OneDrive for enhanced security.
   - Enable a file retention policy to retain data for at least five years.

---

 $~$

 ## Task 1: Bulk User Import

### Steps
1. **Access Microsoft 365 Admin Center**:
   - Navigate to the **Users** section and select **Add multiple users**.

2. **Upload CSV File**:
   - Download the sample CSV file, enter user details, and upload it.

3. **Assign Licenses**:
   - Assign Microsoft 365 E3 licenses to all imported users.

$~$ 
 
![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/1.png)

accessing MS365 Admin Centre and Selecting the Add multiple users option  

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/2.png)

Selecting upload CSV file with user information option and downloading sample file.

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/3.png)
entering 10 user’s details and saving the CSV file

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/4.png)

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/5.png) 

uploaded user details CSV file

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/6.png)

Assigning MS365 E3 License to all 10 users

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/7.png) 

review of adding users 

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/8.png) 

successfully added 10 users

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/9.png)

User’s Display name and Username details

$~$


![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/10.png) 

User’s License details

$~$

## Task 2: Email Encryption

### Steps
1. **Access Exchange Admin Center**:
   - Navigate to the **Exchange Admin Center** and create a new rule.

2. **Configure Encryption Rule**:
   - Set conditions to encrypt emails sent within the organization.

3. **Verify Encryption**:
   - Send an email internally and verify that it is encrypted.

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/11.png)

Accessing Exchange admin center

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/12.png)

Creating Encryption Rule

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/13.png) 

Configuring conditions for the Rule

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/14.png) 

Successfully created and enabled the rule, Rule details

$~$

# Verifying Encryption

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/15.png) 

send an email to user Ricky Martin from user Michael Jackson (Inside organization)

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/16.png) 

received the email from Michael Jackson, and it is encrypted

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/17.png) 

received an email from outside the organization, and it’s not encrypted

$~$

Hence, we can know that the encryption rule is working properly. It’s working for only inside communication as we created.

$~$

## Task 3: OneDrive Configuration

### Steps
1. **Restrict External Sharing**:
   - Configure OneDrive settings to restrict external sharing.

2. **Enable Retention Policy**:
   - Create a retention policy to retain files for at least five years.

Going to configure OneDrive for Business by restricting external sharing for enhanced security, enabling a five-year retention policy for compliance, and setting up a policy to automatically move old files to the Recycle Bin after a year for better storage management.

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/18.png) 

Configure OneDrive settings to restrict external sharing

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/19.png) 

Accessing retention policy under Data lifecycle management in Purview

$~$

 ![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/20.png)
 
Creating Retention policy; entering basic details

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/21.png)

 selecting location for the policy as OneDrive

 $~$

 ![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/22.png)
 
specifying time for retain items

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/23.png) 

successfully created and enabled the retention policy 

$~$


## Key Features

- **Bulk User Import**: Efficiently import and manage multiple users using a CSV file.
- **Email Encryption**: Automatically encrypt internal emails for enhanced security.
- **OneDrive Configuration**: Restrict external sharing and enforce file retention policies for compliance.
- **Automation**: Streamline administrative tasks using Microsoft 365 tools.

---

## Conclusion

This project demonstrates the effective use of Microsoft 365 features to streamline user management, enhance security, and ensure compliance. By automating tasks like bulk user import, email encryption, and OneDrive configuration, organizations can improve efficiency and maintain a secure environment.
