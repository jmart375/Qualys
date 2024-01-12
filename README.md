# Qualys Assessment 

[Qualys](https://www.qualys.com/) is a cloud-based security and compliance management platform that provides a range of services to help organizations identify, prioritize, and remediate vulnerabilities in their IT infrastructure. It offers a suite of security and compliance solutions that enable businesses to strengthen their cybersecurity posture. Here are some key aspects of Qualys:

1. **Vulnerability Management:**
   - Continuous monitoring and assessment of the security posture.
   - Efficient prioritization and remediation of vulnerabilities.

2. **Policy Compliance:**
   - Ensures compliance with internal security policies and external regulations.
   - Defines and enforces security policies, performs compliance assessments, and generates reports.

3. **Web Application Security:**
   - Identifies and remediates vulnerabilities in web applications.
   - Addresses issues like SQL injection, cross-site scripting (XSS), and other web application vulnerabilities.

4. **Threat Protection:**
   - Real-time detection and response to threats.
   - Leverages threat intelligence and security analytics for proactive risk mitigation.

5. **Continuous Monitoring:**
   - Enables continuous monitoring of the security posture.
   - Provides real-time insights into the security status of assets and systems.

6. **Cloud Security:**
   - Extends capabilities to secure cloud environments.
   - Supports cloud security assessments and provides visibility into the security of cloud assets.

7. **APIs and Automation:**
   - Provides APIs for integration with other security tools.
   - Supports automation of security processes for streamlined management.

8. **Reporting and Analytics:**
   - Offers detailed reports and analytics.
   - Helps organizations understand their security posture, track improvements, and meet reporting requirements.

Qualys is widely used by enterprises and security professionals as a comprehensive solution for managing cybersecurity risks and ensuring compliance with industry standards and regulations. It is known for its scalability, ease of use, and ability to provide a holistic view of an organization's security landscape.


# Part 2 – Insecure Web Servers
1.	“F”
2.	“T” Not Trusted

![image](https://github.com/jmart375/Qualys/assets/91294710/4ea61e7b-a3fc-4244-96e1-4c9d1b44a06f)

Above is a snapshot of the SSL report on https://oakridgemoraine.org/.

Based on the findings, it was determined that the https://oakridgemoraine.org/ server uses the SSL Version 3, an outdated and insecure protocol. The server also supports the RC4 cipher, a type of encryption that is considered to pose many security risks. It was also found that the server contains weak Diffie-Hellman parameters, which can result in security attacks. In terms of how to mitigate these risks, it is recommended that server disable the SSLv3 protocol and employ a more secure protocol such as TLS Version 1.3. As well, disable the RC4 cipher because it is vulnerable to various attacks, and instead opt for a more secure cipher such as an AES. The Diffie-Hellman parameter strength was found to be relatively weak and a way to combat that is to increase the strength of the parameters to a minimum of 2048 bits or more. This will ensure that the key exchange is secured and protected against malicious attacks. All in all, the server ought to consider implementing the recommendations mentioned above because it will make the site more secure and less vulnerable to attacks.

3.	Server of our choice. We chose to go with a Not Trusted

![image](https://github.com/jmart375/Qualys/assets/91294710/89e37ad1-0c4a-482b-a02d-1dfc0bf75323)

	Above is a snapshot of the SSL report on https://madridcard.com/.
Based on the assessment, it was found that the https://madridcard.com/ server supports the SSLv3 protocol and RC4 cipher, both of which are deemed insecure and vulnerable. It was also found that the server does not support forward secrecy. Ways to improve or mitigate this would be to replace SSLv3 with TLSv1.3. This will result in a faster and more secure protocol. Also considering that RC4 is a weak cipher, it is recommended to disable it and choose one that is more secure, such as AES. The third mitigation strategy is to enable forward secrecy. This ensures that even if the most recent key is compromised, a minimal amount of data is exposed. By implementing the suggested mitigation strategies, https://madridcard.com/ server will improve its security and reduce attacks.

