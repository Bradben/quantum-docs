---
author: bradben
description: Load and run a Jupyter Notebook with the device data from Microsoft's research into a scaled quantum machines using topological qubits.
ms.date: 11/14/2022
ms.author: brbenefield
ms.service: azure-quantum
ms.subservice: qdk
ms.topic: overview
no-loc: ['Q#', '$$v', Quantum Development Kit]
title: Microsoft's quantum machine
uid: microsoft.quantum.overview.ms-machine
---

# Microsoft's quantum machine

Microsoft is on the path to deliver a quantum machine as part of the Azure Quantum service. You can read more about this journey on [this blog](https://cloudblogs.microsoft.com/quantum/2022/11/17/microsofts-quantum-machine-new-data-available-today/). This is part of a comprehensive plan to empower innovators with quantum solutions for breakthrough impact.

In 2022, Microsoft had a major scientific breakthrough that cleared a significant hurdle toward building a scaled quantum machine with topological qubits. While engineering challenges remain, this new discovery demonstrates a fundamental building block for its approach to scaled quantum computing. For more information about this scientific discovery, read the [blog](https://www.microsoft.com/research/blog/microsoft-has-demonstrated-the-underlying-physics-required-to-create-a-new-kind-of-qubit/), watch a [video](https://www.youtube.com/watch?v=Q8CHms4ixYc), or read the [preprint](https://arxiv.org/abs/2207.02472) of the paper.

The Azure Quantum team has created a Jupyter Notebook which performs all the analysis and generates the plots that appear in the paper. All you need to load and run the notebook is a free Azure account.

## Create an Azure account

To start, you'll need an Azure account with an active subscription. You can register for free and sign up for a [pay-as-you-go subscription](https://azure.microsoft.com/pricing/purchase-options/pay-as-you-go), and run the Jupyter Notebook without incurring any charges.

> [!NOTE]
> If you have any questions regarding the workspace creation process or run into any issue at any point using Azure Quantum, bookmark [Azure Quantum office hours](https://aka.ms/AQ/OfficeHours) and join our open office hours every Thursday 8∶30 AM Pacific Time.

## Create an Azure Quantum workspace

To create an Azure Quantum workspace, follow these steps.

1. Sign in to the [Azure portal](https://portal.azure.com), using the credentials for your Azure subscription.

1. Select **Create a resource** and then search for **Azure Quantum**. On the results page, you should see a tile for the **Azure Quantum** service.

1. Select **Azure Quantum** and then select  **Create**. This opens a form to create a workspace.

1. Select a subscription to associate with the new workspace.

1. Select **Quick create**
1. Enter a name for the workspace.
1. Select the region for the workspace.
1. Click **Create**.
1. Deployment of your workspace may take a few minutes. When the deployment is complete, select **Go to resource**. 

## View a Jupyter Notebook

There are three notebooks available to review:

- Analysis of device data from preprint paper
- First stage of topological gap protocol
- Second stage of topological gap protocol 

To view and run a notebook: 

1. In your new workspace, select **Notebooks** and then select **Topological quantum computing**. 
1. Select your desired notebook, and select **Copy to my notebooks**.

    :::image type="content" source="media/ms-machine-copy-notebook_2.png" alt-text="Copy sample notebook.":::

1. To run all the cells in the notebook, select **Run all** (or **Alt-R**) at the top of the notebook. To step through the notebook cell-by-cell, select **Run cell** (or **Ctrl+Enter**) next to each notebook cell. 


## Next Steps

- [What is Azure Quantum?](xref:microsoft.quantum.azure-quantum-overview)
- [What are the Q# programming language and Quantum Development Kit (QDK)?](xref:microsoft.quantum.overview.q-sharp)
- [Quickstart: Submit a circuit with Qiskit using an Azure Quantum notebook](xref:microsoft.quantum.quickstarts.computing.qiskit.portal)
- [Quickstart: Solve an optimization problem using an Azure Quantum notebook](xref:microsoft.quantum.quickstarts.optimization.qio.portal)
