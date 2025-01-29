# Multiple FiveM Clients

## Introduction
This tutorial is for FiveM developers who are creating interactions or systems with multiple players (Peds). Normally you always have to ask your friend etc. to come to the server to test it. Here I explain how to run FiveM multiple times on one PC with different Rockstar accounts (different identifiers). 

## ⚠️ Important Advices
- Sometimes, when you start the second account, the game freezes and crashes/shuts down. \
**_Solution:_** Restart the FiveM clients
------------------------------------------------------------------------------

## Requirements
> • Multiple official Rockstar Accounts

> Minimal PC Specs:\
> • least 6 CPU Cores\
> • least 32GB RAM\
> • least 8 VRAM\
> __This is just my recommendation!__

------------------------------------------------------------------------------
## Installation

### **Create and save the AccountData file**.
1. Go to your `%AppData%` under `Local/DigitalEntitlements`.
2. Create the `AccountsData` folder.
3. Delete the current **"38d8f400-aa8a-4784-a9f0-26a08628577e "** file (this is where the Rockstar account is stored)
4. Now start FiveM, it will ask you to log in with your Rockstar account.
5. After successful login, the **"38d8f400-aa8a-4784-a9f0-26a08628577e "** file will be created automatically.
6. Now move this file to the new folder "AccountsData" and give it a suffix (in my case I will use **_main account** and **_test account**)
7. Now do step **3. - 6.** again, but with your other Rockstar account
8. You should now have several **38d8f400-aa8a-4784-a9f0-26a08628577e** files in the "AccountsData" folder with the suffix\
![AccountsData Files](https://i.ibb.co/Wk383ws/Accounts-Data.png)


**Create a shortcut to open FiveM with a specific Rockstar account**.

9. Go to your FiveM root folder (should stay in **AppData/Local/FiveM**)\
![FiveM root folder](https://i.ibb.co/1QtQ0QF/FiveMRoot-Folder.png)
10. Copy the **template.bat** into this folder
11. Rename it so you can recognize it (I will call it **"StartMultipleAccounts.bat "** and **"StartTestingAccount.bat "**)
12. Now edit the file with your values
13. Insert in the first copy command the absolute path to your AccountData with the correct suffix in copy parameter 1
14. Insert in the first copy command the absolute path to your DigitalEntitlements folder without the suffix in the copy parameter 2
15. Repeat step **13. - 14.** for the next copy command (for your second account / TestingAccount)
15. Always increase the **-cl** parameter number (your first account should be **-cl1**, your second **-cl2**...)
16. If you don't want to start in windowed mode remove **-windowed** parameter
16. If you want to add more accounts, you can insert the next copy command after **-cl2**.\
![FiveM Start Shortcuts](https://i.ibb.co/YB73rwJ/FiveMStart-Shortcuts.png)

## Examples
### **You can find my examples in the examples folder**
