# 🚀 ToDoApp — Azure Infrastructure with Terraform

> ☁️ **Infrastructure as Code | Azure | Terraform | DevOps**

A cloud infrastructure project for deploying the **ToDoApp environment on Microsoft Azure** using reusable **Terraform modules**.

---

## 🏗️ Architecture Overview

```text
                    ☁️ Microsoft Azure
                           │
                           ▼
                  📦 Resource Group
                           │
              ┌────────────┴────────────┐
              ▼                         ▼
        🌐 Virtual Network          🔐 Key Vault
              │
        ┌─────┴─────┐
        ▼           ▼
     🧩 Subnet    🌍 Public IP
        │
        ▼
     💻 Virtual Machine
        │
        ▼
     🗄️ SQL Server
        │
        ▼
     🛢️ SQL Database
```

---

## 🛠️ Technologies

| Technology             | Purpose                |
| ---------------------- | ---------------------- |
| ☁️ **Microsoft Azure** | Cloud infrastructure   |
| 🏗️ **Terraform**      | Infrastructure as Code |
| 🐙 **GitHub**          | Source code management |
| 🔧 **Git**             | Version control        |
| 🔐 **Azure Key Vault** | Secret management      |
| 🗄️ **Azure SQL**      | Database               |

---

## 📁 Project Structure

```text
ToDoApp/
│
├── 📦 Modules/
│   ├── 🔐 azurerm_key_vault/
│   ├── 🔑 azurerm_key_vault_sercret/
│   ├── 🌍 azurerm_public_ip/
│   ├── 📦 azurerm_resource_group/
│   ├── 🗄️ azurerm_sql_database/
│   ├── 🗄️ azurerm_sql_server/
│   ├── 🌐 azurerm_subnet/
│   ├── 💻 azurerm_virtual_machine/
│   └── 🌐 azurerm_virtual_network/
│
└── 🏗️ todoapp_infra/
    ├── main.tf
    ├── provider.tf
    └── .terraform.lock.hcl
```

---

## ⚡ Terraform Workflow

```text
📝 Write Terraform Code
        ↓
🔍 terraform validate
        ↓
📋 terraform plan
        ↓
🚀 terraform apply
        ↓
☁️ Azure Infrastructure
```

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Ramanstack/ToDoApp.git
cd ToDoApp/todoapp_infra
```

### 2️⃣ Initialize Terraform

```bash
terraform init
```

### 3️⃣ Validate Configuration

```bash
terraform validate
```

### 4️⃣ Create Execution Plan

```bash
terraform plan
```

### 5️⃣ Deploy Infrastructure

```bash
terraform apply
```

---

## 🔐 Security

Security practices followed in this project:

* 🔒 Terraform state files are excluded from Git
* 🔑 `.tfvars` files are excluded from Git
* 🛡️ Sensitive values are not committed to the repository
* 🔐 Azure Key Vault is used for secret management

---

## ✨ Key Features

* ♻️ **Reusable Terraform Modules**
* ☁️ **Azure Cloud Infrastructure**
* 🏗️ **Infrastructure as Code**
* 🔐 **Security-focused configuration**
* 📦 **Modular architecture**
* 🔄 **Version-controlled infrastructure**

---

## 📌 Project Status

🟢 **Active Development**

---

## 👩‍💻 Author

**Ramanstack**

⭐ If you find this project useful, feel free to explore the repository.
