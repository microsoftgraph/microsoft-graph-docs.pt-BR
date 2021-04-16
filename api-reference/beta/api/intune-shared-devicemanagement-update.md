---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80f5fc4065d8db2f0bbb7659f244a14c9ef9331d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867522"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="ce6e0-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ce6e0-103">Update deviceManagement</span></span>

<span data-ttu-id="ce6e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce6e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce6e0-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ce6e0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce6e0-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce6e0-108">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ce6e0-108">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce6e0-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ce6e0-109">Prerequisites</span></span>

<span data-ttu-id="ce6e0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce6e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ce6e0-112">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-112">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="ce6e0-113">Tipo &nbsp; de &nbsp; permissão (por fluxo de &nbsp; trabalho)</span><span class="sxs-lookup"><span data-stu-id="ce6e0-113">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="ce6e0-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ce6e0-114">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="ce6e0-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce6e0-115">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="ce6e0-116">&nbsp;&nbsp; **Android for Work**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-116">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="ce6e0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="ce6e0-118">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-118">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="ce6e0-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-119">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-120">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-120">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="ce6e0-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-121">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ce6e0-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-124">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-124">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="ce6e0-125">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-125">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="ce6e0-126">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ce6e0-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-127">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-128">&nbsp;&nbsp; **SIM Eletrônico**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-128">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="ce6e0-129">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-129">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-130">&nbsp;&nbsp; **Inscrição**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-130">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ce6e0-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-132">&nbsp;&nbsp; **Esgrima**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-132">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="ce6e0-133">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-133">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-134">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-134">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="ce6e0-135">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-135">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-136">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-136">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="ce6e0-137">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-137">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-138">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-138">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ce6e0-139">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-139">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-140">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-140">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ce6e0-141">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-141">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-142">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-142">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="ce6e0-143">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-143">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-144">&nbsp; &nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-144">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="ce6e0-145">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-145">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ce6e0-146">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-146">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="ce6e0-147">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-147">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-148">&nbsp;&nbsp; **Atualização de Software**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-148">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="ce6e0-149">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-149">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-150">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-150">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="ce6e0-151">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-151">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-152">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-152">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="ce6e0-153">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-153">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-154">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-154">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="ce6e0-155">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-155">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-156">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce6e0-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce6e0-157">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-157">Not supported.</span></span>|
| <span data-ttu-id="ce6e0-158">Application</span><span class="sxs-lookup"><span data-stu-id="ce6e0-158">Application</span></span> ||
| <span data-ttu-id="ce6e0-159">&nbsp;&nbsp; **Android for Work**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-159">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="ce6e0-160">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-160">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="ce6e0-161">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-161">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="ce6e0-162">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-162">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-163">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-163">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="ce6e0-164">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-164">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-165">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-165">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ce6e0-166">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-166">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-167">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-167">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="ce6e0-168">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-168">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="ce6e0-169">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-169">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ce6e0-170">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-170">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-171">&nbsp;&nbsp; **SIM Eletrônico**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-171">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="ce6e0-172">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-172">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-173">&nbsp;&nbsp; **Inscrição**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-173">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ce6e0-174">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-174">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-175">&nbsp;&nbsp; **Esgrima**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-175">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="ce6e0-176">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-176">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-177">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-177">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="ce6e0-178">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-178">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-179">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-179">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="ce6e0-180">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-180">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-181">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-181">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ce6e0-182">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-182">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-183">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-183">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ce6e0-184">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-184">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-185">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-185">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="ce6e0-186">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-186">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-187">&nbsp; &nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-187">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="ce6e0-188">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-188">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ce6e0-189">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-189">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="ce6e0-190">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-190">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-191">&nbsp;&nbsp; **Atualização de Software**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-191">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="ce6e0-192">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-192">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-193">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-193">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="ce6e0-194">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-194">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-195">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-195">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="ce6e0-196">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-196">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="ce6e0-197">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-197">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="ce6e0-198">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6e0-198">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce6e0-199">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce6e0-199">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="ce6e0-200">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce6e0-200">Request headers</span></span>

|<span data-ttu-id="ce6e0-201">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce6e0-201">Header</span></span>|<span data-ttu-id="ce6e0-202">Valor</span><span class="sxs-lookup"><span data-stu-id="ce6e0-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce6e0-203">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce6e0-203">Authorization</span></span>|<span data-ttu-id="ce6e0-204">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce6e0-205">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ce6e0-205">Accept</span></span>|<span data-ttu-id="ce6e0-206">application/json</span><span class="sxs-lookup"><span data-stu-id="ce6e0-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce6e0-207">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce6e0-207">Request body</span></span>

