<div align="center">
  <img src="https://raw.githubusercontent.com/zulfff/zulfff/main/assets/hero.svg?v=2" alt="arya@zulfff — muhammad arya arjuna habibullah, security research / bug bounty / cve hunter" width="100%" />
</div>

<p align="center">
  <a href="https://hackerone.com/pelioro"><img src="https://img.shields.io/badge/hackerone-pelioro-0b0e14?style=flat-square&labelColor=0b0e14&logo=hackerone&logoColor=ff6b6b" alt="HackerOne"/></a>
  <a href="https://bugcrowd.com/JustAKids"><img src="https://img.shields.io/badge/bugcrowd-JustAKids-0b0e14?style=flat-square&labelColor=0b0e14&logo=bugcrowd&logoColor=ff8c42" alt="Bugcrowd"/></a>
  <a href="https://intigriti.com/zulfff"><img src="https://img.shields.io/badge/intigriti-zulfff-0b0e14?style=flat-square&labelColor=0b0e14&logo=intigriti&logoColor=a78bfa" alt="Intigriti"/></a>
  <a href="https://twitter.com/XDevTools"><img src="https://img.shields.io/badge/x-@pelioro-0b0e14?style=flat-square&labelColor=0b0e14&logo=x&logoColor=c9d1d9" alt="X / Twitter"/></a>
  <a href="https://www.linkedin.com/in/muhammad-arya-arjuna-habibulah/"><img src="https://img.shields.io/badge/linkedin-arya-0b0e14?style=flat-square&labelColor=0b0e14&logo=linkedin&logoColor=58a6ff" alt="LinkedIn"/></a>
  <a href="mailto:arjunaajalahla100@gmail.com"><img src="https://img.shields.io/badge/mail-0b0e14?style=flat-square&logo=gmail&logoColor=ea4335" alt="Email"/></a>
</p>

<p align="center">
  <a href="https://hub.xerj.org/contributors/zulfff"><img src="https://hub.xerj.org/contributors/zulfff/badge.svg" alt="XERJ Corpus Hub contributor"/></a>
</p>

<br/>

<p><samp><u>./focus</u></samp></p>

<p>
  <code>memory safety</code>
  <code>tls / pqc</code>
  <code>waf &amp; ddos</code>
  <code>ebpf</code>
  <code>rust</code>
  <code>agent tooling</code>
</p>

<br/>

<p><samp><u>./builds</u></samp></p>

