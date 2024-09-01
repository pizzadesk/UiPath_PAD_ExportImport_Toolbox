# PAD_ImportFlows


This attended automation allows to import arguments and all subflows of a Flow into PAD.

It is designed to supplement PAD_ExportFlows ready-to-go automation and import flows into Power Automate Desktop My Flows section, including flow arguments and subflows.

This ready-to-go automation is fully compatible with PAD_ExportFlows, which allows to export flows from the PAD_ExportFlows created folders/files.

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

- The automation prmompts the user to define a folder with previous export of PAD_ExportFlows.

## Usage

  1. Run the automation
  2. Select a folder that contains either all previous "exported_FlowName" exports, or select a "exported_FlowName" folder to import only one flow
    
## Features

- Import one or all PAD flows into "My flows" page

- Leverage PAD_ExportFlows .arg and .subflow files to import nearly all Subflow data, complete with each Argument (Input/Output variable)

- Use .arg for arguments and .subflow for subflows files in Notepad

- Examine contents of PAD flow files with WinAutomation syntax

Neat export folder structure:

    Improt Folder as defined in Browse For Folder prompt
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

Most common error is due to longer time of opening of the Flow Designer panel.

-   If the automation fails at Getting ready screen when opening a specific flow for the first time, please stop the automation, open the flow manually once, and re-run the automation


## Limitations

PAD_ImportFlows does not have the capability to import UI Elements and Images associated with the Flow.

PAD_ImportFlows does not yet have the capability to configure Flow run delays.