<span data-ttu-id="ce6e0-208">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ce6e0-208">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="ce6e0-209">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ce6e0-209">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="ce6e0-210">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce6e0-210">Property</span></span>|<span data-ttu-id="ce6e0-211">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce6e0-211">Type</span></span>|<span data-ttu-id="ce6e0-212">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce6e0-212">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce6e0-213">id</span><span class="sxs-lookup"><span data-stu-id="ce6e0-213">id</span></span>|<span data-ttu-id="ce6e0-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce6e0-214">String</span></span>|<span data-ttu-id="ce6e0-215">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-215">Unique identifier for the device.</span></span>|
|<span data-ttu-id="ce6e0-216">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-216">**Device configuration**</span></span>|
|<span data-ttu-id="ce6e0-217">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="ce6e0-217">intuneAccountId</span></span>|<span data-ttu-id="ce6e0-218">GUID</span><span class="sxs-lookup"><span data-stu-id="ce6e0-218">GUID</span></span>|<span data-ttu-id="ce6e0-219">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="ce6e0-219">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="ce6e0-220">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="ce6e0-220">legacyPcManangementEnabled</span></span>|<span data-ttu-id="ce6e0-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6e0-221">Boolean</span></span>|<span data-ttu-id="ce6e0-222">A propriedade para habilitar o gerenciamento de computador herdado não-MDM gerenciado para essa conta.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-222">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="ce6e0-223">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-223">This property is read-only.</span></span>|
|<span data-ttu-id="ce6e0-224">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="ce6e0-224">maximumDepTokens</span></span>|<span data-ttu-id="ce6e0-225">Int32</span><span class="sxs-lookup"><span data-stu-id="ce6e0-225">Int32</span></span>|<span data-ttu-id="ce6e0-226">Número máximo de tokens DEP permitidos por locatário.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-226">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="ce6e0-227">settings</span><span class="sxs-lookup"><span data-stu-id="ce6e0-227">settings</span></span>|[<span data-ttu-id="ce6e0-228">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="ce6e0-228">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="ce6e0-229">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-229">Account level settings.</span></span>|
|<span data-ttu-id="ce6e0-230">**Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-230">**Device management**</span></span>|
|<span data-ttu-id="ce6e0-231">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="ce6e0-231">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="ce6e0-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce6e0-232">DateTimeOffset</span></span>|<span data-ttu-id="ce6e0-233">A data & hora em que os dados do locatário foram movidos entre as unidades de escala.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-233">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="ce6e0-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="ce6e0-234">adminConsent</span></span>|[<span data-ttu-id="ce6e0-235">adminConsent</span><span class="sxs-lookup"><span data-stu-id="ce6e0-235">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="ce6e0-236">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-236">Admin consent information.</span></span>|
|<span data-ttu-id="ce6e0-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="ce6e0-237">deviceProtectionOverview</span></span>|[<span data-ttu-id="ce6e0-238">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="ce6e0-238">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="ce6e0-239">Visão geral da proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-239">Device protection overview.</span></span>|
|<span data-ttu-id="ce6e0-240">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="ce6e0-240">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="ce6e0-241">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="ce6e0-241">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="ce6e0-242">Regra de limpeza de dispositivo</span><span class="sxs-lookup"><span data-stu-id="ce6e0-242">Device cleanup rule</span></span>|
|<span data-ttu-id="ce6e0-243">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="ce6e0-243">subscriptionState</span></span>|[<span data-ttu-id="ce6e0-244">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="ce6e0-244">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="ce6e0-245">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-245">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="ce6e0-246">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-246">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="ce6e0-247">assinaturas</span><span class="sxs-lookup"><span data-stu-id="ce6e0-247">subscriptions</span></span>|[<span data-ttu-id="ce6e0-248">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="ce6e0-248">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="ce6e0-249">Assinatura do locatário.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-249">Tenant's Subscription.</span></span> <span data-ttu-id="ce6e0-250">Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-250">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="ce6e0-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="ce6e0-251">windowsMalwareOverview</span></span>|[<span data-ttu-id="ce6e0-252">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="ce6e0-252">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="ce6e0-253">Visão geral do malware para dispositivos windows.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-253">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="ce6e0-254">**Integração**</span><span class="sxs-lookup"><span data-stu-id="ce6e0-254">**Onboarding**</span></span>|
|<span data-ttu-id="ce6e0-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="ce6e0-255">intuneBrand</span></span>|[<span data-ttu-id="ce6e0-256">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="ce6e0-256">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="ce6e0-257">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-257">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="ce6e0-258">O suporte à propriedade request body varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-258">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="ce6e0-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce6e0-259">Response</span></span>
<span data-ttu-id="ce6e0-260">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-260">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce6e0-261">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce6e0-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce6e0-262">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce6e0-262">Request</span></span>

<span data-ttu-id="ce6e0-263">Veja um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="ce6e0-263">Here is an example of a request following the device management workflow:</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a><span data-ttu-id="ce6e0-264">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce6e0-264">Response</span></span>

<span data-ttu-id="ce6e0-265">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-265">Here is an example of the response.</span></span> 

<span data-ttu-id="ce6e0-266">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-266">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ce6e0-267">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="ce6e0-267">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```










