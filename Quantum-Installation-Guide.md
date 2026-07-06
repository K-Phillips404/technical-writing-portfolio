# Quantum Project Manager Installation Guide

## Audience: Help Desk Technicians

## Purpose: 

This procedure installs the Quantum Project Manager software on a Windows workstation and connects to an existing data repository.

## Prerequisite:

- The 64-bit version of Microsoft Access must be installed prior to installing Quantum, or Quantum will install a 32-bit version of Access Runtime during installation. This can lead to Office compatibility issues later.
    - If you do not have access installed and want to keep things 64-bit you can install Microsoft Access Runtime 64-bit from this link on Quantum’s website: https://www.quantumss.com/projectmanager/downloadAccessRuntime.htm
- The user must be a local administrator during the installation or directories will be mapped wrong.
- Registration information — including the specific version of your company name, product serial number, registration number, and installation password — must be obtained from Quantum support by calling or emailing them at (610) 373-483, or support@quantumss.com. 

## Installation steps:

1. Navigate to http://www.quantumss.com/projectmanager/download230.htm
2. Select Download Quantum Project Manager Version 23.0c
3. Right click on setup and run as administrator
4. Follow the on screen prompts until asked for the installation password. 
5. Input the password obtained from support.
6. Continue to follow prompts.
7. After installation, you might see a Program Compatibility Assistant message stating the program may not have installed correctly. Select the option that says, “this program installed correctly.”
    - Per Quantum Support is normal behavior.
8. Double Click the desktop shortcut.
    - If you do not see a desktop shortcut, confirm the user is a local administrator. If not, you will have to repeat the installation after granting the user local admin privileges. These privileges may be revoked after installation.
9. If this is an upgrade, you will be met with a message about importing or converting data. Follow prompts and click OK. The program will restart.
10. You will be asked to register the product. Input the registration number obtained form Quantum Support and click yes.
11. The next screen will state the program is locked. Select "unlock via the internet," then click "click here to unlock."
12. If the unlock fails, you will need to contact support.
13. On the program home screen, select the button labeled preferences.
14. In the data location box, select or paste the UNC path to the Quantum Data Repository. 
    - Example: \\ServerName\sharedfolder\QuantumnData
15. Select the file.
    - The file type will be .accdb

## Verification:

Confirm the following:
- Quantum Project Manager launches successfully.
- The application unlocks.
- The user can access and edit company data
