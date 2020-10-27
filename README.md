Find and Delete Empty Resource Groups (authenticate with PS Credential)
=======================================================================

            

**DESCRIPTION**


This runbook connects to Azure using login information stored in Automation PS Credential asset and finds (and optionally deletes) resource groups with no resources. 



You can attach a schedule to this runbook to run it periodically for cleanup purposes.


**REQUIRED ASSETS**


An Automation PS Credential asset that contains the Azure AD user credential with authorization for the subscription. Refer to
http://azure.microsoft.com/blog/2014/08/27/azure-automation-authenticating-to-azure-using-azure-active-directory/
 for details on how to have this set up. 


**REQUIRED INPUT PARAMETERS**


AzureCredentialAssetName  - name of the Automation PS Credential asset that contains the Azure AD user credential with authorization for the subscription.



**OPTIONAL INPUT PARAMETERS**


DeleteEmptyGroups - boolean flag that can be set to TRUE to delete empty groups if found. Defaulted to FALSE.


**OUTPUT: **List of resource group names that have no resources.


**OUTPUT TYPE: 
**System.String


**AUTHOR: **Stas Kuvshinov (Microsoft)


**LAST EDIT: **2016-06-01


![Image](https://github.com/azureautomation/find-and-delete-empty-resource-groups-(authenticate-with-ps-credential)/raw/master/2016-06-01.PNG)


 






        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
