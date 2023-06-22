# Continuous Integration/Continuous Delivery

You design and implement a (semi)automated software release process that matches the needs of the project context.


In short, CI is a set of practices performed as developers are writing code, and CD is a set of practices performed after the code is completed.

![image](https://github.com/SoleilUmwiza92/PortfolioS3/assets/124836754/cff27c9e-1b21-46d7-9a7f-02a6cc3cf8d7)



Continuous Integration (CI) involves merging code changes from multiple developers into a shared repository frequently. 
The main goal is to catch integration issues and conflicts early by automatically building and testing the codebase. 
This ensures that the software remains in a functional and stable state throughout the development process.

In my Individual project, I am using Github Action workflow to run a build whenever new code is pushed to master branch. 
The steps of the workflow are difined in a YAML file which contains maven build, Sonar quality gate and unit Testing and pushing the jar package to the Docker image.

Continuous Deployment (CD) focuses on automating the release and deployment of software to production environments.
With CD, in the individual project any successfully built and tested changes are automatically published to the Docker image for further deployment to a target environment without manual intervention. 
   

