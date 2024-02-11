
# Task: Setting up Jenkins for Continuous Integration/Continuous Deployment (CI/CD)

Configure Jenkins to automate the build, test, and deployment processes for your application.



## Prerequisites
Install java

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/s1.png?raw=true)

Install Jenkins

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/s2.png?raw=true)

Configure Jenkins

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/s3.png?raw=true)

Create Pipeline Job

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/ss4.png?raw=true)


## Test Cases

## Test Case 1: Integration with Version Control
Make a commit to the version control system and verify that Jenkins automatically triggers a build.

Expected Outcome: Jenkins should detect the new commit and start the CI pipeline
automatically, fetching the latest code changes.

Provide Github Project url

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/s4.png?raw=true)

For Building Trigger, Select Poll SCM on Build Trigger

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/s5.png?raw=true)

Define a pipeline, Apply and Save

Once the commit is made, the pipeline is triggered automatically.

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/s6.png?raw=true)


## Test Case 2: Access Control and Permissions

Restrict access to certain Jenkins jobs or features based on user roles.

Expected Outcome: Users without appropriate permissions should be unable to trigger or
modify Jenkins jobs beyond their assigned privileges.

Add Users

Click on Manage Jenkins-> Users-> Add Users
![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/u.png?raw=true)

Manage Jenkins->Install plugins-> Install role based authorization plugin

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/p1.png?raw=true)

Manage Jenkins-> Security-> authorization->Role based strategy

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/role.png?raw=true)


Manage Jenkins->Manage and Assign Roles->Manage role-> Assign global roles by adding role dev and qa

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/r1.png?raw=true)


Manage Jenkins->Manage and Assign Roles->assign roles->
Assign users to the roles

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/a2.png?raw=true)

Now when you loggin as developer you have no access to any of the jenkins job

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/d1.png?raw=true)

Also when you loggin as qa you have no access to any of the jenkins job

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/q1.png?raw=true)

Now that u assign roles,

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/a1.png?raw=true)


Developer can view, Build the jobs

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/d3.png?raw=true)

Whereas, qa can only view the jobs

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/q2.png?raw=true)

This is all about role based authorization!!


## Test Case 3: Notification Setup
Configure email notifications for build status changes (e.g., success, failure, unstable).

Expected Outcome: Jenkins should send email notifications to designated recipients based on
the outcome of the builds, ensuring timely communication of build statuses.

Install necessary email plugins

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/e.png?raw=true)

Click on Manage Jenkins -> System -> Configure global settings and path

Configure email notification settings

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/ss11.png?raw=true)

Configure extented email notification settings

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/s12.png?raw=true)

Configure Default Trigger 

![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/s13.png?raw=true)

When u build the job and when the build is success, an email notification is sent the given email address with the required message.

- [Jenkinsfile link](https://github.com/shreegs123/Jenkins-Trigger.git)


![App Screenshot](https://github.com/shreegs123/Jenkins-Trigger/blob/main/s14.png?raw=true)





