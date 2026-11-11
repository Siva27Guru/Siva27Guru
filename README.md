## Hello Everyone,
I am,
[@Siva27Guru](https://siva27guru.github.io/Siva_Guru_Profile/)
## To Know me click on my name
## 12 hours for : **Passion to Dream  → Work To Do  →  Career to Drive** 
## can verify me @76e2d5c4bcc52001085c7b25251ed620b01677455b5e45441776f0fa4aa9a7b6 👋

<!--
**Siva27Guru/Siva27Guru** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
# 🧭 Engineering Philosophy                                        

I approach engineering from the security perspective:

**Code → Algorithms → Protocols → LLD → HLD**

```mermaid
flowchart LR
    A["Code"] --> B["Algorithms"] --> C["Protocols"] --> D["LLD"] --> E["HLD"]
    S(["🔐 Security is part of every layer"]) -.-> A
    S -.-> B
    S -.-> C
    S -.-> D
    S -.-> E
    style S fill:#0E7C86,color:#fff,stroke:#0E7C86
```

I believe secure systems are not created by adding security at the end. They are designed with security as a fundamental part of the architecture.

---

# 🔬 Current Technical Focus

Started with Solving Problems Designing architecture Finding Security and Scalability issues Addressing Intelligence requirement for better solution expanding to recieve help for an application to define its own scope in secure way thru AI In Security Engineer & Researching Journey to understand figureout Vulnerabilities to Providing Solutions without compromising traditional standards to suit modern update

```mermaid
flowchart LR
    A["Solving problems"] --> B["Designing architecture"]
    B --> C["Finding security and scalability issues"]
    C --> D["Addressing intelligence requirement"]
    D --> E["Application defines its own scope securely through AI"]
    E --> F["Understand vulnerabilities"]
    F --> G["Provide solutions without compromising traditional standards"]
```

Now Focusing on Public Key Infrastructure (PKI), digital certificates, cryptographic systems, and secure communication protocols. My work combines product development and R&D, exploring practical applications of security technologies across modern authentication and communication systems.

### Current work areas

- **PKI & Certificate Management** — X.509, certificate lifecycle, CA infrastructure, OCSP, CRL
- **Cryptography** — RSA, ECC, EdDSA, Post-Quantum Cryptography, and FHE
- **Secure Protocols** — TLS 1.3, mTLS, DTLS, and certificate-based authentication
- **Identity & Authentication** — WebAuthn, FIDO2, IAM, and passwordless authentication
- **IoT Security** — Device identity, trust establishment, and secure device communication
- **Backend Engineering** — Python (Django/Flask), Golang, REST APIs, PostgreSQL, MongoDB, Redis
- **System Design** — LLD, HLD, distributed systems, security architecture, and scalable backend design

```mermaid
mindmap
  root((Security Engineering))
    PKI and Certificates
      X.509
      Certificate lifecycle
      CA infrastructure
      OCSP
      CRL
    Cryptography
      RSA
      ECC
      EdDSA
      Post-Quantum
      FHE
    Secure Protocols
      TLS 1.3
      mTLS
      DTLS
      Certificate-based auth
    Identity and Authentication
      WebAuthn
      FIDO2
      IAM
      Passwordless
    IoT Security
      Device identity
      Trust establishment
      Secure device communication
    Backend Engineering
      Python Django Flask
      Golang
      REST APIs
      PostgreSQL
      MongoDB
      Redis
    System Design
      LLD
      HLD
      Distributed systems
      Security architecture
      Scalable backend
```

**Expanding Technical Focus:** IoT and Embedded Systems Security for Lightweight Systems; AI/ML for Innovative Systems; Backend Architecture; Cloud Technologies and MCP-based Infrastructure Automation.

I believe secure systems are not created by adding security at the end—they are designed with security as a fundamental part of the architecture.

Exploring how cryptography, PKI, authentication, protocols, and architecture can come together to build secure, scalable, and reliable technology solutions.

### 🧩 How the pieces fit together (click to expand)

<details>
<summary><b>PKI: how a certificate earns trust</b></summary>

```mermaid
flowchart TD
    R["Root CA<br/>self-signed, in the trust store"] -->|signs| I["Intermediate CA"]
    I -->|signs| L["Leaf certificate"]
    L --> V{"Validation"}
    V --> C1["Chain signatures"]
    V --> C2["Validity dates"]
    V --> C3["Revocation: OCSP / CRL"]
    V --> C4["Hostname match"]
    C1 & C2 & C3 & C4 --> OK(["Trusted connection"])
    style OK fill:#2E7D4F,color:#fff
```

</details>

<details>
<summary><b>TLS 1.3 handshake (with optional mTLS)</b></summary>

```mermaid
sequenceDiagram
    participant C as Client
    participant S as Server
    C->>S: ClientHello + key_share
    S->>C: ServerHello + key_share
    Note over C,S: Handshake keys derived, traffic is now encrypted
    S->>C: EncryptedExtensions
    opt mTLS
        S->>C: CertificateRequest
    end
    S->>C: Certificate
    S->>C: CertificateVerify
    S->>C: Finished
    opt mTLS
        C->>S: Certificate + CertificateVerify
    end
    C->>S: Finished
    C-->>S: Application data (forward-secret keys)
    S-->>C: Application data
```

</details>

<details>
<summary><b>Where the layers meet in an IoT deployment</b></summary>

```mermaid
flowchart LR
    D["IoT device<br/>device identity + certificate"] <-->|"mTLS / DTLS"| G["Gateway / backend API"]
    G --> DB[("PostgreSQL / MongoDB / Redis")]
    CA["CA infrastructure<br/>issue, renew, revoke"] -.->|"OCSP / CRL"| G
    CA -.->|"enroll"| D
```

</details>

---

# 🌍 My Open-Source Journey

My intention is to:

- Document what I learn consistently.
- Convert theoretical knowledge into practical experiments.
- Implement real-world use cases.
- Improve my problem-solving and architectural thinking.
- Maintain reusable technical references.
- Gradually develop complete, well-documented projects.

Contribute practical implementations and project code to the open-source community in the coming months. My vision is to create open-source repositories that empower everyone to learn, experiment, architect, implement, and validating ideas through practical implementation — ultimately extending their capabilities from the physical world into a secure digital space.

I want every project in my repositories to create a meaningful learning and collaboration environment for developers at different stages of their engineering journey.

| Level | Focus | What it means |
|---|---|---|
| 🌱 **Beginners** | Learn by Building | Understand programming fundamentals, explore real-world use cases, and discover the practical value of technology through hands-on implementation. |
| 🏗️ **Intermediate Developers** | Think and Architect | Develop decision-making capabilities by evaluating design choices, comparing approaches, understanding trade-offs, and improving architectural efficiency, scalability, and security. |
| 🚀 **Experts** | Review, Challenge and Innovate | Share technical expertise, challenge existing implementations, identify improvement opportunities, and contribute suggestions that make projects more efficient, secure, scalable, and reliable. |

My intention is to make every repository a shared engineering space where beginners learn, intermediates develop architectural thinking, and experts help drive continuous improvement.

Because meaningful open-source development happens when knowledge flows in every direction.

**Build → Document → Experiment → Validate → Share → Improve.**

| Level | Focus | What it means |
|---|---|---|
| 🌱 **Beginners** | Learn by Building | Understand programming fundamentals, explore real-world use cases, and discover the practical value of technology through hands-on implementation. |
| 🏗️ **Intermediate Developers** | Think and Architect | Develop decision-making capabilities by evaluating design choices, comparing approaches, understanding trade-offs, and improving architectural efficiency, scalability, and security. |
| 🚀 **Experts** | Review, Challenge and Innovate | Share technical expertise, challenge existing implementations, identify improvement opportunities, and contribute suggestions that make projects more efficient, secure, scalable, and reliable. |

My intention is to make every repository a shared engineering space where beginners learn, intermediates develop architectural thinking, and experts help drive continuous improvement.

Because meaningful open-source development happens when knowledge flows in every direction.

**Build → Document → Experiment → Validate → Share → Improve.**

```mermaid
flowchart LR
    B["Build"] --> D["Document"] --> E["Experiment"] --> V["Validate"] --> S["Share"] --> I["Improve"]
    I -.->|"next iteration"| B
    BG["🌱 Beginners learn"] -.-> B
    IM["🏗️ Intermediates architect"] -.-> E
    EX["🚀 Experts review"] -.-> V
```

---

# 💬 Let's Connect
```mermaid
flowchart LR
    B["Build"] --> D["Document"] --> E["Experiment"] --> V["Validate"] --> S["Share"] --> I["Improve"]
    I -.->|"next iteration"| B
    BG["🌱 Beginners learn"] -.-> B
    IM["🏗️ Intermediates architect"] -.-> E
    EX["🚀 Experts review"] -.-> V
```

---

# 💬 Let's Connect

If you are interested in cryptography, PKI, cybersecurity, security research, architecture, or open-source engineering, let's exchange ideas and build something meaningful.

💻 GitHub: [@Siva27Guru](https://github.com/Siva27Guru)

💼 LinkedIn: [Connect with me](https://www.linkedin.com/in/siva27guru01/)

---

# ⚡ A Continuous Engineering Journey

**Consistent Learning. Reliable Building. Practical Research. Open-Source Contribution.**

Understanding problems deeply, designing securely, and continuously seeking better ways to solve complex engineering challenges.

💼 LinkedIn: [Connect with me](https://www.linkedin.com/in/siva27guru01/)

⚡ A Continuous Engineering Journey

Consistent Learning. Reliable Building. Practical Research. Open-Source Contribution.

Understanding problems deeply, designing securely, and continuously seeking better ways to solve complex engineering challenges.
