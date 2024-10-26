# Yawlmost - Yawl Mattermost Deployment

##  🔍 Overview

Yawlmost is a deployment project for setting up Mattermost, a powerful open-source messaging platform, using Vagrant. 

This project leverages VMware as the provider for creating a robust and scalable environment consisting of manager and worker nodes configured to run in Docker Swarm mode.

## 📦 Configuration

- **Operating System**: Ubuntu 20.04 (ARM64)
- **Virtual Machines**:
   - **Leader Node**: One primary manager node (manager-1)
   - **Manager Nodes**: Two additional manager nodes (manager-2, manager-3)
   - **Worker Nodes**: Two worker nodes (worker-1, worker-2)

## 🚀 Getting Started

### ⚙️ Prerequisites

- Vagrant
- Vagrant vmware_desktop provider
- Ansible

### 🔧 Installation Steps

1. **Clone the repository:**
```shell
git clone git@github.com:Yawl-Company/yawlmost.git
cd yawlmost/mattermost
```
2. **Start the Vagrant environment:**
```shell
vagrant up
```
   
Once the setup is complete, Mattermost will be accessible at http://localhost:8065.

## 🔧 Development Setup

### 🗂 Setup Environment

Make sure your system has `poetry` and `python3.12` installed

```shell
poetry env use python3
poetry shell
poetry install
```