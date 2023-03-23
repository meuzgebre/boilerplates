# Website Pentesting Checklist

Website pentesting involves evaluating the security posture of a website or web application to identify vulnerabilities that could be exploited by an attacker. This checklist provides a comprehensive guide for conducting a website pentest.

### Pre-engagement

 - [ ] Define the scope of the engagement
 - [ ] Obtain permission from the appropriate parties
 - [ ] Establish communication channels and schedules
 - [ ] Set rules of engagement
 - [ ] Create and sign a Non-Disclosure Agreement (NDA)

### Information Gathering

 - [ ] Identify the website technologies
 - [ ] Enumerate subdomains and web directories
 - [ ] Identify the web server and its version
 - [ ] Identify the operating system and its version
 - [ ] Identify the programming language and framework used
 - [ ] Identify the database and its version

### Configuration Management

 - [ ] Test for HTTP methods and headers
 - [ ] Test for insecure HTTP methods
 - [ ] Test for directory traversal vulnerabilities
 - [ ] Test for open ports and services
 - [ ] Test for default files and directories
 - [ ] Test for weak passwords and password policies
 - [ ] Test for user enumeration vulnerabilities
 - [ ] Test for insecure storage of sensitive information

### Authentication and Authorization

 - [ ] Test for weak authentication mechanisms
 - [ ] Test for session fixation vulnerabilities
 - [ ] Test for insecure password recovery mechanisms
 - [ ] Test for insecure session management
 - [ ] Test for insecure password policies
 - [ ] Test for privilege escalation vulnerabilities

### Input Validation

 - [ ] Test for SQL injection vulnerabilities
 - [ ] Test for cross-site scripting (XSS) vulnerabilities
 - [ ] Test for command injection vulnerabilities
 - [ ] Test for file inclusion vulnerabilities
 - [ ] Test for buffer overflow vulnerabilities
 - [ ] Test for input validation vulnerabilities

### Cryptography

 - [ ] Test for weak encryption algorithms and keys
 - [ ] Test for weak key generation algorithms
 - [ ] Test for weak certificate validation and verification
 - [ ] Test for weak SSL/TLS configurations
 - [ ] Test for weak random number generation
 - [ ] Test for insecure storage of cryptographic keys and passwords
 - [ ] Test for use of weak or deprecated encryption algorithms
 - [ ] Test for improper use of cryptography (e.g. encrypting passwords instead of hashing them)

### Network Configuration

- [ ] Test for network misconfigurations
- [ ] Test for firewall vulnerabilities
- [ ] Test for DNS server vulnerabilities
- [ ] Test for network eavesdropping vulnerabilities
- [ ] Test for wireless network vulnerabilities
- [ ] Test for VPN vulnerabilities

### Web Application Vulnerabilities

- [ ] Test for injection vulnerabilities (SQL, XSS, etc.)
- [ ] Test for broken authentication and session management
- [ ] Test for security misconfigurations
- [ ] Test for sensitive data exposure
- [ ] Test for insufficient logging and monitoring
- [ ] Test for insecure third-party integrations
- [ ] Test for file upload vulnerabilities
- [ ] Test for access control vulnerabilities
- [ ] Test for server-side request forgery (SSRF) vulnerabilities

### Business Logic Flaws

- [ ] Test for business logic vulnerabilities (such as logic bypasses, authentication bypasses, etc.)
- [ ] Test for insufficient user input validation
- [ ] Test for input manipulation vulnerabilities
- [ ] Test for privilege escalation vulnerabilities
- [ ] Test for data leakage vulnerabilities
- [ ] Test for insufficient transactional security

### Reporting

- [ ] Provide detailed report of vulnerabilities found
- [ ] Prioritize vulnerabilities based on their impact and likelihood of exploitation
- [ ] Provide remediation recommendations for each vulnerability
- [ ] Provide proof-of-concept exploits for critical vulnerabilities (with permission)
- [ ] Schedule follow-up testing to verify that identified vulnerabilities have been remediated.
