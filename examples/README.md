# terraform-az-fk-bastion examples

This directory contains reusable **Terraform / OpenTofu examples** built around the `terraform-az-fk-bastion` module.

It is part of the **[FoggyKitchen.com training ecosystem](https://foggykitchen.com/courses/azure-fundamentals-terraform-course/)** and is designed to demonstrate **secure operator access patterns** for private Azure workloads.

---

## 🎯 Purpose

The goal of this directory is to provide **clear, educational, and runnable reference examples** for using **Azure Bastion** with real workload topologies.

It focuses on:

- Bastion-based access to **private workloads without public IPs**
- Progressive examples that highlight **networking and security boundaries**
- Practical integration with other FoggyKitchen modules

Each example is intended to be applied **independently** for learning and reuse.

---

## ✨ What the examples cover

The examples in this directory demonstrate:

- A **private Linux VM** accessed through Azure Bastion
- A **private AKS cluster** accessed through Bastion and a jump VM
- NAT Gateway-based **outbound egress**
- NSG-based control at the **NIC and subnet boundaries**

Each example includes:

- Terraform / OpenTofu configuration (`.tf`)
- A focused `README.md` explaining the architectural goal
- A **fully runnable deployment** with no placeholders or mock resources

---

## 📂 Example Overview

| Example | Title | Key Topics |
|--------|-------|------------|
| `01` | **Private VM with Bastion Access** | AzureBastionSubnet, NIC-level NSG, Bastion tunneling |
| `02` | **Private AKS with Bastion Access** | Private AKS, jump VM, NAT Gateway egress, Bastion tunneling |

---

## 📁 Directory Structure

```bash
examples/
├── 01_private_vm_with_bastion_access/
│   └── README.md
├── 02_private_aks_with_bastion_access/
│   └── README.md
└── README.md
```

---

## 🚀 Example Usage

```bash
cd examples/01_private_vm_with_bastion_access
tofu init
tofu plan
tofu apply
```

---

## 🧩 Related Modules & Training

- [terraform-az-fk-bastion](https://github.com/mlinxfeld/terraform-az-fk-bastion)
- [terraform-az-fk-vnet](https://github.com/foggykitchen/terraform-az-fk-vnet)
- [terraform-az-fk-nsg](https://github.com/mlinxfeld/terraform-az-fk-nsg)
- [terraform-az-fk-compute](https://github.com/foggykitchen/terraform-az-fk-compute)
- [terraform-az-fk-natgw](https://github.com/mlinxfeld/terraform-az-fk-natgw)
- [terraform-az-fk-loadbalancer](https://github.com/mlinxfeld/terraform-az-fk-loadbalancer)
- [terraform-az-fk-disk](https://github.com/mlinxfeld/terraform-az-fk-disk)
- [terraform-az-fk-storage](https://github.com/foggykitchen/terraform-az-fk-storage)
- [terraform-az-fk-aks](https://github.com/mlinxfeld/terraform-az-fk-aks)

---

## 🪪 License

Licensed under the **Universal Permissive License (UPL), Version 1.0**.  
See [LICENSE](../LICENSE) for details.

---

© 2026 FoggyKitchen.com — Cloud. Code. Clarity.
