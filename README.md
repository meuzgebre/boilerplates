# Website Pentesting Checklist

Website pentesting involves evaluating the security posture of a website or web application to identify vulnerabilities that could be exploited by an attacker. This checklist provides an extensive and systematic guide for conducting a comprehensive website pentest. From pre-engagement preparations and information gathering to scrutinizing configuration management, authentication, input validation, and cryptographic measures, it provides a methodical approach to assessing web security.

### Pre-engagement

 - [ ] Define the scope of the engagement.
 - [ ] Obtain permission from the appropriate parties.
 - [ ] Establish communication channels and schedules.
 - [ ] Set rules of engagement.
 - [ ] Create and sign a Non-Disclosure Agreement (NDA).

### Information Gathering

 - [ ] Identify the website technologies.
 - [ ] Enumerate subdomains and web directories.
 - [ ] Identify the web server and its version.
 - [ ] Identify the operating system and its version.
 - [ ] Identify the programming language and framework used.
 - [ ] Identify the database and its version.
 - [ ] Enumerate content management system (CMS) plugins and their versions.
 - [ ] Identify the presence of content distribution networks (CDNs).
 - [ ] Determine the content management system (CMS) configuration (e.g., default admin path).
 - [ ] Enumerate available web services or APIs and their endpoints.
 - [ ] Identify content contributors, authors, or administrators.
 - [ ] Review robots.txt and sitemap.xml files for exposed directories.
 - [ ] Enumerate any exposed backup or old website versions.
 - [ ] Identify the use of content versioning systems (e.g., Git repositories).
 - [ ] Perform WHOIS lookup for information on the domain owner.
 - [ ] Identify the website's social media profiles and associated users.
 - [ ] Enumerate email addresses related to the domain.
 - [ ] Discover affiliations, partnerships, or parent/child domain relationships.
 - [ ] Enumerate any web forms used for data collection.
 - [ ] Identify any exposed login portals or user registration pages.
 - [ ] Enumerate external links to other websites, including potential vulnerabilities.
 - [ ] Identify HTTP security headers and configurations (e.g., Content Security Policy, X-Frame-Options).
 - [ ] Enumerate available RSS or Atom feeds.
 - [ ] Identify third-party tracking scripts, widgets, or analytics services.
 - [ ] Review HTTP access and error logs for useful information.
 - [ ] Enumerate any published security advisories or bug bounty programs.
 - [ ] Identify the existence of open redirect vulnerabilities.
 - [ ] Enumerate different language versions of the website.
 - [ ] Review DNS records for SPF, DMARC, and DKIM configurations.
 - [ ] Check for subdomains of subdomains, especially for cloud services (e.g., sub-subdomains).
 - [ ] Identify website owner and administrator contact information.
 - [ ] Enumerate web application frameworks and libraries in use.
 - [ ] Identify the presence of code repositories on platforms like GitHub.
 - [ ] Review public code repositories for sensitive information, credentials, or hardcoded keys.
 - [ ] Enumerate subdomains used for testing or development.
 - [ ] Identify any email servers and their versions.
 - [ ] Enumerate the use of server-side scripting languages.
 - [ ] Identify the presence of web application firewalls (WAFs) or other security solutions.
 - [ ] Enumerate error messages or stack traces that may reveal sensitive information.
 - [ ] Identify any file or media upload functionalities.
 - [ ] Enumerate any interactive elements, such as search functionality or chat widgets.
 - [ ] Review privacy policies, terms of service, and copyright information for details.

