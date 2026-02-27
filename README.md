# Azure Lab

> Please note that this project is ongoing and is meant for learning purposes. This lab focuses on Microsoft Azure cloud security, SIEM, and automation. Feedback is welcome as I refine and expand this environment.

## Objective

To build a controlled Microsoft Azure environment that allows hands-on exploration of cloud security, Microsoft Defender, Sentinel SIEM, and automation. The lab will serve as a foundation for creating detection rules, incident response workflows, and secure cloud architectures.

---

## Initial Setup

This section outlines the core infrastructure and initial configuration for the Azure Lab.

### 1. Azure Subscription and Resource Group

- Sign up for a free or trial [Microsoft Azure account](https://azure.microsoft.com/free/).
  <img width="1433" height="893" alt="image" src="https://github.com/user-attachments/assets/b59a8625-b232-49b0-8fd4-3f4401a11f75" />

  <img width="1704" height="898" alt="image" src="https://github.com/user-attachments/assets/8ce8dfd0-611f-4dc5-b646-3f3ea2d5e761" />


- Create a dedicated resource group to contain all lab resources:
  
  Resource Group Name: RG-AzureLab

  Location: Your preferred Azure region

  <img width="2549" height="1081" alt="image" src="https://github.com/user-attachments/assets/3ac60e0b-9ea0-46a4-8155-b13a87cbe315" />
  
  <img width="984" height="492" alt="image" src="https://github.com/user-attachments/assets/6c243fbe-4288-4580-a830-1a36a7f89064" />

- Create a budget alert (Cost Management > Monitoring > Budgets)

  <img width="1067" height="1024" alt="image" src="https://github.com/user-attachments/assets/d58e9fd5-85f1-405b-a0ee-bfc03c8645d3" />




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
