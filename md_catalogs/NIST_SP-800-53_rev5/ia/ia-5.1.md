---
x-trestle-set-params:
  ia-05.01_odp.01:
    values:
  ia-05.01_odp.02:
    values:
x-trestle-global:
  sort-id: ia-05.01
---

# ia-5.1 - \[Identification and Authentication\] Password-based Authentication

## Control Statement

For password-based authentication:

- \[(a)\] Maintain a list of commonly-used, expected, or compromised passwords and update the list {{ insert: param, ia-05.01_odp.01 }} and when organizational passwords are suspected to have been compromised directly or indirectly;

- \[(b)\] Verify, when users create or update passwords, that the passwords are not found on the list of commonly-used, expected, or compromised passwords in IA-5(1)(a);

- \[(c)\] Transmit passwords only over cryptographically-protected channels;

- \[(d)\] Store passwords using an approved salted key derivation function, preferably using a keyed hash;

- \[(e)\] Require immediate selection of a new password upon account recovery;

- \[(f)\] Allow user selection of long passwords and passphrases, including spaces and all printable characters;

- \[(g)\] Employ automated tools to assist the user in selecting strong password authenticators; and

- \[(h)\] Enforce the following composition and complexity rules: {{ insert: param, ia-05.01_odp.02 }}.

## Control Assessment Objective

for password-based authentication, a list of commonly used, expected, or compromised passwords is maintained and updated {{ insert: param, ia-05.01_odp.01 }} and when organizational passwords are suspected to have been compromised directly or indirectly;
for password-based authentication when passwords are created or updated by users, the passwords are verified not to be found on the list of commonly used, expected, or compromised passwords in IA-05(01)(a);
for password-based authentication, passwords are only transmitted over cryptographically protected channels;
for password-based authentication, passwords are stored using an approved salted key derivation function, preferably using a keyed hash;
for password-based authentication, immediate selection of a new password is required upon account recovery;
for password-based authentication, user selection of long passwords and passphrases is allowed, including spaces and all printable characters;
for password-based authentication, automated tools are employed to assist the user in selecting strong password authenticators;
for password-based authentication, {{ insert: param, ia-05.01_odp.02 }} are enforced.

## Control guidance

Password-based authentication applies to passwords regardless of whether they are used in single-factor or multi-factor authentication. Long passwords or passphrases are preferable over shorter passwords. Enforced composition rules provide marginal security benefits while decreasing usability. However, organizations may choose to establish certain rules for password generation (e.g., minimum character length for long passwords) under certain circumstances and can enforce this requirement in IA-5(1)(h). Account recovery can occur, for example, in situations when a password is forgotten. Cryptographically protected passwords include salted one-way cryptographic hashes of passwords. The list of commonly used, compromised, or expected passwords includes passwords obtained from previous breach corpuses, dictionary words, and repetitive or sequential characters. The list includes context-specific words, such as the name of the service, username, and derivatives thereof.
