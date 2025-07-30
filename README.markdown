# Proanant1/Project-Guide

## Folders and files

| Name |  | Name | Last commit message | Last commit date |
|-------|-------|-------|-------|-------|
| 📜 README.md | | | Initial setup guide | 2025-07-30 |
| 📁 tictactoe | | | Tic Tac Toe game | - |
| 📁 irc100Mint | | | ERC-100 token minting | - |
| 📁 nexus | | | Nexus project | - |
| 📁 soundness | | | Computational integrity | - |
| 📁 zama-commit-test | | | Commit testing | - |

## Introduction 📔

🌟 Welcome to the *Proanant1 Project Guide*! This repo is your one-stop guide to exploring my GitHub projects at *https://github.com/Proanant1*. My work includes *tictactoe* (a fun game), *irc100Mint* (blockchain token experiment), *nexus* (collaborative project), *soundness* (computational integrity), and *zama-commit-test* (version control testing). Follow this guide to set up, run, and contribute to these projects! 🚀

Read every step carefully to understand the setup process. Let’s dive in! ❗

## Benefits 📈

* **Learn by Doing**: Gain hands-on experience with game dev, blockchain, and more.
* **Contribute**: Enhance your GitHub portfolio by contributing to open-source projects.
* **Tech Variety**: Work with JavaScript, Solidity, and other tools across projects.
* **Community**: Join developers collaborating on *Proanant1* repositories.

## What Most Matters 🧩

* **Project Setup**: Get projects running locally or in the cloud.
* **Contribution Quality**: Improve code, docs, or fix bugs.
* **Engagement**: Interact via issues and pull requests.
* **Scoring**: Success = Completion Rate × Contribution Quality × Engagement.

## Device/System Requirements 💻

### Check Specs
* **Windows**: Press `Win + R`, type `dxdiag` for CPU, RAM, GPU details.
* **Linux/Cloud**:
  ```bash
  lscpu
  nvidia-smi
  ```

### Monitor Resources
```bash
htop
```

### Operating System
* Supported: Ubuntu 20.04/22.04 ☑️, Windows 10/11 (with WSL2) ☑️
* Not Supported: Ubuntu 24.04+ ❌, macOS (limited) ❌

Install Ubuntu 22.04: [Guide](https://ubuntu.com/download/desktop)

## Pre-Requirements 🛠

### Install Tools
* **Docker & Docker Compose**: [Docker Desktop](https://www.docker.com/get-started/) (Windows/Mac) or [Docker Install](https://docs.docker.com/engine/install/ubuntu/) (Linux).
* **Git**:
  ```bash
  sudo apt install git -y
  ```

### Install Dependencies
```bash
sudo apt update && sudo apt upgrade -y
sudo apt install curl git wget nodejs npm python3 python3-pip build-essential -y
```

## Clone Repository
```bash
git clone https://github.com/Proanant1/Project-Guide
cd Project-Guide
```

## Setup Instructions 🚀

### 1. Project-Specific Setup

#### *tictactoe* (JavaScript Game)
```bash
cd tictactoe
npm install
npm start
```
* Access: `http://localhost:3000`
* Needs: Node.js, npm (installed above).

#### *irc100Mint* (Solidity Contract)
```bash
cd irc100Mint
npm install -g truffle
truffle compile
truffle migrate --network <your_network>
```
* Needs: Truffle, Ethereum RPC (e.g., Infura).

#### Other Projects (*nexus*, *soundness*, *zama-commit-test*)
* Check each repo’s README for specific instructions.

### 2. Environment Variables
```bash
sudo nano .env
```
Add (e.g., for *irc100Mint*):
```
PRIVATE_KEY=Your_Private_Key_Without_0x
RPC_URL="Your_RPC_URL"
```
Inject:
```bash
source .env
```

### 3. Docker Setup (Optional)
```bash
docker-compose up -d
```
* Edit `docker-compose.yml`:
  ```bash
  sudo nano docker-compose.yml
  ```
  - `mem_limit`: e.g., `4g`
  - `cpus`: e.g., `2.0`
* Check:
  ```bash
  docker ps
  ```

### 4. Test Projects
* *tictactoe*: `npm test` or play in browser.
* *irc100Mint*:
  ```bash
  truffle test
  ```
* Others: See project READMEs.

## FAQ ❔❔

### 1️⃣ Change Files After Setup?
1. Stop containers:
   ```bash
   docker-compose down
   ```
2. Edit files:
   ```bash
   sudo nano .env
   ```
3. Inject:
   ```bash
   source .env
   ```
4. Restart:
   ```bash
   docker-compose up -d
   ```

### 2️⃣ “RPC URL not provided” Error?
1. Stop services:
   ```bash
   docker-compose down
   ```
2. Check `.env`:
   ```bash
   sudo nano .env
   ```
3. Inject:
   ```bash
   source .env
   ```
4. Restart:
   ```bash
   docker-compose up -d
   ```

### 3️⃣ How to Contribute?
1. Fork repo:
   ```bash
   git clone https://github.com/Proanant1/<project_name>
   ```
2. Create branch:
   ```bash
   git checkout -b feature/your-feature
   ```
3. Commit:
   ```bash
   git commit -m "Add feature"
   ```
4. Push & PR:
   ```bash
   git push origin feature/your-feature
   ```

### 4️⃣ Next Day Start?
1. Navigate:
   ```bash
   cd Project-Guide
   cd <project_name>
   ```
2. Inject:
   ```bash
   source .env
   ```
3. Start:
   ```bash
   docker-compose up -d
   # Or npm start, truffle migrate, etc.
   ```

### 5️⃣ Project Purposes?
* *tictactoe*: JavaScript game for learning.
* *irc100Mint*: ERC-100 token experiment.
* *nexus*: Collaborative project.
* *soundness*: Computational integrity.
* *zama-commit-test*: Commit workflow testing.

## About
Guide to setup and contribute to *Proanant1*’s GitHub projects. Code, learn, collaborate! 🌟

## Releases
No releases published

## Packages
No packages published

## Footer
© 2025 GitHub, Inc.