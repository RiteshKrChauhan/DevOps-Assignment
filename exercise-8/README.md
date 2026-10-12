# Exercise 8: Creating a Hello World Jenkins Job

## Objective
Create and run a Jenkins Freestyle job that retrieves a shell script from GitHub and prints `Hello, Jenkins!`.

## Tools Used
- Windows PowerShell
- Docker Desktop
- Jenkins
- Git and GitHub
- Visual Studio Code

## Procedure
1. Created `hello-world.sh` with the following contents:
   ```bash
   #!/bin/bash
   echo "Hello, Jenkins!"
   ```
2. Committed and pushed the script to the [DevOps-Assignment GitHub repository](https://github.com/RiteshKrChauhan/DevOps-Assignment).
3. Created a Jenkins Freestyle job named `HelloWorld`.
4. Configured Git source control to use the repository's `main` branch.
5. Configured the build step:
   ```bash
   cd exercise-8
   bash hello-world.sh
   ```
6. Ran the job and checked the console output.

## Screenshots

### 1. Script created in VS Code
![Screenshot 1 — Script created in VS Code](images/1.png)

### 2. Script available on GitHub
![Screenshot 2 — Script available on GitHub](images/2.png)

### 3. Jenkins job configuration
![Screenshot 3 — Jenkins job configuration](images/3.png)

### 4. Git and build-step configuration
![Screenshot 4 — Git and build-step configuration](images/4.png)

### 5. Successful Jenkins build
![Screenshot 5 — Console output showing Hello, Jenkins! and Finished: SUCCESS](images/5.png)

## Result
The Jenkins job executed the script and printed `Hello, Jenkins!`. The build completed successfully (`Finished: SUCCESS`).
