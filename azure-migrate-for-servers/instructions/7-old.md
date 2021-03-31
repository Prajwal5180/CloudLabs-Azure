# Exercise 7: Migration Validation

At this stage we have assessed our infrastructure, replicated a VM to Azure and migrated it over into an IaaS VM.  It's time to verify our app is up and happy in its new home.

> Tips:
 > * When looking for the failed server, note that the test failover process will append **-test** to your Azure VM

### Task 1: Verify Migration

1. In Azure portal search for **Recovery services vaults** and click on it.

   ![Access and Migrate](image/up1.png)
   
1. Now, open the recovery service vault by clicking on it.

   ![Access and Migrate](image/up2.png)
   
1. In the search bar on the left hand side navigation pane search for *Jobs* and select **Site Recovery jobs**.

   ![Access and Migrate](image/up3.png)
   
1. Click on the job **Test failover** from the list.

   ![Access and Migrate](image/up4.png)

1. On the Replicating Machines blade verify the test migration jobs are all green

   ![Access and Migrate](image/discoverassess-39.png)

1. If the test migration has completed, search for **Virtual Machines** on the search bar at the top of the portal 

1. On the *Virtual machines* blade, you should see one named **webapp01-test**
   
   ![webapptest01](image/virtualmachine.png)
   
1. Click on **webapp01-test**

1. On the **Overview Page** you should see the machine status is **Running**

	>Congratulations! You have successfully migrated the Windows Server 2008R2 server to an Azure IaaS VM.



&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(9)