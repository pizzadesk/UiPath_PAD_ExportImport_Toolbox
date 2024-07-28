# Windows-based UiPath Activities for PAD flow Export and Import

Welcome to the Windows-based UiPath Activities for PAD flow Export and Import repository! This collection of UiPath activities is designed to make backups of Flows inPower Automate for Desktop.
  

## Supported Activities

- Export all flows in My Flows section of Power Automate for Desktop, looping through each Subflow and copying it's contents to save into a .txt file in a specified Backup folder.

- Import specific or all flows into My Flows section of Power Automate for Desktop, looping through each Subflow and pasting it's contents from previouslt saved .txt file from a specified Backup folder.

- ![Screenshot 2024-07-22 103908](https://github.com/user-attachments/assets/7db12c4c-2a60-4e7e-9694-fc3e257ffa73)


## Video showcase

https://github.com/user-attachments/assets/28f1399a-2f67-4a2f-b83a-05189e7a9526


## Getting Started

- Run the process in **Attended mode
- For Export: Select backup folder via popup dialog
- For Import: Select backup-containing folder for all backups at once, or for a specific folder


### Prerequisites

- Install Power Automate for Desktop from Microsoft Store

- Keep Power Automate window open before starting the process

- Install UiPath Studio project that is compatible with UiPath.System.Activities version 24.10.3 and UiPath.UIAutomation.Activities version 24.10.0



### Installation

1. Clone this repository to your local machine.

   https://github.com/pizzadesk/UiPath_PAD_ExportImport_Toolbox.git
