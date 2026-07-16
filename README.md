# Write-ups

Write-ups de pentest de máquinas do **TryHackMe**, produzidos durante a disciplina de **Tópicos Avançados em Computadores (TAC)** na Universidade de Brasília (UnB).

Cada write-up documenta o processo completo de comprometimento de uma máquina: **enumeração → exploração → escalonamento de privilégio → captura de flag**, com foco em técnicas reais de segurança ofensiva.

---

## 📋 Índice de Máquinas

| Máquina | Plataforma | Dificuldade | Técnicas Principais | Write-up |
|---------|-----------|-------------|---------------------|----------|
| [Agent Sudo](./AgentSudo/) | TryHackMe | Fácil | Enumeração HTTP, esteganografia, CVE-2019-14287 (sudo bypass) | [📄 PDF](./AgentSudo/AgentSudo.pdf) |
| [Blue](./Blue/) | TryHackMe | Fácil | Enumeração SMB, EternalBlue (MS17-010), Metasploit | — |
| [Blueprint](./Blueprint/) | TryHackMe | Médio | Enumeração SMB/HTTP, exploit osCommerce, dump de hashes | [📄 PDF](./Blueprint/Blueprint.pdf) |
| [Bounty Hacker](./BountyHacker/) | TryHackMe | Fácil | Enumeração FTP anônimo, brute-force SSH (Hydra), sudo tar | [📄 PDF](./BountyHacker/BountyHacker.pdf) |
| [Brooklyn 99](./Brooklyn99/) | TryHackMe | Fácil | Esteganografia, brute-force SSH, sudo less | — |
| [Chocolate Factory](./ChocolateFactory/) | TryHackMe | Fácil | Enumeração FTP/HTTP, RCE via injeção de comando, sudo vi | [📄 PDF](./ChocolateFactory/ChocolateFactory.pdf) |
| [Crack The Hash](./CrackTheHash/) | TryHackMe | Fácil | Hash cracking (MD5, SHA-1, SHA-256, bcrypt), Hashcat, CrackStation | [📄 PDF](./CrackTheHash/CrackTheHash.pdf) |
| [FowSniff](./FowSniff/) | TryHackMe | Fácil | Enumeração SMB, OSINT, brute-force POP3, shell via .procmailrc | [📄 PDF](./FowSniff/FowSniff.pdf) |
| [Kenobi](./Kenobi/) | TryHackMe | Fácil | Enumeração SMB/NFS, ProFTPD mod_copy, path variable manipulation | — |
| [Lazy Admin](./LazyAdmin/) | TryHackMe | Fácil | Enumeração web (Gobuster), CMS SweetRice RCE, sudo perl | [📄 PDF](./LazyAdmin/LazyAdmin.pdf) |
| [Lookup](./Lookup/) | TryHackMe | Fácil | Enumeração web, brute-force, elFinder RCE (CVE-2019-9194), sudo look | [📄 PDF](./Lookup/Lookup.pdf) |
| [Pickle Rick](./PickleRick/) | TryHackMe | Fácil | Enumeração web, RCE via command injection em painel web, sudo -l | [📄 PDF](./PickleRick/PickleRick.pdf) |
| [Relevant](./Relevant/) | TryHackMe | Médio | Enumeração SMB, upload de shell via share, token impersonation (PrintSpoofer) | [📄 PDF](./Relevant/Relevant.pdf) |
| [RootMe](./RootMe/) | TryHackMe | Fácil | Enumeração web (Gobuster), upload de shell PHP, SUID python | [📄 PDF](./RootMe/Writeup_RootMe.pdf) |
| [Simple CTF](./SimpleCTF/) | TryHackMe | Fácil | Enumeração web, SQLi CMS Made Simple, brute-force SSH, sudo vim | [📄 PDF](./SimpleCTF/SimpleCTF.pdf) |
| [Tom Ghost](./TomGhost/) | TryHackMe | Fácil | Ghostcat (CVE-2020-1938), AJP exploit, cracking de credenciais PGP | [📄 PDF](./TomGhost/TomGhost.pdf) |

---

## 🛠️ Técnicas Abordadas

- **Enumeração**: Nmap, Gobuster, enum4linux, SMB/FTP/HTTP reconnaissance
- **Exploração Web**: RCE via upload de shell, SQL injection, command injection
- **Exploits Conhecidos**: EternalBlue (MS17-010), Ghostcat (CVE-2020-1938), CVE-2019-14287, elFinder RCE
- **Escalonamento de Privilégio Linux**: Abusos de sudo (vim, perl, python, tar, less, look), SUID binaries, PATH hijacking
- **Escalonamento de Privilégio Windows**: Token impersonation (PrintSpoofer), hash dumping
- **Cracking**: Hashcat, John the Ripper, CrackStation — MD5, SHA-1, bcrypt, PGP
- **Ferramentas**: Metasploit, Hydra, Netcat, Burp Suite, Steghide

---

## 📁 Estrutura do Repositório

```
TAC-UnB-Write-ups/
├── AgentSudo/        # CVE-2019-14287 + esteganografia
├── Blue/             # EternalBlue MS17-010
├── Blueprint/        # osCommerce RCE + hash dump
├── BountyHacker/     # FTP anônimo + sudo tar
├── Brooklyn99/       # Esteganografia + sudo less
├── ChocolateFactory/ # Command injection + sudo vi
├── CrackTheHash/     # Hash cracking multi-algoritmo
├── FowSniff/         # POP3 brute-force + .procmailrc
├── Kenobi/           # ProFTPD + NFS
├── LazyAdmin/        # SweetRice CMS RCE
├── Lookup/           # elFinder RCE (CVE-2019-9194)
├── PickleRick/       # Web command injection
├── Relevant/         # SMB shell upload + token impersonation
├── RootMe/           # PHP upload + SUID python
├── SimpleCTF/        # SQLi + sudo vim
└── TomGhost/         # Ghostcat CVE-2020-1938
```

---

## 👤 Sobre

Repositório mantido por **[@Mateusrb6](https://github.com/Mateusrb6)** como portfólio de segurança ofensiva.  
Disciplina: **Tópicos Avançados em Computadores** — Universidade de Brasília (UnB).
