# Case Study:  Defender for Endpoint Deployment

## Overview:
</br>

<img align="left" alt="Portfolio Logo" width="400px" src="https://emsroute.com/wp-content/uploads/2022/01/defendelogo.png" />
</br>

- **Position**:  Information Security Analyst, Subject Matter Expert (SME)
- **Timeframe**:  Six months
- **Objective**:  Successfully deploy Microsoft Defender for Endpoint (MDE) as a prerequisite for implementing Microsoft Purview Data Loss Prevention (DLP).  
</br>
</br>
</br>


## Background
- **Context**:  As part of the Security Engineering and Architecture Team within the Information Security Office (ISO), we aimed to enhance our security posture through effective DLP solutions.  
- **Stakeholders**:  Involved directors, the Chief Information Security Officer (CISO), Chief Technology Officer (CTO), and product support teams. 

## Problem Statement
- The organization needed a robust DLP solution, and the existing contract with Symantec DLP was nearing its end.  The decision was made to transition to Microsoft Purview, leveraging our ongoing Microsoft contract for better support and pricing.  

## Approach
- **Research and Analysis**:  Conducted thorough research using Microsoft Learn and completed various trainings to become familiar with MDE functionalities and requirements.
- **Methodology**:  Collaborated with product support teams to formulate a comprehensive deployment plan for MDE.
- **Tools and Technologies**:  Utilized Microsoft Defender for Endpoint, BigFix for deployment, MDE and CrowdStrike for EDR Exclusion policies, PowerShell scripts for testing and deployment, and MDE Dashboards and KQL for analysis.  

## Implementation
**Steps Taken**:
1. Created a Group Policy deployment script for Windows 10 & 11 devices and shared it with the product team to push fleet-wide via BigFix.  
2.	Enrolled in MDE's EDR Exclusion feature, allowing the our team to create EDR exclusion policies to ensure proper implementation.   
3.	Deployed MDE while ensuring it operated in passive mode to prevent conflicts, keeping CrowdStrike as our primary EDR solution.  
4.	Observed performance issues on endpoints during rollout, particularly with the simultaneous deployment of Tanium for device management, necessitating further analysis.
5.	Established exclusion policies to mitigate conflicting scanning issues that initially caused performance bottlenecks.

**Challenges Faced**:  Discovered that MDE required careful management alongside other security solutions to avoid performance impacts.  

## Results
- **Outcomes**:  Successfully deployed MDE alongside existing security tools, leveraging vulnerability data to enhance security posture.  
- **Impact**:  Created a process to monitor devices for Zscaler installation and initiated a monthly vulnerability report for tracking software updates and configurations.  

## Lessons Learned
- Recognized the importance of thorough testing and collaboration among security tools to avoid conflicts.  
- Gained valuable insights into managing multiple security solutions effectively.  

## Conclusion
- The deployment of Microsoft Defender for Endpoint not only fulfilled the prerequisite for Microsoft Purview DLP but also provided additional insights to bolster the organization's overall security posture.  

### References
- [Set up Microsoft Defender for Endpoint deployment](https://learn.microsoft.com/en-us/defender-endpoint/production-deployment)
- [Microsoft Defender Antivirus compatibility with other security products](https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-antivirus-compatibility)
- [Reference: Endpoint security exclusions](https://help.tanium.com/bundle/ug_client_cloud/page/client/security_exclusions.html)
- [Exclusions overview](https://learn.microsoft.com/en-us/defender-endpoint/navigate-defender-endpoint-antivirus-exclusions)
- [Get started with endpoint data loss prevention](https://learn.microsoft.com/en-us/purview/endpoint-dlp-getting-started)
