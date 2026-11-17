# NETWORKWALKS-B084-WK3-CYBERSECURITy
**Password Security, Password Auditing & Hash Analysis using John the Ripper**

## 1. Introduction

This report documents the hands-on cybersecurity activities performed during Week 3 of my Cybersecurity Internship at **NetworkWalks**.

This week's focus was on password security, password auditing, hash extraction, and password recovery techniques using **John the Ripper (JTR)**.

I explored how password auditing tools work, how password hashes can be extracted from encrypted PDF documents, and how wordlists are used to test password candidates in controlled lab environments.

The practical exercises also included password-related Capture The Flag (CTF) challenges to strengthen my understanding of cybersecurity concepts.

## 2. Objectives

- Understand password security and password auditing techniques.
- Install and configure John the Ripper Jumbo on macOS.
- Explore command-line and graphical interfaces.
- Perform wordlist-based password auditing.
- Extract password hashes from password-protected PDF files.
- Understand hash formats and password verification mechanisms.
- Practice password recovery using custom wordlists.
- Solve practical password-related CTF challenges.

## 3. Tools Used

| Tool | Purpose |
|---|---|
| John the Ripper Jumbo | Password auditing and recovery |
| Johnny | Graphical frontend for John the Ripper |
| pdf2john.pl | Extract password hashes from PDF files |
| macOS | Operating system used for practical exercises |
| Homebrew | Package manager used for installation |
| Python | Supporting scripts and experimentation |
| Wordlists | Generate and test password candidates |
| PDF Encryption | Understand password-protected documents |

## 4. Activities Performed

### 4.1 John the Ripper Installation and Configuration

**Step 1: Installation of John the Ripper Jumbo**

Installed and configured John the Ripper Jumbo on macOS.

Explored its command-line interface and understood its role in password security auditing.

```bash
brew install john-jumbo
```

**Step 2: Exploring John the Ripper**

Explored the available commands and options.

```bash
john --help
```

Studied its password auditing capabilities and explored how different password recovery modes work.

**Step 3: Wordlist-Based Password Auditing**

Experimented with dictionary-based password attacks using wordlists in a controlled lab environment.

Learned how John the Ripper tests password candidates against extracted password hashes.

**Step 4: Exploring Johnny GUI**

Explored Johnny, the graphical frontend for John the Ripper.

Understood how the graphical interface simplifies password auditing operations and displays results.

### 4.2 Password Hash Extraction and Analysis

**Step 1: Creating Password-Protected PDF Files**

Created test PDF documents protected with passwords to understand PDF encryption and password verification.

**Step 2: Extracting PDF Password Hashes**

Used `pdf2john.pl` to extract password hashes from the protected PDF documents.

The extracted hash information was used for password auditing in the lab environment.

```bash
pdf2john.pl sample.pdf
```

**Step 3: Hash Analysis**

Examined the relationship between encrypted documents and password-verification data.

Studied how extracted hashes are represented and why identifying the correct hash format is important.

**Step 4: Testing Custom Wordlists**

Used custom wordlists to test password candidates against the extracted hashes.

Successfully recovered passwords from deliberately vulnerable practice samples.

### 4.3 Practical CTF Challenges

Worked through password-related Capture The Flag (CTF) challenges to apply the concepts learned during the exercises.

Activities included:

- Solving password-related cybersecurity challenges.
- Capturing multiple training flags.
- Practicing password auditing concepts.
- Exploring persistence-related challenges.
- Improving command-line skills and practical problem-solving abilities.

These exercises helped connect theoretical password security concepts with practical cybersecurity scenarios.

## 5. Key Concepts Learned

| Concept | Description |
|---|---|
| Password Auditing | Evaluating password strength using security tools |
| Password Hashing | Converting passwords into hash representations for verification |
| Hash Extraction | Retrieving password-verification data from protected files |
| Dictionary Attack | Testing password candidates from a predefined wordlist |
| Wordlist Generation | Preparing candidate passwords for auditing |
| PDF Encryption | Understanding password protection in PDF documents |
| Hash Identification | Recognizing hash formats before performing password audits |
| Checksum vs Password Hash | Understanding the difference between file integrity checks and password-verification hashes |

## 6. Observations and Learnings

During this week's practical exercises, I learned that password auditing is not simply about trying random combinations.

It involves understanding:

1. **Hash Formats:** Different applications use different password-hashing and verification formats.
2. **Candidate Generation:** Wordlists help generate possible passwords for testing.
3. **Password Verification:** Extracted hashes allow auditing tools to verify password candidates without directly decrypting the original password.
4. **Computational Cost:** Password recovery depends on factors such as password complexity, hash algorithm, and available computing resources.
5. **Tool Interpretation:** Understanding tool output is important for identifying successful password recovery and avoiding incorrect conclusions.

I also learned the importance of distinguishing file checksums from password-verification hashes.

## 7. Recommendations and Security Best Practices

1. **Use Strong Passwords:** Create long, unique passwords that are difficult to guess.
2. **Avoid Common Passwords:** Do not use predictable passwords or commonly available wordlist entries.
3. **Use Password Managers:** Store and manage unique passwords securely.
4. **Enable Multi-Factor Authentication:** Add an additional layer of account protection.
5. **Use Secure Password Hashing:** Applications should use modern password-hashing algorithms such as Argon2id, bcrypt, or scrypt.
6. **Perform Regular Audits:** Periodically evaluate password security using authorized auditing tools.
7. **Protect Sensitive Documents:** Use strong passwords when encrypting confidential PDF documents.

## 8. Conclusion

During Week 3 of my Cybersecurity Internship at **NetworkWalks**, I gained practical experience with password security, password auditing, and hash analysis.

I installed and explored John the Ripper Jumbo, worked with its Johnny graphical frontend, extracted password hashes from encrypted PDF documents using `pdf2john.pl`, and performed wordlist-based password recovery on practice samples.

I also participated in practical CTF challenges and captured multiple training flags.

Overall, these exercises improved my understanding of password-verification mechanisms, hash formats, dictionary-based attacks, and the importance of strong password practices.

This week provided valuable hands-on experience in understanding how password auditing works and how security professionals identify weak password practices.

---

**End of Week 3 Report**
