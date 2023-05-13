# Project03-AWSContinuousIntegration
This project aims to demontrate a continuous integration piepline used in typical development and production environments. Continuous integration is implemented in teams to drive teams to implement small code changes and check them in to a repository more frequently. Teams are in need of a way to consistently and constantly integrate and validate these changes. Continuous integration implements an automated way to build, package, and test applications. Having a consistent integration process allows developers to commit code changes more frequently, which leads to better collaboration and code quality.


**EXAMPLE:**
<p>In a typical Agile SDLC environment, developers are making code commits on the regular. These code commits must be built and tested from then on. There will be multiple code changes. These would be exucted by developers or build and release teams. But in this scanrio, code will not be checked so often and bugs will be found out too late. Because of this, the developers would need to take more time to rework all these errors. This could possibly harm the deadline. Even though it needs to be fixed quickly, the build and release team will be doing it manually which would require things like approvals.
  </p>

**SOLUTION:**
* Regular build and text for every commit
* Automated process
* Notify for every build status
* Can fix bugs quicker


 **OBJECTIVE:**

* FAULT ISOLATION
* SHORT MEAN TIME TO REPAIR
* QUICKER TURN AROUND ON FEATURE CHANGES
* LESS DISRUPTIVE
</p>

**Services used:**
* AWS
* Jenkins
* Nexus
* SonarQube
* Slack
</p>

***


<p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI1.png" width="700"  title="hover text">
  </p>
  <p align="center">
  Create security group for jenkins server. Allow SSH, and port 8080.
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI2.png" width="700"  title="hover text">
  </p>
  <p align="center">
  Create nexus security group allowing port 8081 for nexus and SSH.
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI3.png" width="700"  title="hover text">
  </p>
  <p align="center">
  Create sonarqube security group and allow security of jenkins and sonar to allow test results to be uploaded.
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI4.png" width="700"  title="hover text">
  </p>
  <p align="center">
  Go to jenkins SG and allow for sonar to send results back to jenkins.
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI5.png" width="700"  title="hover text">
  </p>
  <p align="center">
  Creat EC2 for Jenkins server. Put in user data that installs java, maven, jenkins.
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI6.png" width="700"  title="hover text">
  </p>
  <p align="center">
  Create EC2 for Nexus server. Put user data that installs nexus.
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI7.png" width="700"  title="hover text">
  </p>
  <p align="center">
  Create EC2 for sonarqube and put user data that installs sonarqube.
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI8.png" width="700"  title="hover text">
  </p>
  <p align="center">
  SSH into jenkins server.
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI9.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI10.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI11.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI12.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI13.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI14.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI15.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI16.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI17.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI18.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI19.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI20.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI21.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI22.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI23.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI24.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI25.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI26.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI27.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI28.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI29.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI30.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI31.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI32.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI33.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI34.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI35.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI36.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI37.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI38.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI39.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI40.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI41.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI42.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI43.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI44.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI45.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI46.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI47.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI48.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI49.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI50.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI51.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI52.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI53.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI54.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI55.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI56.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI57.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI58.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI59.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI60.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI61.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI62.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI63.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI64.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI65.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI66.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI67.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI68.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI69.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI70.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI71.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI72.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI73.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI74.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI75.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI76.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI77.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI78.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI79.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI80.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI81.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI82.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI83.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI84.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI85.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI86.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI87.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI88.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI89.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI90.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI91.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI92.png" width="700"  title="hover text">
  </p>
  <p align="center">
  <img src="https://raw.githubusercontent.com/KaityLeG/Project03-AWSCIPipeline/main/images/JCI93.png" width="700"  title="hover text">
  </p>
