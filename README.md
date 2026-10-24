# CS305-Software-Security
Projects from SNHU CS 305 course

## Project Overview

Artemis Financial was a financial services company that needed to improve the security of its software application. The company wanted to protect sensitive information, secure communications, and reduce vulnerabilities in its existing software. My goal was to review the application for security issues and apply secure coding practices to improve its protection without losing its existing functionality.

## Reflection

### 1. Client and Software Requirements

Artemis Financial was my client for this project. The company needed its software to communicate securely and protect the information it handled. I worked on improving the application's security by configuring HTTPS, creating a digital certificate, implementing a SHA-256 checksum endpoint, and checking the application's dependencies for known vulnerabilities.

### 2. Identifying Vulnerabilities and the Importance of Secure Coding

I did well at using security tools to identify potential vulnerabilities and applying changes to improve the application's security. I used OWASP Dependency-Check to scan the project's dependencies and generate a report. I also configured HTTPS and implemented SHA-256 hashing to demonstrate checksum verification. Secure coding is important because vulnerabilities can expose sensitive information, allow unauthorized access, and damage a company's reputation. Strong software security helps protect customers, maintain trust, reduce the risk of costly incidents, and support the company's long-term success.

### 3. Most Challenging or Helpful Part of the Assessment

The most challenging part of this project was configuring the development environment and getting the dependency scan to run successfully. I encountered issues with the NVD API key, Maven configuration, and certificate setup. Troubleshooting these problems helped me understand how the different tools work together. The most helpful part was seeing how a dependency scan could identify potential security concerns that might not be obvious from reviewing the application code alone.

Another challenging, yet helpful, part of the assessment was to identify and suppress false positives or vulnerabilities that were irrelevant to the program. This took time and effort reading each CPE and CVE, determining if the vulnerabilities matched the descriptions within the files, and to understand if the vulnerability needed to be suppressed. This assignment helped me better evaluate what files need to be suppressed to prevent false positives or if other security measures, like updating to the latest version, need to be considered.

### 4. Adding Layers of Security and Assessing Vulnerabilities

I increased security by configuring HTTPS on port 8443 and using a self-signed certificate for the project. I also implemented a SHA-256 checksum endpoint and used OWASP Dependency-Check to review third-party dependencies for known vulnerabilities. These measures address different aspects of security rather than relying on a single solution. In future projects, I would continue using dependency scanning, code reviews, vulnerability databases, and security testing. I would prioritize findings based on their severity, exploitability, and impact on the application before choosing appropriate mitigation techniques.

### 5. Ensuring Functionality and Security

I tested the application by running it and verifying that its HTTPS endpoints responded as expected. I accessed the `/profile` endpoint over HTTPS and tested the `/hash` endpoint to verify the checksum functionality. I also ran OWASP Dependency-Check and confirmed that it completed successfully, scanned 49 dependencies (28 unique), and generated a report. After making changes, I used these tests and the dependency report to check the application. In future projects, I would also add automated tests and rerun security scans after dependency updates or significant code changes to help identify regressions and newly introduced vulnerabilities.

### 6. Helpful Resources, Tools, and Coding Practices

The most useful tools and resources were Java, Spring Boot, Maven, OWASP Dependency-Check, the National Vulnerability Database (NVD), and the Java `keytool` utility. I used these tools to configure the application, manage its dependencies, create a certificate, and review potential vulnerabilities. I also learned the importance of keeping API keys private, reading error messages carefully, and verifying that security changes do not break existing functionality. These practices will be useful in future programming assignments and professional development work.

### 7. Work to Show Future Employers

I could show future employers the completed Artemis Financial Practices for Secure Software Report, the application code, and the Dependency-Check report. These artifacts demonstrate my ability to configure secure communications, implement a hashing function, use security scanning tools, and troubleshoot development problems. They also show that I understand the importance of evaluating dependencies and documenting security decisions. This project provides an example of applying cybersecurity concepts to a working software application rather than only discussing them in theory.
