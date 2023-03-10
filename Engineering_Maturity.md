# Engineering Maturity Model Template
  
  
## ORG NAME
Total Score: 5
  
### Development
Score: 5
  
##### Documentation
Score: 5  
Max Score: 5  
Description:  
Level 1 - Little to No docs.  
Level 2 - Onboarding and dev env setup docs exists.  
Level 3 - SD Process docs exists - a developer can create and submit work on their own. Guidelines for code styling, repo structure, branch structure, submitting PRs, etc.  
Level 4 - Detailed architecture docs exist, including interservice communications (REST API, MB messages, etc.), DB schemas, etc.  
Level 5 - a new person can successfully start, get familiar with, work, maintain and develop the project without any assistance. Docs are in an easy to use format and tools - ex. Postman or Swagger.  
  
##### Onboarding
Score: 5  
Max Score: 5  
Description:  
Level 1 - No documentation, onboarding is done by a member of the team  
Level 2 - Some onboarding docs exist. A member of the team walks a new starter through the process  
Level 3 - Detailed onboarding docs and plan exist, that a new starter can follow on their own  
Level 4 - Semi-automated onboarding  
Level 5 - Fully automated onboarding process, including all accounts, info on systems, meet & greet, process info, etc. New starters receive all information & accounts they would need to successfully work on the project and the process is automated as much as possible  
  
##### Local Env Setup
Score: 5  
Max Score: 5  
Description:  
How automated and easy the local environment setup is:  
Level 1 - Fully manual setup  
Level 2 - Uses a package manager. Setup documentation exists.  
Level 3 - Uses a package manager. Setup is semi-automated via running different scripts / commands, which are well documented.  
Level 4 - Setup is fully automated, but not including the required 3rd parties (ex. DB, ELK, etc.).  
Level 5 - Setup is fully automated by running 1-2 commands, which are well documented. This includes download and install of all 3rd parties (ex. DB, ELK, etc.). It is ok to have 1-2 prerequisets - ex. Docker, k8s.  

##### IDE Setup
Score: 5  
Max Score: 5  
Description:  
Level 1 - Everything is done manually, no docs or unification  
Level 2 - Docs exists how to manually setup the IDE  
Level 3 - Code styling rules and config exists in the repo and can be imported in the IDE  
Level 4 - Detailed docs exist on IDE setup  
Level 5 - IDE setup is fully automated and unified across all devs  

##### Pre-commit Hooks
Score: 5  
Max Score: 5  
Description:  
Level 1 - No pre-commit hooks  
Level 2 - Pre-commit hook for linting, stopping commit on errors  
Level 3 - Pre-commit hook for build, stopping commit on errors  
Level 4 - Pre-commit hook for automated tests, stopping commit on errors  
Level 5 - Fully automated pre-commit hook setup, including automatic linting errors fix  

##### Knowledge and Skills Sharing
Score: 5  
Max Score: 5  
Description:  
How much of the knowledge and skills are shared across the team - can they successfully cover for each other:  
Level 1 - No knowledge sharing processes exist. Team members are highly specialized in a particular part of the project and cannot cover for each other  
Level 2 - Knowledge sharing exists only in the form of documentation. Team members are highly specialized in one area, but have a little understanding of the technologies used in other areas as well  
Level 3 - Regular knowledge sharing happens in the team. Team members are familiar with all areas and technologies in the product and can work on any area with supervision and guidance from another member. They can cover for each other on small tasks with noticeable productivity loss  
Level 4 - All team members have the necessary knowledge and skills to work on all parts of the product at any time, with some noticeable productivity or quality loss  
Level 5 - All team members have the necessary knowledge and skills to work on all parts of the product at any time, without noticeable productivity loss  


### Testing
Score: 5

##### Unit Tests
Score: 5  
Max Score: 5  
Description:  
Unit tests coverage as a percentage of the total code base:  
Level 1 - 0-20%  
Level 2 - 20-40%  
Level 3 - 40-60%  
Level 4 - 60-80%  
Level 5 - 80-100%  

##### Functional
Score: 5  
Max Score: 5  
Description:  
Percentage of automated functional testing, of all test scenarios - this includes E2E scenarios:  
Level 1 - 0-20%  
Level 2 - 20-40%  
Level 3 - 40-60%  
Level 4 - 60-80%  
Level 5 - 80-100%  

