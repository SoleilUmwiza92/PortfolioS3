# Software quality

You use software tooling and methodology that continuously monitors and improves the software quality during software development.

# Peer Review

Peer review or Code review is a practice of four eyes principle where the code is reviewed by another team member to ensure the code quality is maintained during development.

The peer review practice was used during the Group project since we were working in a group and for the individual project, I have to rely on other software that are performing code quality checks, such as Sonar cloud b Quality gate.

# Unit Testing

During development of a software, it is important to test all possible scenarios to make sure that positives and negatives scenarios are handled properly and avoids bugs.

During my Individual Project, I was able to cover Unit testing using Junit5 Jupiter API since the project was Java Spring boot based.

# Integration Testing 

Integration Testing is a practice of testing if different layers of the application are integrated.
The layers used in the Individual project are Frontend, REST API Service and MongoDB database as a backend system.

In my Individual project, integration testing is implemented using **SpringBootTest**, **DataMongoTest** together with **Flapdoodle Embedded MongoDB** where data is not persistent in the real database. 
The implemented Integration testing can be found [here](https://github.com/SoleilUmwiza92/MyMunicipalityRestService/blob/master/src/test/java/com/myMunicipality/documentApi/MyApplicationIntegrationTest.java).

# Quality Gate Checks

Quality Gate checks is a practice of using external services to analyse a project’s code and show potential security vulnerabilities, code smells and bugs.

In the Individual project, Sonar cloud is used to perform code analysis whenever new code is pushed to the master branch as part of the Continuous Integration.
