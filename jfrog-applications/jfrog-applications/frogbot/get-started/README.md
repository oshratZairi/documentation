# Get Started

JFrog Frogbot is a Git bot that scans your git repositories for security vulnerabilities.

1. It scans pull requests immediately after they are opened but before they are merged. This process notifies you if the pull request is about to introduce new vulnerabilities to your code. This unique capability ensures that the code is scanned and can be fixed even before vulnerabilities are introduced into the codebase.
2. It scans the Git repository periodically and creates pull requests with fixes for vulnerabilities that are detected.

It supports the following Git providers:

* Azure Repos
* Bitbucket Server
* GitHub
* GitLab

#### Why use JFrog Frogbot?

* **Software Composition Analysis (SCA)**: Scan your project dependencies for security issues. For selected security issues, get leverage-enhanced CVE data that is provided by our JFrog Security Research team. Frogbot uses JFrog's vast vulnerabilities database, to which we continuously add new component vulnerability data. Also included is VulnDB, the industry's most comprehensive security database, to further extend the range of vulnerabilities detected and fixed by Frogbot.
* **Vulnerability Contextual Analysis**: This feature uses the code context to eliminate false positive reports on vulnerable dependencies that are not applicable to the code. Vulnerability Contextual Analysis is currently supported for Python and JavaScript code.
* **Secrets Detection**: Detect any secrets left exposed inside the code. to stop any accidental leak of internal tokens or credentials.
* **Infrastructure as Code scans (IaC)**: Scan Infrastructure as Code (Terraform) files for early detection of cloud and infrastructure misconfigurations.

> _**NOTE:**_ **Vulnerability Contextual Analysis**, **Secrets Detection** and **Infrastructure as Code scans** require the [JFrog Advanced Security Package](https://jfrog.com/xray/).

#### What's needed for the setup?

* Frogbot uses a JFrog environment to scan your Git repositories. If you don't have a JFrog environment, you can set up one for free, and use it with no limits.
* Frogbot also requires a runtime environment for the scanning. The following environments are supported:
  * GitHub Actions
  * Jenkins
  * JFrog Pipelines
  * GitLab Pipelines
  * Azure Pipelines