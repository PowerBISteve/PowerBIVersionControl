# Power BI Version Control

Power BI Version Control is a free, full  solution that lets users apply version control, local editing and to PBIX or PBIT files. This is designed fully in the Power Platform and SharePoint environment designed on giving business users or smaller organizations the ability to easily implement version control for their Power BI projects. It is not necessarily design as a replacement for existing enterprise source control solutions.

## Deploying the Solution

### Initial Install

You can install the app for each project.
For full install details, see here: ***???????***

### Set Up

The install will create the required folders on the SharePoint site. 

*Ensure to sync only the* ***Local Development Folder***


##### From SharePoint:
- Navigate to the correct SharePoint site
- Select **Documents** and navigate to the **Local Development Folder** created by the install
- In the toolbar, select **Sync**

##### From Teams:
- Open the teams channel 
- In the toolbar, select **Files** and navigate to the **Local Development Folder** created by the install
- Select **Sync**

You can also add the files to an existing team and selecting **Add Cloud Storage**.

For more info, [see more info on syncing here](https://support.microsoft.com/en-us/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88).

The files in this directory will now be able to be accessed from the local machine.



## How to use

We recommend to [embed the solutions in a Team Chanel](https://docs.microsoft.com/en-us/powerapps/teams/embed-teams-tab), along with a view if the files. This will allow all appropriate members to see the solution in one place.


### Check Out
- Enter the **Check Out** page by the button on the main page
- This will list all PBIX and PBIT files in the **Published Reports** folder. Select the reports you wish to modify in the **Check Out Reports** column 
  *You will only be able to check out reports that are not already checked out*
- Click ***Check in reports*** button
- Wait a few moments for the reports to check out and download. It may take longer if using PBIX or large files


### Editing the files
- Navigate to OneDrive folder on your local machine. The selected reports wil appear in the synced folder **Local Development Folder**
- You can now open and edit these files. If using live connections, consider using the [Hot Swap Connections Tool](https://powerbi.tips/2020/08/hot-swap-report-connections-external-tools/)
- If you want to save copies you can do so in a subdirectory or elsewhere on your local machine. Try to avoid this as much as possible, it is recommended to make small and frequent updates / check ins
- When ready, make sure the ***only*** the files ready for check in are saved in **Local Development Folder**. Makes sure the names of files have not been altered
- If you manually publish reports, publish immediately before closing and checking in


### Check In

Once edits are done, you may choose to Check In the reports to the **Published Reports** folder. Alternatively, you may wish to discard your work. This will release the file and ignore any changes you have made, deleting it from the **Local Development Folder** folder.

#### Commit changes:
- Enter the **Check In** page by the button on the main page
- This will list all PBIX and PBIT files in the **Local Development Folder** folder. Select the reports you wish to Check In in the **Check Out Reports** column
  *You will only be able to check in reports that are checked out to you*
- Make sure to add comments. This should include what was changed. If using DevOps, include task numbers where possible
- Click ***Check in reports*** button

#### Discard changes:
- Enter the **Check In** page by the button on the main page
- This will list all PBIX and PBIT files in the **Local Development Folder** folder. Select the reports you wish to Discard in the **Discard Report** column
  *You will only be able to discard reports that are checked out to you*
- Confirm Discard


  
  