##### Regression
Score: 5  
Max Score: 5  
Description:  
Regression Cycle:  
Level 1 - Fully manual regression cycle taking several days  
Level 2 - Mostly manual regression with some automated tests, covering mostly P1 critical paths / scenarios. Regression takes several days. Hotfixes can be done within 1-2 days with minimal focused manual testing  
Level 3 - Automated tests covering all P1 critical and P2 major paths / scenarios. Fully automated sanity / smoke tests, executed at least daily. Hotfixes can be done in a few hours with no manual testing  
Level 4 - Regression is fully automated. It might not cover all corner cases or all product configurations. Regression can take up to several hours, but no more than 24h. Releases can be done reliably with automated checks only  
Level 5 - Regression is fully automated and happens in a matter of minutes (1h at most), allowing rapid, reliable and frequent releases. Close to no flaky tests. Flaky tests are rerun and if a flaky test is noticed, a ticket is automatically created to fix it  

##### Static Code Analysis
Score: 5  
Max Score: 5  
Description:  
Level 1 - No static code analysis  
Level 2 - Ad-hoc manualy executed static code analysis  
Level 3 - Static code analysis is executed regularly on a dedicated server, covering at least 1 area of the code base  
Level 4 - Static code analysis is executed regularly on a dedicated server, covering areas of the code base. It is checked by a human regularly and problem areas are addressed on time  
Level 5 - Detailed static code analysis, including code complexity, code maintainability, estimated bug rate, potential security issues. Execution is automatic on every build, issues and code degradation prevent PR merging  

##### Performance
Score: 5  
Max Score: 5  
Description:  
Level 1 - No performance testing  
Level 2 - Limited manual performance testing is done on an ad-hoc basis  
Level 3 - Thorough manual performance testing is done regularly, covering all needed areas  
Level 4 - Semi-automated performance testing is done. It might not include things like automatic catching and reporting of performance degradation issues  
Level 5 - Fully automated performance testing is done regularly. No manual involvement is needed. Issues are reported automatically  

##### Security
Score: 5  
Max Score: 5  
Description:  
Level 1 - No security testing  
Level 2 - Limited manual security testing is done on an ad-hoc basis by internal or external experts. Members of the team have basic knowledge about security  
Level 3 - Thorough manual security testing is done regularly, covering all needed areas. Members of the teamare familiar with the most common security issues and best practices  
Level 4 - Semi-automated security testing is done, including static and dynamic code analysis. Members of the team are very familiar with security and pass regular security trainings.  
Level 5 - Fully automated security testing is done regularly. No manual involvement is needed. Issues are reported automatically. Regular security audits are done  

##### Accessibility
Score: 5  
Max Score: 5  
Description:  
Level 1 - No accessibility testing  
Level 2 - Limited manual accessibility testing is done on an ad-hoc basis by internal or external experts. Members of the team have basic knowledge about accessiblity  
Level 3 - Thorough manual accessibilitytesting is done regularly, covering all needed areas. Members of the team are familiar with the most common accessibility issues and best practices  
Level 4 - Semi-automated accessibility testing is done. Members of the team are very familiar with accessibility and pass regular trainings.  
Level 5 - Fully automated accessibility testing is done regularly. No manual involvement is needed. Issues are reported automatically.  


### DevOps
Score: 5

##### Build
Score: 5  
Max Score: 5  
Description:  
Level 1 - Ad-hoc manual builds on a developer machine  
Level 2 - Ad-hoc manual builds on a dedicated server  
Level 3 - Automated build, including code linting, tests, etc. Artefacts are uploaded on a shared server / artifactory. Build result and links are automatically updated in the PR. Failed builds prevent PR merging  
Level 4 - Build environment is available as code - ex. containers.  
Level 5 - Modular build - build only modules / services that have changed. Build happens in <10 mins  

##### Environments
Score: 5  
Max Score: 5  
Description:  
Level 1 - No shared dev / test environments  
Level 2 - Manually managed dev / test environments exists, covering the needs - ex. dev, test, staging, etc.  
Level 3 - Semi-automated environment management exists using various ad-hoc scripts. All environments have proper SSL certificates and domain names  
Level 4 - Fully automated single environment setup, using a proper system to trigger it  
Level 5 - All environments all available as Infrastructure as code, including all supporting systems - ex. build server, artifactory, etc. New environments can be spinned up automatically in a matter of seconds. The whole infrastructure can easily be spun up from code. Easy way to replicate prod environments, including anonimizing client data  

