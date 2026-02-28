# Azure Lab

> Please note that this project is ongoing and is meant for learning purposes. This lab focuses on Microsoft Azure cloud security, SIEM, and automation. Feedback is welcome as I refine and expand this environment.

## Objective

To build a controlled Microsoft Azure environment that allows hands-on exploration of cloud security, Microsoft Defender, Sentinel SIEM, and automation. The lab will serve as a foundation for creating detection rules, incident response workflows, and secure cloud architectures.

---

## Initial Setup

This section outlines the core infrastructure and initial configuration for the Azure Lab.

### 1. Azure Subscription 

- Sign up for a free or trial [Microsoft Azure account](https://azure.microsoft.com/free/)
  
  <img width="1433" height="893" alt="image" src="https://github.com/user-attachments/assets/b59a8625-b232-49b0-8fd4-3f4401a11f75" />

  <img width="1704" height="898" alt="image" src="https://github.com/user-attachments/assets/8ce8dfd0-611f-4dc5-b646-3f3ea2d5e761" />

### 2. Resource Group

- Create a dedicated resource group to contain all lab resources:
  
  Resource Group Name: RG-AzureLab

  Location: Your preferred Azure region

  <img width="2549" height="1081" alt="image" src="https://github.com/user-attachments/assets/3ac60e0b-9ea0-46a4-8155-b13a87cbe315" />
  
  <img width="984" height="492" alt="image" src="https://github.com/user-attachments/assets/6c243fbe-4288-4580-a830-1a36a7f89064" />

- Create a budget alert (Cost Management > Monitoring > Budgets)

  <img width="1067" height="1024" alt="image" src="https://github.com/user-attachments/assets/d58e9fd5-85f1-405b-a0ee-bfc03c8645d3" />

### 3. Log Analytics Workspace

- Create a dedicated log analytics workspace:

  Resource Group Name: LA-AzureLab

  Location: Your preferred Azure region

  <img width="868" height="770" alt="image" src="https://github.com/user-attachments/assets/cb79e9f4-2113-4eed-a066-07078e9b50a2" />

### 4. Microsoft Sentinel

- Create Microsoft Sentinel and select the log analytics created earlier

  <img width="1920" height="970" alt="image" src="https://github.com/user-attachments/assets/fe5a4b58-418d-49ba-a1a8-1ad771585038" />

  <img width="2283" height="313" alt="image" src="https://github.com/user-attachments/assets/623e0caa-2561-4909-a23c-0c5bd1dc2ee1" />

### 5. Data Connectors

- Install and enable data connectors (Microsoft Sentinel > Configuration > Data Connectors)

  <img width="1520" height="1025" alt="image" src="https://github.com/user-attachments/assets/34fbb01d-66ab-4cae-89d9-731b06501372" />

  <img width="2066" height="672" alt="image" src="https://github.com/user-attachments/assets/fd4a6f1a-edd0-4053-b97b-62c0a27e7d67" />

### 5. Entra ID (Azure AD)

- Configure Entra ID users and roles (Microsoft Entra ID > Users)

  <img width="1539" height="518" alt="image" src="https://github.com/user-attachments/assets/a1a00945-3d28-468e-a27c-16461ec3f963" />

### 6. Virtual Machine

- Deploy virtual machine 

  <img width="2023" height="1011" alt="image" src="https://github.com/user-attachments/assets/d57aa64c-7e79-4a73-a5b7-c4189e5102d1" />

---
