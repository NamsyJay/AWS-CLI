## FULL CI/CD PRODUCTION PIPELINE 
This is a Full Production Level Pipeline. This platform will be built from scratch up until time-to-market.

## WORKFLOW
The code will sourced from the Github Repo, and the source code Terraform for creating EKS cluster. 
The Jenkins Pipeline will be started.
Compilation of code will be done to check for syntax errors.
Proceed with the Test cases (this could be written by the Testing Team or the DevOps Team).
Aqua Trivy will be used for vulnerability scanning.
SonarQube used for code quality check.
Maven will be used for building the code.
Nexus Repository is for stroing artifacts.
Docker is used to build an image and this will be kept in a private repository.
The Image will be scanned again with Aqua Trivy.
