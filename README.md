# 🔐 Python Ransomware Demonstration

An educational Python project that demonstrates the **basic concepts behind ransomware**, including file encryption, asymmetric key generation, and recovery/decryption workflows.

> ⚠️ **Educational & Authorized-Use Disclaimer**
>
> This project is intended **strictly for cybersecurity education, research, and controlled laboratory environments**. Only run it on files and systems you own or have explicit permission to test.
>
> Never deploy ransomware or ransomware-like software against systems, files, or users without authorization.

## 📖 Overview

Ransomware is a type of malware that prevents victims from accessing their data, commonly by encrypting files and requiring a recovery mechanism.

This project provides a controlled demonstration of some of the cryptographic concepts involved in such attacks.

The project uses:

* **Python**
* **RSA** for asymmetric public/private key cryptography
* **Fernet** for symmetric encryption
* Local test files for demonstrating encryption and recovery

The repository is designed to help students and security researchers understand how these cryptographic components can be combined in a ransomware-style workflow.

## 🧰 Technologies

| Technology   | Purpose                         |
| ------------ | ------------------------------- |
| Python 3.7   | Application runtime             |
| RSA          | Public/private key cryptography |
| Fernet       | Symmetric encryption            |
| Cryptography | Cryptographic implementation    |

## 📁 Project Structure

```text
galaxy11/
│
├── ransom.py
├── RSA_private_public_keys.py
├── Decrypt_fernet_key.py
└── README.md
```

### `ransom.py`

Contains the main demonstration logic for encrypting files within the designated test environment.

### `RSA_private_public_keys.py`

Demonstrates generation of an RSA public/private key pair used as part of the cryptographic workflow.

### `Decrypt_fernet_key.py`

Demonstrates the recovery/decryption portion of the project.

## 🔑 Cryptography Concepts

The project demonstrates a combination of **symmetric and asymmetric cryptography**.

### Symmetric encryption

Fernet provides symmetric authenticated encryption.

Conceptually:

```text
Plaintext
    │
    ▼
Fernet Key
    │
    ▼
Encrypted Data
```

The same secret key is required to decrypt the encrypted data.

### Asymmetric encryption

RSA uses a key pair:

```text
             RSA Key Pair
            /            \
           ▼              ▼
      Public Key      Private Key
           │              │
           │              │
      Encryption       Decryption
```

The combination of these techniques is commonly referred to as **hybrid encryption**.

## 🧪 Safe Laboratory Setup

For educational experimentation, use a completely isolated test environment.

Recommended setup:

* Use a virtual machine or disposable test environment.
* Create a dedicated directory containing **dummy files only**.
* Do not use personal documents or production data.
* Do not run the project on another person's computer.
* Do not connect the test environment to systems you do not control.
* Keep backups of any test data you want to preserve.

### Example test data

```text
lab/
├── test1.txt
├── test2.txt
└── test3.txt
```

Use only disposable files in the laboratory.

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/Ibrahist/galaxy11.git
cd galaxy11
```

Create a virtual environment:

### Windows

```bash
python -m venv .venv
.venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the required cryptography dependency:

```bash
pip install cryptography
```

## ▶️ Running the Demonstration

The repository contains separate scripts for:

1. RSA key generation
2. The controlled encryption demonstration
3. Recovery/decryption of the demonstration data

Run these **only inside your isolated test environment and against disposable test files**.

The original repository was created with Python 3.7.

## 🔬 Learning Objectives

This project can be used to study:

* Symmetric vs. asymmetric cryptography
* RSA public/private key pairs
* Fernet encryption
* Hybrid encryption concepts
* File encryption concepts
* Malware analysis fundamentals
* Ransomware attack chains
* Defensive cybersecurity techniques

## 🛡️ Defensive Security Takeaways

Understanding ransomware behavior can help security professionals develop defenses.

Useful defensive measures include:

* Maintain offline or immutable backups.
* Apply security updates regularly.
* Use endpoint detection and response (EDR).
* Monitor unusual file modification activity.
* Restrict unnecessary administrative privileges.
* Segment critical systems and networks.
* Monitor suspicious encryption activity.
* Train users to recognize phishing and malicious attachments.
* Test backup restoration procedures regularly.

## ⚠️ Important Safety Notice

This project can modify files during execution.

**Never point the demonstration at:**

* Your operating system directories
* Personal documents
* Production servers
* Shared network drives
* Other people's computers
* Any system you do not explicitly own or have permission to test

Use a disposable laboratory environment and dummy data.

## 🧑‍💻 Educational Use

Potential educational applications include:

* Cybersecurity classes
* Malware-analysis laboratories
* Cryptography demonstrations
* Security research
* Blue-team detection exercises
* Controlled incident-response simulations

## 📌 Limitations

This is an **educational demonstration**, not production security software.

The implementation should not be interpreted as a complete representation of modern ransomware families. Real-world ransomware can involve substantially more sophisticated techniques, infrastructure, persistence mechanisms, evasion methods, and operational components.

## 🤝 Contributing

Contributions that improve the project's **educational and defensive value** are welcome.

Examples include:

* Improving documentation
* Adding explanatory comments
* Adding safe unit tests
* Adding cryptography explanations
* Adding defensive detection examples
* Improving laboratory isolation instructions

Please avoid contributions intended to facilitate unauthorized deployment or misuse.

## 📄 License

No explicit open-source license is currently specified in the repository.

If you plan to distribute or accept external contributions, consider adding an appropriate license.

## 👤 Author

**Ibrahist**

GitHub: https://github.com/Ibrahist

## ⭐ Repository

If this project is useful for learning cybersecurity concepts, consider starring the repository.

---

**Built for cybersecurity education, research, and controlled laboratory experimentation.**
