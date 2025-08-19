# Vishing Attack Emulation Report

## Executive Summary

During my internship in the summer of 2025, I collaborated with my technical mentor to execute a simulated Vishing (voice phishing) attack targeting our HelpDesk. A threat actor group known as Scattered Spider had successfully 'vished' competitors in our sector, using social engineering tactics to convince HelpDesk employees to transfer Multi-Factor Authentication (MFA) protections to another device. As a proactive measure, we emulated their Tactics, Techniques, and Procedures (TTPs) by impersonating an executive, calling into the HelpDesk, and forwarding an email containing a link, asking for assistance. This link, embedded in an adapted legitimate email from our CEO, redirected to a mock legitimate Single Sign-On (SSO) login page designed for credential capture. Known for repeated targeting within industries, it was crucial to assess our security stance. Fortunately, neither I nor my mentor succeeded in the attacks. The HelpDesk responded appropriately by alerting the correct teams and denying access, demonstrating robust preparation against such threats.

## Introduction

Scattered Spider is a well-known threat actor group, operating across many cyber domains. Of particular note is their inclination towards social engineering attacks using native English speakers. They prey on willingness to help people, exploiting HelpDesk functions such as password resets and MFA resets to gain initial access. This adds a new level of difficulty, requiring us to be doubly sure of who we're working with on the phone even for seemingly mundane interactions. 

## Metholodogy & Execution

### Pretext

To ensure our HelpDesk is prepared for this emerging threat, my mentor and I prepared and executed a vishing attack against our HelpDesk. To emulate Scattered Spider's TTPs, we selected a remote executive as our impersonation target. As this was a real person at our company, we were able to use Microsoft Defender's Attack Simulation toolkit to send emails as if they had come from his legitimate email. This allowed us to test our lines and assess whether the HelpDesk technicians would sufficiently validate any person on the phone, especially before providing credentials. 

### Profile

To be able to impersonate our target effectively, we needed to build a profile. Using OSINT sources such as Facebook, Instagram, LinkedIn, and officialusa.com, we compiled a list of details such as current and previous registered addresses, alternate names, past employers, phone numbers, hobbies and pets. With this information, as well as information available to us internally, we were able to prep a cheat sheet to use during our calls.

### Attack Vector

For the attack vector, we repurposed a legitimate email sent out by our CEO, asking recipients to follow a link to show support for a local legal issue. However, the link in the email had been spoofed to redirect to our malicious company-branded SSO login page. Our intent was to forward the email using Microsoft Defender's Attack Simulation, which would make it appear to the recipient as a legitimate email from the executive. We would keep the technician on the line as we walk them through the email and the SSO sign in, claiming to be attempting to click the link on a mobile device while traveling. In order to truly set the pretext, we used spoofed Google phone numbers from towns near where the excutive lives, as well as employing ambient airport noises in the background. 

