# July 2025 Intern Phishing Engagement Report

## Executive Summary 

In July 2025, alongside another intern, I engaged in the planning and execution of a simulated phishing attack as a captone project for our summer internship. The target group consisted of the 2025 Summer Interns, totaling 56 emails sent. This was a credential harvesting attack, with the email disguised to appear as a mid-internship check-in form sent out by an internal recruiter, requiring a SharePoint login to view. Of the 56 emails sent, 48 individuals read the email, 24 clicked the link, and 19 supplied credentials, resulting in a 34% total compromise rate. With our mentor providing loose guidelines, we independently conducted OSINT and reconnaissance, crafted and executed the phishing email, and later provided explanations and training sessions to the participants to enhance their awareness and skills.

## Introduction

With 91% of breaches beginning with a phishing-related compromise, it is imperative for organizations to regularly conduct simulated attacks to ensure employees are educated on detecting and reporting phishing emails. During my summer internship in the Threat & Vulnerability Management (TVM) team, I collaborated with a fellow intern to execute a phishing exercise targeting the 2025 Summer Intern group. Our mentor established two essential criteria: the attack must aim at harvesting credentials, and we must demonstrate how an attacker would realistically identify our impersonation target.

Allowed significant autonomy in designing and executing the engagement, we conducted thorough OSINT and reconnaissance using platforms like LinkedIn, which led us to target impersonating a recruiter. After developing and refining several drafts of the phishing email over a week, we launched the attack on a Monday morning and concluded it by Wednesday. Following the exercise, we distributed communications that detailed the simulated scenario, highlighted Indicators of Compromise (IoCs) the interns should have noted, and provided training for those who were compromised.

## Scope

### Target Group

The focus of this exercise was on the 2025 Summer Intern cohort, comprising 52 interns and an additional 4 full-time employees who held responsibilities related to the interns, totaling 56 targets. Interns were selected due to their generally infrequent involvement in key business operations and increased susceptibility to phishing attempts. As this was a project-based learning exercise, our target group was chosen for us beforehand as a requirement. 

### Goals

The primary goal of this phishing exercise was to afford us hands-on experience in the planning and execution of a phishing campaign as a capstone project for our internship. We were given minimal guidance beyond set requirements, allowing us to function independently and enhance our learning through experience. A secondary goal was to evaluate the interns' ability to recognize and report phishing attempts and to facilitate training and education typically associated with such engagements.

## Methodology

### Planning & Preparation

As stated in the Executive Summary, we were provide with 2 guidelines: it must be a credential harvesting attack, and we must be able to demonstrate how an external threat actor would know to impersonate our chosen target. To satisfy these requirements, we turned to OSINT to gather information on potential targets. Using LinkedIn and public email records, we found pictures and posts of the recruiter with the intern group as well as confirmation they had recruited the interns, followed by finding their work email address. We presented this information to our mentor, and were given the green light to proceed. 

Once we had confirmation on our impersonation target, we set to writing the email. Since we needed a credential harvesting attack, we needed some form of login page. We decided that a check-in form from the recruiter would be innoculous enough to slip under the radar. Using standard email formats availabe online combined with samples of the recruiter's own emails and signature, we crafted a targeted email asking recipients to follow a link to a Microsoft form, under a sharepoint link. 

However, there were 3 IoCs present: An 'external' banner, a spoofed email, and a 'SharePointen' link. Recipients were expected to notice the external banner and scrutinize further details. The spoofed email was chosen as we did not have access to an internal email for this exercise, requiring us to swtich two letters in the email address. The 'SharePointen' link was produced using the Microsoft Defender Attack Simulation's toolkit. 

### Execution

Using Microsoft's Attack Simulations, we pre-loaded the attack the week before it went live. This tool allows for a loose structure with custom-loaded segments as needed. Within this tool, we identified the target email distribution list, the spoofed 'from' email, the content of the email, the 'SharePointen' link, as well as the landing page for credential input. We launched the simulation on a Monday at 9am, hoping to catch people in their normal Monday morning workflows. The simulation concluded the following Wednesday at 9am, with a wrap-up email informing recipient that they had been participating in a phishing exercise. 

