# Windows-based UiPath Activities for PAD flow Export and Import

Welcome to the Windows-based UiPath Activities for PAD flow Export and Import repository! This collection of UiPath activities is designed to make backups of Flows in Power AutomateDesktop.
  

## Supported Activities

-  Export all flows in My Flows section of Power Automate for Desktop, looping through each Subflow and storing contents in WinAutomation syntax-based .txt files in Subflow folder.

-  Export each flow Arguments (Input/Output variable panel contents) including all variable propety data, and store in Arguments folder of exported flow.
  
-  Import specific or all flows into My Flows section of Power Automate for Desktop, looping through each Subflow and pasting it's contents from previouslt saved .txt file from a specified Backup folder.
  
-  Import specific or all flow Arguments (Input/Output variable panel contents) including all variable propety data from the Arguments folder for each flow.

-  Folder structure

```plaintext
    Export Folder
    ——ExportedFlow_1
    ——-Subflows
    ————Main.txt
    ————Subflow_X.txt
    ——-Arguments
    ————Input
    —————InputArgument.txt
    ————Output
    —————OutputArgument.txt
```

## Video showcase

-  Export All flows:

https://github.com/user-attachments/assets/6be8fef4-a9eb-4774-ab33-7f65d4309275

-  Import All flows:

https://github.com/user-attachments/assets/ff33376c-c4c8-478f-bfe4-1b83bb497d15




## Getting Started

- Run the process in **Attended mode
- For Export: Select backup folder via popup dialog
- For Import: Select backup-containing folder for all backups at once, or for a specific folder


### Prerequisites

- Install Power Automate for Desktop from Microsoft Store or with MSI Installer

- Keep Power Automate window open before starting the process

- Install UiPath Studio project that is compatible with UiPath.System.Activities version 24.10.3 and UiPath.UIAutomation.Activities version 24.10.0