### Configuration Management

 - [ ] Test for HTTP methods and headers.
 - [ ] Test for insecure HTTP methods.
 - [ ] Test for directory traversal vulnerabilities.
 - [ ] Test for open ports and services.
 - [ ] Test for default files and directories.
 - [ ] Test for weak passwords and password policies.
 - [ ] Test for user enumeration vulnerabilities.
 - [ ] Test for insecure storage of sensitive information.
 - [ ] Test for HTTP security headers (eg, Content Security Policy, X-Content-Type-Options).
 - [ ] Test for Cross-Origin Resource Sharing (CORS) misconfigurations.
 - [ ] Test for security-related HTTP response headers (eg, Strict-Transport-Security).
 - [ ] Test for HTTP security options like HTTP Public Key Pinning (HPKP).
 - [ ] Review Secure Sockets Layer (SSL) or Transport Layer Security (TLS) configurations.
 - [ ] Test for security misconfigurations in HTTP methods (eg, HTTP PUT, DELETE).
 - [ ] Review Content Management System (CMS) configurations for security settings.
 - [ ] Test for security misconfigurations in web server settings (eg, Apache, Nginx).
 - [ ] Test for weak password policies and enforcement.
 - [ ] Identify password complexity requirements and policies.
 - [ ] Test for password reuse prevention mechanisms.
 - [ ] Test for password aging and expiration policies.
 - [ ] Review the handling of failed login attempts (account lockout, delays).
 - [ ] Test for password storage mechanisms (hashing and salting).
 - [ ] Identify the use of single sign-on (SSO) solutions.
 - [ ] Enumerate default files and directories (eg, admin, login, backup).
 - [ ] Identify error handling and debugging information exposure.
 - [ ] Test for sensitive information disclosure in error messages.
 - [ ] Test for security misconfigurations in database settings (eg, MySQL, PostgreSQL).
 - [ ] Identify publicly accessible configuration files (eg, env, configphp).
 - [ ] Test for open ports and services outside standard HTTP/HTTPS.
 - [ ] Identify services like SSH, RDP, FTP, and their security configurations.
 - [ ] Enumerate open network ports and identify their applications.
 - [ ] Test for default service accounts and their associated privileges.
 - [ ] Review server default configurations for potential vulnerabilities.
 - [ ] Test for security misconfigurations related to server hardening.
 - [ ] Identify the presence of default files or directories (eg, robotstxt, git).
 - [ ] Test for misconfigured access control on sensitive files and directories.
 - [ ] Test for security misconfigurations related to file uploads.
 - [ ] Identify potential web services or APIs not properly secured.
 - [ ] Test for XML External Entity (XXE) vulnerabilities.
 - [ ] Enumerate cloud services, containers, or serverless functions.
 - [ ] Review configurations of load balancers, firewalls, and security groups.
 - [ ] Test for the presence of backdoors or hidden scripts.
 - [ ] Enumerate externally accessible configuration files (eg, webconfig, htaccess).
 - [ ] Test for environment-specific security settings (dev, staging, production).
 - [ ] Identify backup and archive retention policies and configurations.
 - [ ] Review security headers related to frame options (eg, X-Frame-Options).
 - [ ] Test for security misconfigurations in web application frameworks and libraries.

### Authentication and Authorization

 - [ ] Test for weak authentication mechanisms.
 - [ ] Test for session fixation vulnerabilities.
 - [ ] Test for insecure password recovery mechanisms.
 - [ ] Test for insecure session management.
 - [ ] Test for insecure password policies.
 - [ ] Test for privilege escalation vulnerabilities.
 - [ ] Test for weak password storage mechanisms (eg, plaintext, unsalted hashes).
 - [ ] Review password storage policies and compliance with best practices.
 - [ ] Test for brute force and account lockout mechanisms.
 - [ ] Identify password reset and account recovery processes.
 - [ ] Test for password reset token security and randomness.
 - [ ] Review multi-factor authentication (MFA) implementation.
 - [ ] Test for MFA bypass or token leakage vulnerabilities.
 - [ ] Test for session management issues (eg, session fixation, hijacking).
 - [ ] Identify insecure or missing session timeout settings.
 - [ ] Review password change mechanisms and requirements.
 - [ ] Test for insecure or weak password recovery questions.
 - [ ] Test for privilege escalation within user roles.
 - [ ] Review authorization controls for access to sensitive resources.
 - [ ] Test for direct object reference vulnerabilities.
 - [ ] Identify insecure direct object references.
 - [ ] Review access controls for administrative interfaces.
 - [ ] Test for role-based access control (RBAC) bypass.
 - [ ] Identify unauthorized access to privileged functions.
 - [ ] Test for vertical privilege escalation (user to admin).
 - [ ] Test for horizontal privilege escalation (user to user).
 - [ ] Review security policies for user roles and permissions.
 - [ ] Test for session fixation or session token theft.
 - [ ] Test for account hijacking and unauthorized account access.
 - [ ] Identify security issues with single sign-on (SSO) solutions.
 - [ ] Test for authentication bypass vulnerabilities.
 - [ ] Review the secure transmission of authentication credentials.
 - [ ] Test for security misconfigurations related to OAuth or OpenID Connect.
 - [ ] Identify security issues with passwordless authentication.
 - [ ] Test for vulnerabilities in user registration processes.
 - [ ] Review and test password policies for compliance.
 - [ ] Identify weak or insecure password recovery mechanisms.
 - [ ] Test for insufficient or missing rate limiting on authentication attempts.
 - [ ] Review session fixation protection mechanisms.
 - [ ] Test for security misconfigurations related to tokens and cookies.
 - [ ] Identify issues with single sign-out (SSO) or session termination.

