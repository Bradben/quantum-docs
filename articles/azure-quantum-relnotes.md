---
author: geduardo
description: Learn about the latest updates of the Azure Quantum service.
ms.author: v-edsanc
ms.date: 02/01/2021
ms.service: azure-quantum
ms.subservice: core
ms.topic: article
title: Azure Quantum Release Notes
uid: microsoft.quantum.azure.relnotes
---

# Azure Quantum release notes

### 2021-2-22: SDK Quota List Support
- The azure-quantum python SDK now exposes a workspace-level method for listing all quotas that effect the workspace and their current meter values.

### 2021-2-22: Enable quantum providers in quantum workspaces via Azure CLI
- A map of targets to providers and plansis created.

### 2021-02-01: New public repository for document contributions
- Document contributions can now made to our new public GitHub repository, https://github.com/MicrosoftDocs/quantum-docs. 

### 2020-11-23: Added `create` and `delete` commands for `az quantum workspace` group
- The create command is currently limited because it doesn't add providers to a new quantum workspace, and those need to be added from the portal. The limitation will be removed in a future update.

### 2020-10-26: Adapted QCI translation to the latest spec 
- Added support for latest conditional syntax, reset patterns, and gate instructions.

### 2020-10-26: Capability verification for references
- Each error is linked to a piece of source code, so that users can adapt their code in a way that eliminates the issue without significant effort.

### 2020-10-26: Added `delete` commands for `az quantum workspace` group

### 2020-10-26: Improved Python SDK `Workspace` constructor 
- The constructor of the `Workspace` in the Python SDK now has an option to take the resource ID of the Azure Quantum workspace, which is shown on the workspace page in the Azure Portal, rather than requiring the subscription ID, resource group name, and workspace name.

### 2020-08-31: Bug fixes & job scheduling perf improvements
- Fixed a bug where the `all_betas` parameter returned from parameter-free solvers was named `betas`

### 2020-08-25: Job Shop optimization sample now available
[The sample for job shop optimization is now available in the Samples folder](https://github.com/microsoft/qio-samples). This complete sample teaches:

- What the job shop scheduling problem is and why it is important
- How to represent problem terms mathematically
- How to build penalty functions to represent problem constraints
- How to transform these mathematical functions into code using the Python SDK for optimization
- How to submit problem terms to Azure Quantum
- How to interpret the results

### 2020-08-24: Parameter-free solvers now return parameters
A highly requested feature – the ability to see the parameters chosen by parameter-free solvers – is now available. When running a problem against a parameter-free solver you will now see a “parameters” object returned in the job result. These parameters were used to generate the returned configuration.

```json
{
    "configuration": {
        "0": 1,
        "1": -1,
        "2": 1
    },
    "cost": 0.4,
    "parameters": {
        "all_betas": [
            0.1,
            0.2,
            0.3
        ],
        "replicas": 3,
        "sweeps": 100
    }
}
```

No SDK updates are needed to take advantage of this update.
