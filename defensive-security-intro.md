# Cyber Security 101 — Defensive Security Intro

## Purpose

Defensive security focuses on reducing risk, monitoring systems, detecting suspicious activity, investigating incidents, and restoring normal operations.

## Defensive-security areas

- **SOC:** Monitors alerts and investigates potential security incidents.
- **Threat intelligence:** Collects and evaluates information about threats and adversary behaviour.
- **DFIR:** Digital forensics and incident response; preserves and analyses evidence and coordinates response.
- **Malware analysis:** Examines suspicious software to understand behaviour and impact.
- **Security engineering:** Designs and maintains technical controls.

## A basic alert-triage workflow

1. Validate the alert and identify the affected asset.
2. Gather related endpoint, network, identity, and application telemetry.
3. Build a timeline.
4. Assess scope, impact, and confidence.
5. Escalate or respond according to playbooks.
6. Document evidence and decisions.

An alert is a signal to investigate. False positives and benign events are possible, so analysts should correlate multiple data points before making a conclusion.

## Common telemetry

- Authentication events
- Endpoint process and network activity
- DNS and proxy logs
- Firewall events
- Web server access logs
- SIEM correlation alerts

## Key takeaways

- Defensive security is a continuous process.
- Context and correlation are necessary for reliable conclusions.
- Evidence should be handled consistently and documented.
- Response actions must follow organisational procedures and authority.

## Official room

[TryHackMe Cyber Security 101](https://tryhackme.com/path/outline/cybersecurity101)
