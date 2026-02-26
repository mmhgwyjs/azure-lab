# Azure Lab

> Please note that this project is ongoing and is meant for learning purposes. This lab focuses on Microsoft Azure cloud security, SIEM, and automation. Feedback is welcome as I refine and expand this environment.

## Objective

To build a controlled Microsoft Azure environment that allows hands-on exploration of cloud security, Microsoft Defender, Sentinel SIEM, and automation. The lab will serve as a foundation for creating detection rules, incident response workflows, and secure cloud architectures.

---

## Initial Setup

This section outlines the core infrastructure and initial configuration for the Azure Lab.

### 1. Azure Subscription and Resource Group

- Sign up for a free or trial [Microsoft Azure account](https://azure.microsoft.com/free/).  
- Create a dedicated resource group to contain all lab resources:  
Resource Group Name: RG-AzureLab
Location: Your preferred Azure region


- Organize resources for clarity and cost control.

---

### 2. Virtual Machine Deployment

- Deploy Windows 10/11 VMs for endpoint testing.  
- Deploy Linux VMs if needed for cross-platform scenarios.  
- VM sizes can be B1s or other low-cost tiers to minimize expenses.  

> These VMs serve as test environments for Defender onboarding, attack simulation, and SIEM data ingestion.

---

### 3. Microsoft Defender Integration

- Enable **Microsoft Defender for Endpoint** on Windows VMs.  
- Enable **Microsoft Defender for Cloud** for the resource group.  
- Review secure score recommendations and implement baseline policies.  

> The Defender suite will be the primary source of alerts and security telemetry for the lab.

---

### 4. Microsoft Sentinel Setup

- Create a **Log Analytics Workspace** and link it to your resource group.  
- Deploy **Microsoft Sentinel**.  
- Connect data sources:
  - Security Events (Windows/Linux VMs)
  - Azure Activity Logs
  - Entra ID logs (Azure AD)
- Verify data ingestion and build a simple dashboard to visualize alerts.

---

### 5. Baseline Network and Identity Configuration

- Set up **Azure AD** (Entra ID) for identity management.  
- Configure RBAC roles to simulate typical tenant permissions.  
- Apply **basic conditional access policies** for MFA and sign-in controls.  
- Set up NSGs and basic network segmentation.

> These steps ensure that your lab mimics a realistic enterprise cloud environment.

---
