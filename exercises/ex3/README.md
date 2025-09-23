# Transport your pro-code application

In this exercise, we will create a new development project in SAP Build based on the Git Repository created in [Exercise 0](../ex0#exercicse-01---create-a-copy-of-this-repository). We will add small code change release the changes to our Git Repository.

## Exercise 3.0 - Create a new Development Project in SAP Build

1. In SAP BTP cockpit, navigate to your development SAP BTP subaccount named `XP266_DEV`. 
2. Go to **Services** > **Instances and Subscription** and open **SAP Build Code** in the Subscriptions area.
       <br>![](../ex3/images/btp_buildcode.png)
3. The SAP Build Lobby will open. To establish a new development project, click on **Create** > **Clone from Git**.
        <br>![](../ex3/images/buildcode_lobby.png)
4. In Create project popup, set the objective as **Application**, and click **Next**.
5. Choose **SAP Fiori application** and confirm with **Next**.
        <br>![](../ex3/images/buildcode_createproject_type.png)
6. Since this project is based on the Git repository copied in [Exercise 0](../ex0#exercicse-01---create-a-copy-of-this-repository), provide the corresponding repository URL, which can be retrieved from Git.
        <br>![](../ex3/images/git_copyurl.png)
7. Enter a name e.g. **Teched-Development-Project** and optionally a description.
8. Confirm with **Review** and **Create**.
        <br>![](../ex3/images/buildcode_createproject_name.png)
9. The **Business Applicaiton Studio** will open in a new browser tab, preparing your development environment.

## Exercise 3.1 - Add additional sample data to your application

Now that your SAP Build project has been created, you can start development.

1. In your project **CAP-BOOKSHOP_WDI5**, go to **db** > **data** > **sap.capire.bookshop-Books.csv**
        <br>![](../ex3/images/bas_add_content.png)
2. Add addtional entries:
```js
275;The Phoenix Project;"The Phoenix Project: A Novel About IT, DevOps, and Helping Your Business Win is a business novel by Gene Kim, Kevin Behr, and George Spafford. It presents a fictional case study of a troubled IT organization and its journey towards DevOps, emphasizing the importance of collaboration, automation, and continuous improvement.";180;33;14.99;USD;19
276;Italian Journey;"Italian Journey, a travelogue written by Johann Wolfgang von Goethe, recounts his travels through Italy between 1786 and 1788. The work is notable for its detailed descriptions of the Italian landscape, culture, and art, providing a valuable historical perspective.";190;44;11.50;EUR;13
277;Life 3.0;"Life 3.0: Being Human in the Age of Artificial Intelligence is a non-fiction book by Swedish-American physicist and cosmologist Max Tegmark. The book explores the implications of artificial intelligence and discusses potential scenarios of advanced AI impacting human society.";200;55;19.99;USD;16
``` 

## Exercise 3.2 - Release your Changes to GitHub

Now that we have added some changes, the next steps will be to release them to our Git repository

1. In Business Application Studio, open the **Source Control** on the side panel, which has now one pending change.
        <br>![](../ex3/images/bas_sidebar.png)
2. Add a message describing your change e.g. ``Additional books sample data``
3. Click **Commit** and **Sync Changes**
        <br>![](../ex3/images/bas_commit_changes.png)
4. In the popup confirm the push to the main branch
5. At this point you need to allow Business Application Studio to push changes to your repository. Follow the steps as displayed until all configuration is set.
        <br>![](../ex3/images/bas_git_confirmation.png)
6. Back Business Application Studio save your credentials for this session only.
7. Push your changes to git.
        <br>![](../ex3/images/bas_push_changes.png)
8. Your code changes been now added to Git Repository.

## Summary

You've now created your first development project in SAP Build, established code changes and released them to Git.

Continue to - [Transport your low-code application](../ex4/README.md).