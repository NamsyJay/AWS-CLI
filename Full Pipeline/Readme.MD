## FULL CI/CD PRODUCTION PIPELINE 
This is a Full Production Level Pipeline. This platform will be built from scratch up until time-to-market.

## PROJECT WORKFLOW
- The code will sourced from the Github Repo, and the source code Terraform for creating EKS cluster. 
- The Jenkins Pipeline will be started.
- Compilation of code will be done to check for syntax errors.
- Proceed with the Test cases (this could be written by the Testing Team or the DevOps Team).
- Aqua Trivy will be used for vulnerability scanning.
- SonarQube used for code quality check.
- Maven will be used for building the code.
- Nexus Repository is for stroing artifacts.
- Docker is used to build an image and this will be kept in a private repository.
- Aqua Trivy will scan the image again for vulnerabilities.
- Create and deploy applications on the EKS cluster.
  - secrets will be set up in the K8s cluster so that the Docker registry can access necessary credentials.
- Map domain using Hostinger.
- Monitor the website with Blackbox exporter, which will forward the metrics to Prometheus.
- The metrics will be shared with Grafana for visualisation.

