# Access Container Home Page from Cloud Control

## Introduction

This lab walks you through the steps to access the container home page from Oracle Enterprise Manager Cloud Control (Oracle EMCC). You will also learn how to switch between containers and manage your favorites.

Estimated Time: 15 minutes

### Objectives

Access the container home page from Oracle EMCC. Switch between the Container Database (CDB) home page and the Pluggable Database (PDB) home page. Add pages to and remove pages from the favorites.

### Prerequisites

 - Oracle Database 21c installed and a CDB with at least one PDB created.
 - Oracle EMCC 13.5 installed with Oracle Database 19c as the repository.
 - You have completed -
    - Lab: Prepare Setup (*Free-tier* and *Paid Tenants* only)
    - Lab: Setup Compute Instance
    - Lab: Initialize Environment
    - Lab: Log in to Oracle EMCC
 - You have added Oracle Database 21c and the listener as managed targets as explained in this task - [Add Oracle Database and Listener as targets](?lab=manage-targets#Task2:AddOracleDatabaseandListenerastargets).

**Note:** If you have removed the targets Oracle Database 21c and the target listener from Oracle EMCC as per the previous lab, add them again as managed targets. 

## Task 1: Access Container Home page

1.  From the **Targets** menu, select **Databases**.

    ![Databases Menu](../manage-targets/images/emcc-target-005-dbmenu.png)

    The Databases page displays a list of Oracle Databases added to Oracle EMCC as managed targets. Note that the **View** type selected is **Search list**.   
	The values may differ depending on the system you are using.  

    ![Target Added](../manage-targets/images/emcc-target-014-dbhome.png)

2.  On the Databases page, select the Oracle Database name, for example *orcl.us.oracle.com*, and go to **View** > **Expand All Below**. 

    ![Databases Expand All](images/emcc-dbhome-001-expandall.png)

    Alternatively, click on the expand/collapse arrow next to the Oracle Database name. The list displays the database instance and the PDBs for each Oracle Database on the host.

    ![Databases List](images/emcc-dbhome-002-dblist.png)

3.  Click on the container name to access the container home page.

    **Container home page**: If you click the Oracle Database instance name, for example *orcl.us.oracle.com*, it brings up the instance home page.

    ![Oracle Database Instance Home page](images/emcc-dbhome-003-instancehome.png)

    **PDB home page**: If you click the PDB name, for example *orclpdb*, it brings up the PDB home page.

    ![PDB Home page](images/emcc-dbhome-004-pdbhome.png)

From the home page, you can monitor and administer your Oracle Database.

## Task 2: Switch between Containers

You can alter the session and switch between containers in Oracle EMCC within a single login.

This means that from the Database Instance home page, you can switch to the CDB or the PDB home page without logging out of Oracle EMCC. Similarly, from the PDB home page, you can switch to the CDB or to another PDB home page, if more than one PDB exists in the CDB.

1.  Open the container home page for the Oracle Database instance as explained in *Task 1*.   

2.  Click the down arrow next to the container and select **All Containers**.

    ![All Containers](images/emcc-dbhome-005-allcontainers.png)

3.  Select the CDB name, *CDB$ROOT*, from the containers list and click **OK**.  

    ![Container List](images/emcc-dbhome-006-containerlistcdb.png)

    It brings up the CDB home page. 

    ![CDB Home page](images/emcc-dbhome-007-cdbhome.png)

    Similarly, select the PDB name, for example *orclpdb*, from the containers list to open the PDB home page.

    ![PDB Home page](images/emcc-dbhome-004-pdbhome.png)

    **Note**: To jump from one container to another quickly, click the down arrow followed by the container name. The window displays the selected container home page.

    ![Select Container](images/emcc-dbhome-008-selectcontainer.png)

	> You cannot open the Database Instance home page from the CDB or the PDB home page. To open the Database Instance home page, go to the Databases page and click on the Database Instance name, for example *orcl.us.oracle.com*, as explained in *Task 1*. 

## Task 3: View Target Information

To view information about a target or to monitor a target, open the target home page. 

1.  Open the container home page for the Oracle Database instance as explained in *Task 1*.   

2.  From the **Oracle Database** menu, select **Target Information**. 

    ![Target Information](images/emcc-dbhome-009-targetinfo.png)

    Alternatively, you can click on the icon (i) next to the container name.

    ![Container Information](images/emcc-dbhome-010-containerinfo.png)

    The window displays the details of the target container.   

3.  Switch the container to PDB and view PDB details. Click the down arrow next to the container and select the PDB name, *orclpdb*.  
    The values may differ depending on the system you are using.

    ![Select ORCLPDB](images/emcc-dbhome-011-selectpdb.png)

    It opens the PDB home page.  

4.  From the **Oracle Database** menu, select **Target Information**.  
    Alternatively, click the icon (i) next to the PDB name, *orclpdb*.

    ![PDB Information](images/emcc-dbhome-012-pdbinfo.png)

    Similarly, open the CDB home page and view details of the target CDB.

    ![CDB Information](images/emcc-dbhome-013-cdbinfo.png)

## Task 4: Manage Your Favorites

You can add pages to the favorites and bookmark them in Oracle EMCC for easy access. Similarly, you can remove pages from the favorites.

1.  Open the page that you want to bookmark. For example, go to the CDB home page as explained in *Task 2*.

    ![CDB Information](images/emcc-dbhome-007-cdbhome.png)

2.  To add a page to favorites, click the **Favorites** menu (star icon) and select **Add Page to Favorites**.

    ![Image alt text](images/emcc-dbhome-014-favoriteadd.png)

    The window displays a confirmation message that you have added the active page to favorites.   

3.  To remove a page from favorites, click on the **Favorites** menu (star icon) and select **Remove Page from Favorites**.

    ![Image alt text](images/emcc-dbhome-015-favoriteremove.png)

    The window displays a confirmation message that you have removed the page from favorites.

    Moreover, you can open a recently visited page from the **History** menu in Oracle EMCC. 

    ![Image alt text](images/emcc-dbhome-016-history.png)

This brings you towards the successful completion of this workshop on *Oracle EM Database Administration (DBA)*.

## Acknowledgements

-   **Author** - Manish Garodia, Principal User Assistance Developer, Database Technologies

-   **Contributors** - Suresh Rajan, Kurt Engeleiter

-   **Last Updated By/Date** - Manish Garodia, November 2021
