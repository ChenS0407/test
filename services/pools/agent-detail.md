# Build machine details page
After hosting your build machine to bk-ci, you can view the list of build machines and the details of each one on this page.

## builder list
![In the list, you can check the basic information of the builder and click on the alias to enter the builder details.](../../.gitbook/assets/image%20%2834%29.png)



* **Builder details**

  ![There are 6 functional areas on the builder details page, corresponding to the following functions.](../../.gitbook/assets/image%20%2820%29.png)

  

1. Construct the CPU usage trend chart

2. Create the memory usage trend chart

3. Create the VM network I/O trend chart

4. Create the disk I/O trend chart

5. Copy the installation command: This command is used to reinstall the Agent when the builder reinstalls the system and the Agent directory is deleted

6. Provides 4 important information related to this builder:

   1. Basic information: includes the startup user, installation directory, Agent version, and maximum number of concurrent construction tasks (the default value is 4 to prevent the builder from overloading).
   2. Environment Variables (to be deleted)

   3. Build tasks: All pipeline jobs assigned to this builder will appear here. When you encounter task queuing, you can go here to view specific task assignment information.

   4. Online and offline records of the machine: A record is generated here when the construction machine Agent goes offline.
