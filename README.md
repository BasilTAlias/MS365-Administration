# Microsoft 365 Implementation Project

This repository contains documentation and scripts related to implementing and managing a Microsoft 365 environment.

## Project Overview
The project involves setting up and managing a Microsoft 365 environment, including user and group management, security configuration, collaboration tools setup, and more.

## Documentation
For a detailed report on the project, refer to the Creating User with Powershell pdf Doc.

## Project Files

## Installing Modules

    Install-Module -Name AzureAD
    Install-Module Microsoft. Graph

    
## Connecting to AzureAD

    connect-AzureAD


###User creation Script####


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


#########################