| project | what it is |
| :------ | :--------- |
| [`argus`](https://github.com/zulfff/argus) | eBPF firewall and edge-router automation — XDP filtering, WireGuard ZTNA mesh, NetBox/VyOS reconcile |
| [`aegis-waf`](https://github.com/zulfff/aegis-waf) | WAF with behavioural threat detection and multi-layer DDoS mitigation, written in Rust |
| [`fortress-ws`](https://github.com/FortressCommunity/fortress-ws) | WebSocket gateway with threat detection, JWT auth, Redis rate limits and a gRPC Rust scanner |
| [`subhost`](https://github.com/zulfff/SubHost-demo) | DAG consensus, distributed storage and edge compute — quantum-resistant crypto, native IBC |
| [`lelouch`](https://github.com/zulfff/lelouch) | local-first compression of noisy tool output before it ever reaches the model |
| [`envforge`](https://github.com/zulfff/envforge) | zero-dependency config manager with validation, hot reload and secret masking |

<br/>

<p><samp><u>./cves</u></samp></p>

<sub>3 verified · 1 pending attribution · 1 advisory-only · listed newest first</sub>

<p>
  <samp><b>CVE-2026-104255</b> · liboqs · medium · advisory</samp><br/>
  <b>LM-OTS key reuse and signature forgery in LMS stateful signing</b><br/>
  Fail-open lock handling in LMS stateful signing allows LM-OTS key reuse. Tracked as advisory <code>GHSA-xv6c-h66p-6mfq</code>; no NVD record yet, so it is not counted in the verified set.<br/>
  <sub><code>cwe-787</code> <code>published 6 oct 2026</code> <code>patched 0.17.0</code> · <a href="https://github.com/open-quantum-safe/liboqs/security/advisories/GHSA-xv6c-h66p-6mfq">advisory ↗</a></sub>
</p>

<p>
  <samp><b>CVE-2026-6325</b> · wolfssl · 7.5 high · attribution pending</samp><br/>
  <b>Out-of-bounds write in SetSuitesHashSigAlgo</b><br/>
  An oversized signature algorithms list writes past the destination buffer. NVD records 7.5 high while the CNA records 2.0 low, and attribution to this profile is still unconfirmed — so it stays out of the verified count.<br/>
  <sub><code>cwe-787</code> <code>published 25 jun 2026</code> · <a href="https://github.com/wolfSSL/wolfssl/pull/10204">patch ↗</a></sub>
</p>

<p>
  <samp><b>CVE-2026-44518</b> · liboqs · 5.3 medium · fixed 0.16.0</samp><br/>
  <b>XMSS buffer overread</b><br/>
  XMSS and XMSS^MT verification fail to validate the caller-supplied signature length. A short buffer causes an out-of-bounds read whose bytes are consumed internally as hash input, with denial of service if the read crosses an unmapped page.<br/>
  <sub><code>cwe-125</code> <code>cwe-20</code> <code>published 29 may 2026</code> · <a href="https://nvd.nist.gov/vuln/detail/CVE-2026-44518">record ↗</a> <a href="https://github.com/open-quantum-safe/liboqs/security/advisories/GHSA-wf7v-fhxj-73m2">advisory ↗</a></sub>
</p>

<p>
  <samp><b>CVE-2026-5188</b> · wolfssl · 8.1 high · patched</samp><br/>
  <b>Integer underflow in X.509 Subject Alternative Name parsing</b><br/>
  A malformed Subject Alternative Name entry can declare a length larger than its enclosing sequence, wrapping the internal counter. Limited to configurations using the original ASN.1 parser, which is disabled by default.<br/>
  <sub><code>cwe-191</code> <code>cvss 3.1 8.1 high (nvd)</code> <code>cvss 4.0 2.3 low (cna)</code> <code>published 10 apr 2026</code> · <a href="https://github.com/wolfSSL/wolfssl/pull/10024">patch ↗</a></sub>
</p>

<p>
  <samp><b>CVE-2026-3229</b> · wolfssl · 5.5 medium · patched</samp><br/>
  <b>Integer overflow in certificate chain allocation</b><br/>
  An integer overflow in <code>wolfssl_add_to_chain</code> writes certificate data past an undersized buffer and corrupts the heap. Not directly remote — exploitation needs the certificate-loading context to be compromised first.<br/>
  <sub><code>cwe-122</code> <code>cvss 3.1 5.5 medium (nvd)</code> <code>cvss 4.0 1.2 low (cna)</code> <code>published 19 mar 2026</code> · <a href="https://github.com/wolfSSL/wolfssl/pull/9827">patch ↗</a></sub>
</p>

<br/>

<p><samp><u>./stack</u></samp></p>

<div align="left">
  <img src="https://skillicons.dev/icons?i=rust,go,c,cpp,python,ts,js,nodejs,linux,bash,docker,kubernetes,redis,git,github,neovim&perline=16" alt="Rust, Go, C, C++, Python, TypeScript, JavaScript, Node.js, Linux, Bash, Docker, Kubernetes, Redis, Git, GitHub, Neovim" />
</div>

<p>
  <code>ffuf</code>
  <code>nuclei</code>
  <code>amass</code>
  <code>ghidra</code>
  <code>radare2</code>
  <code>impacket</code>
  <code>bloodhound</code>
</p>

<br/>

<p><samp><u>./activity</u></samp></p>

<p>
  <samp>$ 3 verified cves · 2 libraries patched</samp><br/>
  <samp>$ <a href="https://github.com/zulfff?tab=repositories">67 public repositories</a></samp><br/>
  <samp>$ joined github in 2024</samp><br/>
  <samp>$ <a href="mailto:arjunaajalahla100@gmail.com">arjunaajalahla100@gmail.com</a></samp>
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=zulfff&theme=github-compact&hide_border=true&area=true&area_color=3b82f6&bg_color=00000000&color=8b949e&line=3b82f6&point=58a6ff&title_color=8b949e&custom_title=recent%20activity" alt="Recent contribution activity" width="100%" />
</p>

<details>
<summary><samp>contribution snake</samp></summary>
<br/>
<p align="center">
  <img src="https://raw.githubusercontent.com/zulfff/zulfff/output/github-contribution-grid-snake-dark.svg" alt="Contribution snake" width="100%" />
</p>
</details>

<br/>

<p align="center">
  <samp><sub>report responsibly · patch quickly</sub></samp>
</p>
