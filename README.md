# DevOps Pipeline in Thingworx
### Introduction
This documentation is about Git Devops Setup on the Thigworx and Pushing/Pulling the Entities to Azure Devops Repo. The Total process is based on Thingworx 9.2.1.

#### Setting up the Github Backup extension:
•	Download Github Extension from this link
•	Import the Extension in to the Thingworx (Thingworx should be Licensed)
•	Create Thing based on Thing Template GitBackup Template
•	Do the Following Configurations in the Created Thing. (Get the Git Credentials from the Repo from the Azure Devops)
![image](https://user-images.githubusercontent.com/67698473/168417030-56d47c81-be13-49a3-a142-06ca1dad351d.png)
•	Go to mashup and Open the GitBackup.Main.Mashup and click on PULL button to merge master branch with the repo.

#### Pushing Entities to Azure Devops Repo

1. Click on Export button. Select the Project whose entities need to be pushed to the repo and click Export Entities button.
2. Select the entities and click on Add button. After selecting all the required entities click export Button.
3. (optional) To export the extensions, click on Export Extension Button.
4. (optional) All the extensions gets dump from the system. It is recommended to go to the Extensions folder and remove the Extensions which are not needed. 
5. Go to Main Tab and click on Push button to push the entities to the repo with a push message.
6. You can check the push was successful in your Git browser
7.	Go to Azure DevOps and check the entities in the repo.

#### Pulling Entities from Azure Devops Repo

1.	  Click the Pull button from the Main tab of the GitBackup.Main.Mashup.
2.    Click on Workspace Tab. Expand the project and select the entities. Click on Import entity.
3.    (optional) To import Extensions, Select the extension and click on Import Extension Button.