##### Deployment
Score: 5  
Max Score: 5  
Description:  
Level 1 - Ad-hoc manual deployment is done by copying files and executing shell commands  
Level 2 - Automated new deployment on a clean server in the most common configuration  
Level 3 - Automated new deployment on any server, including cleanup and pre-requisites install / setup on the most common configuration  
Level 4 - Automated deployment on any environment in any supported configuration. Short downtime is accesptable  
Level 5 - No downtime deployments. Automatic rollback on failures. Configurable deployment strategy - ex. blue / green; canary; A/B rollout; etc.  

##### Monitoring
Score: 5  
Max Score: 5  
Description:  
Level 1 - No measurements are done  
Level 2 - Some metrics exist as read-only on a system  
Level 3 - Detailed metrics are available for each production system, including uptime, response time, liveliness, dropped requests, errors, current load  
Level 4 - Pro-active notifications from the metrics are sent appropriately  
Level 5 - Alerts are handled by a system that uses correlation and noise reduction  

##### Runtime
Score: 5  
Max Score: 5  
Description:  
Level 1 - No runtime automation  
Level 2 - Automated health-checks with notifications on issues  
Level 3 - High-availability - deployment uses a load balancer or other tools to assure high-availability if a service goes down and automatically switch to the backup service  
Level 4 - Automated horizontal scalling - automatically add or remove services as needed, based on load and service liveliness. Keep compute costs down automatically  
Level 5 - A/B testing and rolling updates are available  


### Product
Score: 5

##### Logging
Score: 3  
Max Score: 3  
Description:  
Level 1 - Logs are written on the disk per service  
Level 2 - Log rotation and archiving is available  
Level 3 - Centralized logging system is available with easy to search interface  


##### Multitenancy
Score: 5  
Max Score: 5  
Description:  
Level 1 - Multitenancy is not supported  
Level 2 - Multitenancy is supported partially - some of the services can handle multiple tenants, while other cannot  
Level 3 - Multitenancy is fully supported  
Level 4 - New tenants can be onboarded fully automatically  
Level 5 - Restrictions can be applied per tenant basis - ex. resource usage  

##### Request Traceability
Score: 2  
Max Score: 2  
Description:  
Level 1 - No request traceability  
Level 2 - Each request is assigned an UID, which is passed along and logged by each services that handles that particular request. The UID is passed to the client as well. Engineers can search a centralized logging system for a request UID and get all logs from all services, related to the request  

##### Service Discovery
Score: 2  
Max Score: 2  
Description:  
Level 1 - Manual process done by hardcoded configuration what is the address of each service  
Level 2 - Centralized service registration and discovery system is avilable  

##### Feature Flags
Score: 3  
Max Score: 3  
Description:  
Level 1 - No such functionality available  
Level 2 - Feature flags are available as a configuration in the product  
Level 3 - Feature flags are available in a centralized service  

##### Usage Analytics
Score: 3  
Max Score: 3  
Description:  
Level 1 - No analytics available  
Level 2 - Simply usage analytics available - ex. how many time a particular page was loaded  
Level 3 - Detailed custom usage analytics available - ex. ability to see detailed interactions with the application and filter the data  


### Technology
Score: 5

##### Tooling Versions
Score: 3  
Max Score: 3  
Description:  
Do we use an up to date version of our tools? Tools are considered anything that we use to write or run the application:  
Level 1 - Using at least 1 deprecated tool version  
Level 2 - Using some latest and some older versions, but no deprecated ones  
Level 3 - Using only latest stable versions of all tools. All security patches of our tools and dependencies are applied quickly  


##### OS Compatibility
Score: 3  
Max Score: 3  
Description:  
Can we run our application on different OS:  
Level 1 - Runs on only 1 OS  
Level 2 - Can be run on multiple OSs, but has some limitations, or requires a lot of additional configuration and support  
Level 3 - Can be run on any popular OS as is, or with minimal configuration  


##### Cloud Compatibility
Score: 3  
Max Score: 3  
Description:  
Can we run our application on different Cloud providers:  
Level 1 - Runs on only 1 Cloud provider  
Level 2 - Can be run on different cloud providers, but has some limitations, or requires a lot of additional configuration and support  
Level 3 - Can be run on any popular cloud as is, or with minimal configuration  

##### Horizontal Scalability
Score: 5  
Max Score: 5  
Description:  
Can the application be scalled horizontally:  
Level 1 - No horizontal scallability  
Level 2 - Horizontal scallability is available, but requires manual setup and work is not load balanced  
Level 3 - Horizontal scalability is done fully automatically with good load distribution  
Level 4 - Automated scalling up and down, depending on the load  