### Input Validation

 - [ ] Test for SQL injection vulnerabilities.
 - [ ] Test for cross-site scripting (XSS) vulnerabilities.
 - [ ] Test for command injection vulnerabilities.
 - [ ] Test for file inclusion vulnerabilities.
 - [ ] Test for buffer overflow vulnerabilities.
 - [ ] Test for input validation vulnerabilities.
 - [ ] Test for LDAP injection vulnerabilities.
 - [ ] Test for NoSQL injection vulnerabilities (if applicable).
 - [ ] Test for XML injection vulnerabilities.
 - [ ] Test for XXE (XML External Entity) injection.
 - [ ] Test for XPath injection vulnerabilities (if applicable).
 - [ ] Test for template injection vulnerabilities.
 - [ ] Test for remote code execution (RCE) via user inputs.
 - [ ] Review and test data serialization mechanisms for security issues.
 - [ ] Test for insecure deserialization vulnerabilities.
 - [ ] Test for HTTP parameter pollution (HPP) vulnerabilities.
 - [ ] Review and test request parameter tampering.
 - [ ] Test for HTML injection and data leakage issues.
 - [ ] Test for server-side request forgery (SSRF) vulnerabilities.
 - [ ] Test for server-side template injection vulnerabilities.
 - [ ] Test for business logic flaws related to input validation.
 - [ ] Test for insecure file upload vulnerabilities.
 - [ ] Review client-side input validation for security misconfigurations.
 - [ ] Test for input validation bypass vulnerabilities.
 - [ ] Test for vulnerabilities in custom input validation logic.
 - [ ] Review the use of regular expressions in input validation.
 - [ ] Test for code injection vulnerabilities via custom input handling.
 - [ ] Test for path traversal vulnerabilities in custom input handling.
 - [ ] Review and test the handling of JSON and XML inputs for security.
 - [ ] Test for input data tampering and manipulation vulnerabilities.
 - [ ] Test for time-based attacks (eg, blind SQL injection).
 - [ ] Test for second-order vulnerabilities (eg, stored XSS).
 - [ ] Review and test for security of client-side validation rules.
 - [ ] Test for authorization bypass via manipulated inputs.
 - [ ] Review and test the security of RESTful API inputs.
 - [ ] Test for object injection vulnerabilities.
 - [ ] Test for CSV injection (if applicable).
 - [ ] Review and test query parameterization for security issues.
 - [ ] Test for session cookie security (eg, cookie tampering).
 - [ ] Test for security misconfigurations in form data handling.

