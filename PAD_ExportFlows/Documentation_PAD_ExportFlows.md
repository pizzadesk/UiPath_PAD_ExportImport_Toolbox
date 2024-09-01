# PAD_ExportFlows

This attended automation allows to export arguments and all subflows of a Flow in PAD.

It is designed for RPA developers or RPA users that have the need to export flows from Power Automate Desktop My Flows section, including flow arguments and subflows.

This ready-to-go automation is fully compatible with PAD_ImportFlows, which allows to import flows from the PAD_ExportFlows created folders/files.


## Prerequisites

This ready-to-go automation has been tested and confirmed working with: 

  1. Minimum display resolution 1024x768
  2. UiPath Assistant 24.10
  3. Power Automate Desktop 2.46 and 2.47, both Store and Standalone installer type
  4. Windows 11 22H2
  5. Windows 10 21H2

## Installation

To install this ready-to-go automation, simply download it from UiPath Assistant 24.10 Marketplace.

## Configuration

This ready-to-go automation requires little configuration.

- Prior to launching the automation, please launch and sign in to Power Automate Desktop. If you fail to do so, you will be prompted during automation. 

- The automation offers to choose and existing or create a new folder for exports at runtime.

## Usage

  1. Run the automation
  2. Select or create new folder that will store exported flow/flows from PAD My Flows section
  3. Define which flows to export from the list of My Flows by entering flow names separated with ;, or type All into prompt to export all flows from My Flows

## Features

- Extract one, several, or all PAD flows from "My flows" page

- Create backups of each subflow in a flow-named folder structure, complete with each Argument (Input/Output variable)

- Export files as .arg for arguments and .subflow for subflows for easy viewing in Notepad

- Examine contents of PAD flow files with WinAutomation syntax

Neat export folder structure:

    Export Folder defined in Browse For Folder prompt
    ——exported_FlowName
    ——-Subflows
    ————Main.subflow
    ————SubflowName.subflow
    ——-Arguments
    ————Input
    —————InputArgument.arg
    ————Output
    —————OutputArgument.arg

## Error Handling and Troubleshooting

Most common error is due to UiPath Browse For Folder activity that presents folder selection dialog underneath active windows.

-   If after the initial message box to select a folder for export, a Browse For Folder does not appear, please check manually if it is hidden underneath any active windows

Second most common error is due to longer time of opening of the Flow Designer panel.

-   If the automation fails at Getting ready screen when opening a specific flow for the first time, please stop the automation, open the flow manually once, and re-run the automation

Third most common error is due to flows appearing in My Flows section of PAD, but they have been deleted in another instance of PAD.

-   When automation opens user-specified flow from My Flows, if it has been deleted inside another instance of PAD for the same user, the deletion have not been yet synced to PAD instance that is being automated. This will result in an error popup in PAD. 

## Limitations

PAD_ExportFlows does not have the capability to extract UI Elements and Images associated with the Flow.

PAD_ExportFlows does not yet have the capability to configure Flow run delays.
