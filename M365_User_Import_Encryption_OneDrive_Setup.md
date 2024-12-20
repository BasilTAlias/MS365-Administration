# Import Bulk Users

- Use the Microsoft 365 admin center to bulk import 10 users from a CSV file.
- Assign appropriate licenses (Microsoft 365 E3) to the imported users.

 $~$
 
![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/1.png)

accessing MS365 Admin center and Selecting Add multiple user’s option  

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/2.png)

Selecting upload CSV file with user information option and downloading sample file.

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/3.png)
entering 10 user’s details and saving the csv file

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/4.png)

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/5.png) 

uploaded user details csv file

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

# Set Up Data Encryption

- Configure Microsoft 365 Message Encryption.
- Ensure that emails from inside the organization are automatically encrypted. (Hints: Navigate to Exchange admin center, and then Rules)

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/11.png)

accessing Exchange admin center

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/12.png)

creating a Rule

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/13.png) 

configuring Conditions for the Rule

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/14.png) 

successfully created and enabled the rule, Rule details

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

# Implement OneDrive for Business
- Configure OneDrive settings to restrict external sharing.
- Enable file retention policies to ensure data is retained for at least five years.

Going to configure OneDrive for Business by restricting external sharing for enhanced security, enabling a five-year retention policy for compliance, and setting up a policy to automatically move old files to the Recycle Bin after a year for better storage management.

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/18.png) 

Configure OneDrive settings to restrict external sharing

$~$

![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/19.png) 

accessing retention policy under Data lifecycle management in Purview

$~$

 ![Alt text of the image](https://github.com/BasilTAlias/MS365-Projects/blob/main/Images/M365_User_Import_Encryption_OneDrive_Setup/20.png)
 
creating Retention policy; entering basic details

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
