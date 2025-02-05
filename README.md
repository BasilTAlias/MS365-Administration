# Microsoft 365 Implementation Project

This repository contains documentation and scripts for implementing and managing a Microsoft 365 environment. The project focuses on setting up user and group management, configuring security settings, and deploying collaboration tools using PowerShell scripts.

---

## Project Overview

The project involves the implementation and management of a Microsoft 365 environment, including:

- **User and Group Management**: Creating and managing users and groups using PowerShell.
- **Security Configuration**: Ensuring secure access and compliance within the environment.
- **Collaboration Tools Setup**: Enabling and configuring tools like Teams, SharePoint, and OneDrive.
- **Automation**: Using PowerShell scripts to automate repetitive tasks and streamline operations.

---

## Documentation

For a detailed report on the project, refer to the [Creating User with PowerShell.md](#).

---

## Project Files

### Installing Required Modules

To interact with Microsoft 365 services, install the necessary PowerShell modules:

    Install-Module -Name AzureAD
    Install-Module Microsoft. Graph

    
Connecting to AzureAD

    connect-AzureAD


### User creation Script ####


# Define user details
    $users = @(
        @{
            UserPrincipalName = "ProjectUser1@BTech77.onmicrosoft.com"
            DisplayName = "ProjectUser One"
            Password = "password"
            GivenName = "ProjectUser"
            Surname = "One"
            MailNickname = "ProjectUser1"
            AccountEnabled = $true
        },
        @{
            UserPrincipalName = "ProjectU@BTech77.onmicrosoft.com"
            DisplayName = "ProjectUser Two"
            Password = "password"
            GivenName = "ProjectUser"
            Surname = "Two"
            MailNickname = "ProjectUser2"
            AccountEnabled = $true
        }
    )

# Create users
    foreach ($user in $users) {
        $passwordProfile = New-Object -TypeName Microsoft.Open.AzureAD.Model.PasswordProfile
        $passwordProfile.Password = $user.Password
        #$passwordProfile.ForceChangePasswordNextSignIn = $false

    New-AzureADUser -UserPrincipalName $user.UserPrincipalName `
                   -DisplayName $user.DisplayName `
                   -PasswordProfile $passwordProfile `
                   -MailNickname $user.MailNickname `
                   -AccountEnabled $user.AccountEnabled `
                   -GivenName $user.GivenName `
                   -Surname $user.Surname
}


## Key Features
 -   **Automated User Creation**: PowerShell scripts for bulk user creation, reducing manual effort.
    
 -   **Secure Configuration**: Ensures secure access and compliance with Microsoft 365 security best practices.
    
 -   **Scalability**: Easily scalable to accommodate growing organizational needs.
    
 -   **Documentation**: Detailed documentation for easy reference and implementation.

---

## Conclusion

This project demonstrates the effective implementation and management of a Microsoft 365 environment using PowerShell scripts. By automating user creation and ensuring secure configurations, the project highlights the efficiency and scalability of Microsoft 365 for enterprise environments.
