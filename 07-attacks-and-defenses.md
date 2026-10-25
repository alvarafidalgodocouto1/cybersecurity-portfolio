# Pre Security — Attacks and Defenses

## Module overview

This module introduces the CIA triad, cryptography concepts, and the perspectives of hackers and defenders.

## 1. CIA triad

- **Confidentiality:** Information is accessible only to authorised parties.
- **Integrity:** Information remains accurate and is not changed improperly.
- **Availability:** Systems and information are accessible when needed.

Incidents can affect more than one goal. For example, data theft impacts confidentiality, tampering impacts integrity, and destructive malware may impact availability.

## 2. Cryptography concepts

- **Encoding:** Changes representation; it does not provide secrecy by itself.
- **Encryption:** Uses a key to protect confidentiality.
- **Hashing:** Produces a digest used in integrity checks and other applications.
- **Symmetric encryption:** Uses the same secret key to encrypt and decrypt.
- **Asymmetric cryptography:** Uses a related public/private key pair for functions such as digital signatures or key establishment.
- **Digital signatures:** Can support integrity and authenticity when keys and trust are properly managed.

Password storage should use a suitable password-hashing scheme with salts, not plaintext or a reversible cipher.

## 3. Become a hacker

Ethical hacking identifies weaknesses within an explicitly authorised scope. A responsible assessment defines targets, allowed techniques, time limits, reporting expectations, and rules for handling data.

## 4. Become a defender

Defenders reduce risk through secure configuration, patching, least privilege, monitoring, incident response, backups, and user education. Layered controls are important because no single control prevents every threat.

## Threat vocabulary

- **Threat:** Something capable of causing harm.
- **Vulnerability:** A weakness that could be exploited.
- **Exploit:** A method that takes advantage of a vulnerability.
- **Risk:** A way to consider likelihood and impact.

A vulnerability does not automatically mean that a system has been compromised.

## Key takeaways

- The CIA triad provides a model for security goals.
- Encoding, encryption, and hashing have different purposes.
- Ethical security work requires permission and defined scope.
- Defence combines technical controls, monitoring, and response processes.

## Rooms covered by this module

- The CIA Triad
- Cryptography Concepts
- Become a Hacker
- Become a Defender

## Official reference

[TryHackMe Pre Security](https://tryhackme.com/path/outline/presecurity)
