# Use variables to control the pipeline
Users can customize variables to control the execution of subsequent tasks, thus controlling the execution flow of the pipeline
**Assume a scenario: **The stage3 shell script executes when the stage2 shell script executes successfully

1. stage2 shell plug-in sets the status variable

2. ![Set status variable at end of shell script](../../../.gitbook/assets/image-variables-set-status-success.png)

  

3. stage3 shell plug-in select "Run it when all custom variables are macthed"

  ![Select conditional execution](../../../.gitbook/assets/image-variables-run-if-var-set.png)

  

4. The shell plug-in adds' status==success 'as a new execution condition variable
  ![Set execution conditions](../../../.gitbook/assets/image-variables-status-condition.png)

5. If the conditions are met, the command is executed successfully

  ![Execution succeeds if conditions are met](../../../.gitbook/assets/image-variables-run-success.png)

6. Failed to set analog variables
  ![Simulation condition not satisfied](../../../.gitbook/assets/image-variables-set-status-failed.png)

  

7. If the conditions are not met, the plug-in is not executed

  ![Script does not run if conditions are not met](../../../.gitbook/assets/image-variables-skip-if-unsuccess.png)
  Similarly, you can reverse the execution criteria for a plug-in: "Don‘t run it when all the custom variables are macthed"

  ![All user-defined variables do not meet the running time](../../../.gitbook/assets/image-variables-status-condition-not.png)