### Cryptography

 - [ ] Test for weak encryption algorithms and keys.
 - [ ] Test for weak key generation algorithms.
 - [ ] Test for weak certificate validation and verification.
 - [ ] Test for weak SSL/TLS configurations.
 - [ ] Test for weak random number generation.
 - [ ] Test for insecure storage of cryptographic keys and passwords.
 - [ ] Test for use of weak or deprecated encryption algorithms.
 - [ ] Test for improper use of cryptography (e.g. encrypting passwords instead of hashing them).
 - [ ] Test for cryptographic side-channel attacks (eg, timing attacks).
 - [ ] Review and test cryptographic key management practices.
 - [ ] Test for proper implementation of cryptographic libraries.
 - [ ] Verify secure key exchange mechanisms (eg, Diffie-Hellman).
 - [ ] Test for cryptographic algorithm downgrade attacks.
 - [ ] Review and test for secure password hashing (eg, bcrypt).
 - [ ] Test for weak or insufficient entropy sources for cryptographic operations.
 - [ ] Verify the use of cryptographic secure random number generators.
 - [ ] Review the protection of private keys and certificates.
 - [ ] Test for cryptographic key and certificate expiration handling.
 - [ ] Verify secure implementation of cryptographic hashing functions.
 - [ ] Test for cryptographic padding oracle vulnerabilities (eg, PKCS#7).
 - [ ] Test for the presence of hardcoded cryptographic keys.
 - [ ] Verify secure use of cryptographic salts (if applicable).
 - [ ] Test for cryptographic downgrade attacks in SSL/TLS protocols.
 - [ ] Review and test the use of secure cryptographic modes of operation.
 - [ ] Verify the integrity of cryptographic signatures and certificates.
 - [ ] Test for secure cryptographic configuration in databases.
 - [ ] Test for encryption key rotation and rekeying procedures.
 - [ ] Verify secure cryptographic storage of sensitive data.
 - [ ] Test for the proper generation and handling of Initialization Vectors (IVs).
 - [ ] Test for the presence of unused or deprecated cryptographic components.
 - [ ] Review the security of public key infrastructure (PKI) implementations.
 - [ ] Verify that cryptographic libraries and modules are up-to-date.
 - [ ] Test for cryptographic weaknesses in custom encryption methods.
 - [ ] Review and test secure cryptographic key escrow and recovery procedures.
 - [ ] Verify the use of secure authentication tokens for cryptographic operations.
 - [ ] Test for cryptographic protocol downgrade attacks (eg, POODLE).
 - [ ] Review and test secure SSL/TLS ciphersuite configurations.
 - [ ] Verify secure implementation of hardware security modules (HSMs).
 - [ ] Test for secure encryption in transit and at rest.
 - [ ] Review the use of secure random initialization vectors (IVs).
 - [ ] Verify secure handling of cryptographic initialization vectors.
 - [ ] Test for cryptographic export control and compliance.
 - [ ] Review and test the secure handling of cryptographic exceptions.
 - [ ] Verify secure use of cryptographic time-based mechanisms.
 - [ ] Test for cryptographic padding oracle vulnerabilities (eg, Bleichenbacher's attack).
 - [ ] Verify secure generation and storage of encryption keys in mobile applications.

### Network Configuration

- [ ] Test for network misconfigurations.
- [ ] Test for firewall vulnerabilities.
- [ ] Test for DNS server vulnerabilities.
- [ ] Test for network eavesdropping vulnerabilities.
- [ ] Test for wireless network vulnerabilities.
- [ ] Test for VPN vulnerabilities.
- [ ] Test for insecure network protocols (e.g., Telnet, FTP, SMB) and recommend secure alternatives.
- [ ] Review and test network segmentation and isolation to prevent lateral movement.
- [ ] Test for insecure Wireless Access Points (WAPs) and suggest security improvements.
- [ ] Review and test network monitoring and intrusion detection systems (IDS/IPS).
- [ ] Verify the use of secure VPN (Virtual Private Network) configurations.
- [ ] Test for rogue devices connected to the network.
- [ ] Test for weak or default network device credentials.
- [ ] Review the use of secure network access controls and segmentation.
- [ ] Test for broadcast and multicast network vulnerabilities.
- [ ] Verify the implementation of secure network routing and switching.
- [ ] Test for vulnerabilities in Software-Defined Networking (SDN) implementations.
- [ ] Test for insecure Network Time Protocol (NTP) configurations.
- [ ] Review and test network device logging and alerting.
- [ ] Test for weaknesses in network address assignment (DHCP).
- [ ] Verify secure network traffic encryption (e.g., IPsec, SSL/TLS).
- [ ] Test for insecure IPv6 configurations.
- [ ] Test for network traffic interception and sniffing vulnerabilities.
- [ ] Review and test network security policies and procedures.
- [ ] Test for weak network device security configurations.
- [ ] Verify the use of secure network device management interfaces.
- [ ] Test for DNS cache poisoning and spoofing attacks.
- [ ] Review and test the security of mobile device connections.
- [ ] Test for vulnerabilities in network security appliances (e.g., firewalls, IDS/IPS).
- [ ] Test for unauthorized devices connected to network ports (e.g., MAC spoofing).
- [ ] Verify the use of secure network device authentication and authorization.
- [ ] Test for vulnerabilities in network traffic filtering and ACLs.
- [ ] Review the use of secure network segmentation with VLANs.
- [ ] Test for vulnerabilities in Network Attached Storage (NAS) devices.
- [ ] Test for weaknesses in load balancer and reverse proxy configurations.
- [ ] Verify the use of secure wireless security protocols (e.g., WPA3).
- [ ] Test for vulnerabilities in network isolation and zoning.
- [ ] Test for weaknesses in virtual network environments (e.g., VM escape).
- [ ] Review and test the security of remote network access solutions (e.g., RDP, SSH).
- [ ] Verify secure network traffic logging and analysis.
- [ ] Test for network misconfigurations that may lead to DoS attacks.
- [ ] Test for IPv6 transition technologies security.
- [ ] Review and test network access control policies.
- [ ] Verify the security of network security policies and rule sets.
- [ ] Test for vulnerabilities in network services (e.g., DNS, DHCP, LDAP).
- [ ] Review and test network security patch management.
- [ ] Test for vulnerabilities in network communication protocols (e.g., BGP, SNMP).

### Web Application Vulnerabilities

- [ ] Test for injection vulnerabilities (SQL, XSS, etc.).
- [ ] Test for broken authentication and session management.
- [ ] Test for security misconfigurations.
- [ ] Test for sensitive data exposure.
- [ ] Test for insufficient logging and monitoring.
- [ ] Test for insecure third-party integrations.
- [ ] Test for file upload vulnerabilities.
- [ ] Test for access control vulnerabilities.
- [ ] Test for server-side request forgery (SSRF) vulnerabilities.
- [ ] Test for Cross-Site Request Forgery (CSRF) vulnerabilities.
- [ ] Test for Cross-Site Script Inclusion (XSSI) vulnerabilities.
- [ ] Test for XML External Entity (XXE) vulnerabilities.
- [ ] Test for Server-Side Template Injection (SSTI) vulnerabilities.
- [ ] Test for HTTP Request Smuggling vulnerabilities.
- [ ] Test for Clickjacking vulnerabilities.
- [ ] Test for Remote File Inclusion (RFI) vulnerabilities.
- [ ] Test for Local File Inclusion (LFI) vulnerabilities.
- [ ] Test for Server-Side Template Injection (SSTI) vulnerabilities.
- [ ] Test for insecure data storage in client-side storage (e.g., localStorage).
- [ ] Test for Insecure Direct Object References (IDOR) vulnerabilities.
- [ ] Test for HTTP Parameter Pollution (HPP) vulnerabilities.
- [ ] Test for XML Injection (XIN) vulnerabilities.
- [ ] Test for JSON Injection (JSONi) vulnerabilities.
- [ ] Test for Host Header Injection vulnerabilities.
- [ ] Test for HTTP Desync attacks.
- [ ] Test for Server-Side Request Forgery (SSRF) vulnerabilities.
- [ ] Test for Remote Code Execution (RCE) vulnerabilities.
- [ ] Test for Command Injection (OS Command, OS Shell) vulnerabilities.
- [ ] Test for Business Logic Flaws (e.g., logic bypass, authorization bypass).
- [ ] Test for insecure password reset processes.
- [ ] Test for vulnerabilities in session tokens and cookies.
- [ ] Test for API vulnerabilities (e.g., REST, GraphQL).
- [ ] Test for NoSQL Injection vulnerabilities.
- [ ] Test for GraphQL Injection vulnerabilities.
- [ ] Test for WebSockets security vulnerabilities.
- [ ] Test for security misconfigurations in CDN configurations.
- [ ] Test for security misconfigurations in cloud-based services (e.g., AWS, Azure).
- [ ] Test for insecure or incomplete security headers (e.g., CSP, HSTS).
- [ ] Test for DOM-based vulnerabilities.
- [ ] Test for vulnerabilities in web application containers (e.g., Docker).
- [ ] Test for client-side encryption vulnerabilities.
- [ ] Test for vulnerabilities in client-side JavaScript libraries and frameworks.
- [ ] Test for vulnerabilities in Single Sign-On (SSO) solutions.
- [ ] Test for vulnerabilities in multi-factor authentication (MFA) systems.
- [ ] Test for vulnerabilities in password managers.
- [ ] Test for vulnerabilities in web application firewall (WAF) configurations.
- [ ] Test for vulnerabilities in content management systems (CMS).
- [ ] Test for vulnerabilities in web application plugins and extensions.
- [ ] Test for vulnerabilities in microservices architectures.
- [ ] Test for vulnerabilities in API gateways and reverse proxies.
- [ ] Test for vulnerabilities in web application deployment scripts and automation.
- [ ] Test for vulnerabilities in user-generated content (UGC) handling.
- [ ] Test for vulnerabilities in user session management (e.g., tokens, cookies).

### Business Logic Flaws

- [ ] Test for business logic vulnerabilities (such as logic bypasses, authentication bypasses, etc.).
- [ ] Test for insufficient user input validation.
- [ ] Test for input manipulation vulnerabilities.
- [ ] Test for privilege escalation vulnerabilities.
- [ ] Test for data leakage vulnerabilities.
- [ ] Test for insufficient transactional security.
- [ ] Test for race conditions and concurrency issues.
- [ ] Test for business process flaws that can be abused by attackers.
- [ ] Test for discrepancies between client-side and server-side validation.
- [ ] Test for insecure direct object references (IDOR).
- [ ] Test for differences in behavior based on user roles.
- [ ] Test for discrepancies between the application's intended workflow and the actual behavior.
- [ ] Test for flaws in multi-step processes, such as transaction authorization.
- [ ] Test for flaws in access control mechanisms that can lead to privilege escalation.
- [ ] Test for bypassing payment processes and other financial operations.
- [ ] Test for issues in user and data session management, especially related to concurrency.
- [ ] Test for data leakage in error messages or logs.
- [ ] Test for issues in security decisions based on untrusted data (e.g., client-side trust).

### Web Services/API Security
- [ ] Test for OAuth 2.0 and OpenID Connect vulnerabilities in authentication services.
- [ ] Check for API rate limiting and access control mechanisms.
- [ ] Review API response and error handling for information leakage.
- [ ] Assess the presence of GraphQL endpoints and potential security issues.

### Content Management System (CMS) Security

- [ ] Check for outdated plugins, themes, and core components.
- [ ] Evaluate the security of the CMS's admin interface.
- [ ] Assess the effectiveness of role-based permissions in the CMS.
- [ ] Check for username enumerations.

### Reporting

- [ ] Provide detailed report of vulnerabilities found.
- [ ] Prioritize vulnerabilities based on their impact and likelihood of exploitation.
- [ ] Provide remediation recommendations for each vulnerability.
- [ ] Provide proof-of-concept exploits for critical vulnerabilities (with permission).
- [ ] Schedule follow-up testing to verify that identified vulnerabilities have been remediated.
