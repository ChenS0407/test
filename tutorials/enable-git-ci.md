# Run bkci in your git repository

## Preparation
* A gitlab project

If not, refer to [Associate your first codebase](link-first-repo.md)

* A bk-ci project
* Understand [basic concept of pipeline](../overview/learn-pipeline-in-5-min.md)

## Listens for codebase push events via BK-CI
1. Create a blank pipeline

2. Add trigger to Job1-1: GitLab

   ![gitlab](../.gitbook/assets/quickstart_4.png)

3. Add Job2-1 to perform compilation tasks

   ![gitlab](../.gitbook/assets/quickstart_5.png)

4. Add the following three plug-ins:   

   * Checkout GitLab

   

   ![gitlab](../.gitbook/assets/quickstart_7.png)

   * Shell Script

     

     ![](../.gitbook/assets/quickstart_8.png)

   * Upload artifacts

     
     
     ![](../.gitbook/assets/quickstart_9.png)

