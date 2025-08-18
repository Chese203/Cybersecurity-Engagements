# Vishing Attack Emulation Report

## Executive Summary

During my internship in the summer of 2025, I collaborated with my technical mentor to execute a simulated Vishing (voice phishing) attack targeting our HelpDesk. A threat actor group known as Scattered Spider had successfully 'vished' competitors in our sector, using social engineering tactics to convince HelpDesk employees to transfer Multi-Factor Authentication (MFA) protections to another device. As a proactive measure, we emulated their Tactics, Techniques, and Procedures (TTPs) by impersonating an executive, calling into the HelpDesk, and forwarding an email containing a link, asking for assistance. This link, embedded in an adapted legitimate email from our CEO, redirected to a mock legitimate Single Sign-On (SSO) login page designed for credential capture. Known for repeated targeting within industries, it was crucial to assess our security stance. Fortunately, neither I nor my mentor succeeded in the attacks. The HelpDesk responded appropriately by alerting the correct teams and denying access, demonstrating robust preparation against such threats.

## Introduction

