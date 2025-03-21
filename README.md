# Penetration Test Report for Penetration Testing and Ethical Hacking Exam

## Overview

This repository contains the detailed **Penetration Test Report** for the **Penetration Testing and Ethical Hacking Exam** network. The goal of this penetration test was to evaluate the security of the internal network, identify vulnerabilities, and exploit flaws within the **calipendula.loc** domain and the **finance.calipendula.loc** subdomain.

During the test, several critical vulnerabilities were discovered, including **Remote Code Execution**, **Token Impersonation**, and **Incorrect Permission Assignment for Critical Resources**. These issues allowed the tester to compromise internal systems and gain administrative access, highlighting the need for improved security measures.

This test was conducted in collaboration with my team, and together, we simulated attacks to assess the security of the network and identify areas that require attention and remediation.

## Objective

The objective of this assessment was to perform an **internal penetration test** targeting the Penetration Testing and Ethical Hacking Exam network. The test focused on simulating attacks that a potential hacker might use to infiltrate the system, with the intention of evaluating security weaknesses and reporting findings for remediation.

## Key Findings

- **Remote Code Execution (RCE)**: A critical vulnerability allowing attackers to execute arbitrary code remotely.
- **Token Impersonification**: A weakness that allowed impersonation of user tokens, gaining unauthorized access.
- **Incorrect Permission Assignment**: Critical resources were improperly secured, enabling unauthorized users to access sensitive data.

## Systems Exploited

During the penetration test, the following systems were compromised:

- **192.168.72.3** (CAVA)
- **192.168.72.4** (SAVA)
- **192.168.72.5** (PTEH-DEBIAN)
- **192.168.72.7** (DC1)
- **192.168.72.8** (srvapp)
- **192.168.72.9** (sanseverino)

Access was gained due to **outdated patches** and **poor security configurations**, leading to both local and domain administrator privileges.

## Test Methodology

The internal penetration test was performed by exploiting weaknesses in network security, focusing on misconfigurations, outdated software, and insecure permissions. The test followed the steps of:

1. **Reconnaissance**: Scanning and identifying live systems and services.
2. **Vulnerability Identification**: Searching for known vulnerabilities and misconfigurations.
3. **Exploitation**: Attempting to exploit the discovered vulnerabilities to gain access.
4. **Privilege Escalation**: Attempting to escalate privileges to gain administrative control.
5. **Reporting**: Documenting the findings and providing recommendations for mitigation.

## Summary of Tools Used

The following tools were utilized during the penetration test:

- **Nmap**: Used for network scanning and identifying open ports and services on the target machines.
- **Metasploit**: A framework used for exploiting vulnerabilities, including Remote Code Execution (RCE) and other known exploits.
- **Burp Suite**: Used for web vulnerability scanning and identifying flaws such as Token Impersonation.
- **Nikto**: A web server scanner used to identify potential security vulnerabilities in web applications running on the target servers.
- **Netcat**: Used for creating reverse shells and establishing network connections for exploitation.
- **John the Ripper**: A password cracking tool used to test the strength of password hashes found during the test.
- **Wireshark**: A network protocol analyzer used to capture and analyze network traffic to look for vulnerabilities in data transmissions.
- **Hydra**: Used for brute-force password cracking on services with weak authentication.

## Remediation Recommendations

- **Patch Management**: Apply critical patches to outdated systems to mitigate known vulnerabilities.
- **Access Control**: Review and correct permission assignments for sensitive resources.
- **Token Management**: Implement stronger token validation and authentication methods to prevent impersonation.
- **Security Hardening**: Follow best practices for securing servers and network resources against unauthorized access.

## Conclusion

The test revealed significant vulnerabilities in the internal network, many of which could have been exploited by attackers to gain unauthorized access and control over the systems. Immediate attention and remediation of the identified issues are necessary to improve the security posture of the organization.

This report reflects the collaborative efforts of **my team and I** in identifying and addressing key security flaws in the network infrastructure.

