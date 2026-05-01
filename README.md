<div align="center">

# Muhammad Arya Arjuna Habibullah

**Security Researcher | Bug Bounty Hunter | Vulnerability Finder**

[![HackerOne](https://img.shields.io/badge/HackerOne-pelioro-red?style=for-the-badge&logo=hackerone)](https://hackerone.com/pelioro)
[![Bugcrowd](https://img.shields.io/badge/Bugcrowd-JustAKids-blue?style=for-the-badge&logo=bugcrowd)](https://bugcrowd.com/JustAKids)
[![Intigriti](https://img.shields.io/badge/Intigriti-zulfff-purple?style=for-the-badge&logo=intigriti)](https://intigriti.com/zulfff)

</div>

---

## About Me

Security researcher who loves finding vulnerabilities in web apps, APIs, and cryptography. I fucking love digging into code to uncover bugs that could impact millions of users. Not just finding bugs, but also learning how to fucking break systems in cool ways.

- **Specializations**: Web Security, Cryptography, Binary Analysis
- **Based**: Indonesia
- **Active Platforms**: HackerOne, Bugcrowd, Intigriti
- **Learning**: Always exploring new attack vectors and defense mechanisms, idgaf how hard it gets

---

## CVE Discoveries - This shit is real

### CVE-2026-5188
**Integer Underflow in wolfSSL X.509 SAN Parsing**

- **CWE**: CWE-191 (Integer Underflow)
- **CVSS Score**: 8.1 (high)
- **Description**: An integer underflow issue exists in wolfSSL when parsing the Subject Alternative Name (SAN) extension of X.509 certificates. A malformed certificate can specify an entry length larger than the enclosing sequence, causing the internal length counter to wrap during parsing.
- **Impact**: Incorrect handling of certificate data in configurations using the original ASN.1 parsing implementation
- **References**: 
  - [NVD](https://nvd.nist.gov/vuln/detail/CVE-2026-5188)
  - [CVE.org](https://www.cve.org/CVERecord?id=CVE-2026-5188)
  - [wolfSSL PR](https://github.com/wolfSSL/wolfssl/pull/10024)

### CVE-2026-3229
**Integer Overflow in wolfSSL wolfssl_add_to_chain**

- **CWE**: CWE-122 (Heap-based Buffer Overflow)
- **CVSS Score**: 5.5 (Medium)
- **Description**: An integer overflow vulnerability existed in the static function wolfssl_add_to_chain, that caused heap corruption when certificate data was written out of bounds of an insufficiently sized certificate buffer. The function is called by wolfSSL_CTX_add_extra_chain_cert, wolfSSL_CTX_add1_chain_cert, and wolfSSL_add0_chain_cert APIs. These APIs are enabled for 3rd party compatibility features: enable-opensslall, enable-opensslextra, enable-lighty, enable-stunnel, enable-nginx, enable-haproxy.
- **Impact**: Heap corruption leading to potential code execution in compromised application contexts
- **References**:
  - [NVD](https://nvd.nist.gov/vuln/detail/CVE-2026-3229)
  - [wolfSSL PR](https://github.com/wolfSSL/wolfssl/pull/9827)

---

## Skills & Technologies - Tools I fucking use

### Security Research
- Web Application Security
- API Security Testing
- Cryptography Analysis
- Binary Exploitation
- Reverse Engineering

### Tools & Frameworks
- ffuf (fuzzing)
- nuclei (vulnerability scanning)
- subfinder (subdomain enumeration)
- httpx (HTTP toolkit)
- amass (OSINT)
- ghidra (reverse engineering)
- radare2 (binary analysis)
- pwntools (exploitation)
- bloodhound (AD security)
- crackmapexec (pentesting)
- impacket (protocol attacks)

### Programming Languages
```python
Python = "Primary"
JavaScript = "Web Security"
C/C++ = "Binary Analysis"
Go = "Tool Development"
```

---

## Bug Bounty Achievements

- Multiple valid reports on HackerOne - this shit pays
- Recognized researcher on Bugcrowd - yeah, I'm that good
- Active contributor on Intigriti - always hunting
- CVE Finder (2026) - found 2 CVEs in wolfSSL, fuck yeah

---

## Contact

<div align="center">

[![Twitter](https://img.shields.io/badge/Twitter-%40pelioro-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/XDevTools)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Muhammad%20Arya%20Arjuna%20Habibullah-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/muhammad-arya-arjuna-habibulah/)
[![Email](https://img.shields.io/badge/Email-Contact%20Me-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:arjunaajalahla100@gmail.com)

</div>

---

<div align="center">

**"Bug hunting is not just a hobby, it's a fucking lifestyle."**

**If you like my shit, give it a fucking star!**

</div>

---

<div align="center">

**Visitors - come look at this shit**

![Visitor Count](https://profile-counter.glitch.me/pelioro/count.svg)

</div>
y
