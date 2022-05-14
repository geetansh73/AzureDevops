# DevOps Pipeline in Thingworx
### Introduction
This documentation is about Git Devops Setup on the Thigworx and Pushing/Pulling the Entities to Azure Devops Repo. The Total process is based on Thingworx 9.2.1.

#### Setting up the Github Backup extension:
•	Download Github Extension from this link
•	Import the Extension in to the Thingworx (Thingworx should be Licensed)
•	Create Thing based on Thing Template GitBackup Template
•	Do the Following Configurations in the Created Thing. (Get the Git Credentials from the Repo from the Azure Devops)

![image](https://user-images.githubusercontent.com/67698473/168418576-19996173-3b57-4b95-8c6c-84fef70116ee.png)


![image](https://user-images.githubusercontent.com/67698473/168417088-54fd2099-cdc2-49cd-b841-7ccbc182546f.png)

###### •	Go to mashup and Open the GitBackup.Main.Mashup and click on PULL button to merge master branch with the repo.

![image](https://user-images.githubusercontent.com/67698473/168417115-c77f2393-344a-4e28-acf2-99f42803647b.png)

#### Pushing Entities to Azure Devops Repo

1. Click on Export button. Select the Project whose entities need to be pushed to the repo and click Export Entities button.

![image](https://user-images.githubusercontent.com/67698473/168417137-b3346680-5abf-43f8-901a-cb789d1d29ad.png)

2. Select the entities and click on Add button. After selecting all the required entities click export Button.

![image](https://user-images.githubusercontent.com/67698473/168417157-7d0b477b-a1f4-4186-87b1-2180dd82352d.png)

3. (optional) To export the extensions, click on Export Extension Button.

![image](https://user-images.githubusercontent.com/67698473/168417185-9957f4a8-92a6-4c15-bb89-871a84d0aaa4.png)

4. (optional) All the extensions gets dump from the system. It is recommended to go to the Extensions folder and remove the Extensions which are not needed. 

![image](https://user-images.githubusercontent.com/67698473/168417217-faac498f-d8ff-45a1-ab4a-6bebbb6fd534.png)

5. Go to Main Tab and click on Push button to push the entities to the repo with a push message.

![image](https://user-images.githubusercontent.com/67698473/168417227-ecf5413e-9940-46b8-ab00-e8aa1ca1869a.png)

6. You can check the push was successful in your Git browser

![image](https://user-images.githubusercontent.com/67698473/168417237-9e2c6f88-0463-4d03-b87e-ff2a35e8cb67.png)


7.	Go to Azure DevOps and check the entities in the repo.

![image](https://user-images.githubusercontent.com/67698473/168417246-564bed78-0d2c-4a7d-b802-f020023fe8c8.png)

#### Pulling Entities from Azure Devops Repo

1.	  Click the Pull button from the Main tab of the GitBackup.Main.Mashup.

![image](https://user-images.githubusercontent.com/67698473/168417265-665c8f8b-b299-445e-8ded-5ca7a75985ac.png)

2.    Click on Workspace Tab. Expand the project and select the entities. Click on Import entity.

![image](https://user-images.githubusercontent.com/67698473/168417281-a9d46047-a75c-4be7-9e42-7a0020d50ad4.png)

3.    (optional) To import Extensions, Select the extension and click on Import Extension Button.

![image](https://user-images.githubusercontent.com/67698473/168417290-440c0b6b-ca46-4a9c-8db6-959d6ba8b737.png)
