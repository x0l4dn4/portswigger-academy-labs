# PortSwigger Web Security Academy Labs

Personal study repository for tracking progress and documenting completed labs while learning web application security through the [PortSwigger Web Security Academy](https://portswigger.net/web-security). Each lab will have notes and a Python script that reproduces the exploitation flow. Each topic is described in `About.md` to get a theoretical introduction before labs.

## Repository Structure

```text
├── assets/
│   ├── sqli-lab01.jpg
│   └── ...
├── template/
│   ├── notes-template.md
│   └── exploit-template.py
├── topics/
│   ├── sql-injection/
│   │   ├── About.md
│   │   ├── lab-01-login-bypass/
│   │   │   ├── notes.md
│   │   │   └── exploit.py
│   │   └── lab-02-union-attack/
│   │       ├── notes.md
│   │       └── exploit.py
│   ├── XSS/
│   │   ├── About.md
│   │   └── lab-01-reflected-xss/
│   │       ├── notes.md
│   │       └── exploit.py
│   ├── authentication/
│   ├── access-control/
│   ├── csrf/
│   └── ...
├── README.md
├── resources.md
```