# DynamicsAXVersionControl 
#Summary

This repository extends the Microsoft Dynamics AX 2012 R3 Version Control Sytem. The work within will offer new features that will remove some pain points that exist with the base system. 

#Change Log:

07/17 2016 - Added functionality to separate unprocessed items by AOT group from the Synchronize Log form. I recently dealt with having a malformed .xpo that prevented synchronization with TFS. The infolog only stated that there was an error on line 170, but it did not tell me which file. When using the current process feature from the Synchronize Log form, all items that belong to the same batch id (the synchronization field), will attempt to resync. This is an existing pain point, as all of the items were stored with a batch id of one (1). Separating into smaller batches will allow you to quickly identify the .xpo that is causing the error. 
