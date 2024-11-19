

# John the Ripper  
**John the Ripper** is one of the most popular tools in Kali Linux for performing brute force attacks. This repository provides the best and easiest way to get started with this powerful tool.  

<div align="center">  
  <img src="https://github.com/user-attachments/assets/bff2f291-5cfd-4b63-98b7-33f93a055687" alt="John the Ripper Logo">  
</div>  

---

## Table of Contents  
- [Introduction](#introduction)  
- [Features](#features)  
- [Installation](#installation)  
- [Usage Guide](#usage-guide)  
- [License](#license)  

---

## Introduction  
John the Ripper is an open-source password-cracking tool designed to perform dictionary attacks and password hash testing. It's widely used in cybersecurity for penetration testing and security assessments.  

---

## Features  
- Supports a variety of hash types (MD5, SHA-256, etc.)  
- Highly customizable and scalable  
- Integrates well with other tools  
- Compatible with multiple platforms  

---

## Installation  
1. **Clone the repository:**  
   ```bash  
   git clone https://github.com/your-repo/john-the-ripper.git  
   ```  

2. **Navigate to the directory:**  
   ```bash  
   cd john-the-ripper  
   ```  

3. **Install dependencies:**  
   ```bash  
   sudo apt update && sudo apt install build-essential libssl-dev  
   ```  

4. **Build the tool:**  
   ```bash  
   make -s clean && make -sj4  
   ```  

---

## Usage Guide  
To perform a brute force attack using John the Ripper, follow these steps:  

1. **Create a wordlist** or use a pre-existing one (e.g., `rockyou.txt`).  
2. **Hash the password:**  
   ```bash  
   echo -n "password" | md5sum  
   ```  
3. **Run John the Ripper:**  
   ```bash  
   john --wordlist=rockyou.txt --format=raw-md5 hashed_password.txt  
   ```  

---

## License  
This project is licensed under the [MIT License](LICENSE).  

---  
