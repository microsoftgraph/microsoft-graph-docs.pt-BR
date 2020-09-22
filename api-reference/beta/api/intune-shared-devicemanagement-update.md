---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d829950fdcbca21145f3bda88c90833eb38831c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022411"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="90fa3-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="90fa3-103">Update deviceManagement</span></span>

<span data-ttu-id="90fa3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90fa3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90fa3-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="90fa3-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90fa3-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="90fa3-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90fa3-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90fa3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90fa3-108">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="90fa3-108">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90fa3-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90fa3-109">Prerequisites</span></span>

<span data-ttu-id="90fa3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90fa3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="90fa3-112">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="90fa3-112">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="90fa3-113">&nbsp;Tipo &nbsp; de permissão (por &nbsp; fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="90fa3-113">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="90fa3-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90fa3-114">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="90fa3-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90fa3-115">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="90fa3-116">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="90fa3-116">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="90fa3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="90fa3-118">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="90fa3-118">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="90fa3-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-119">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-120">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="90fa3-120">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="90fa3-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-121">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="90fa3-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="90fa3-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-124">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="90fa3-124">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="90fa3-125">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-125">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="90fa3-126">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="90fa3-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="90fa3-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-127">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-128">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="90fa3-128">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="90fa3-129">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-129">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-130">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="90fa3-130">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="90fa3-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-132">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="90fa3-132">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="90fa3-133">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-133">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-134">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="90fa3-134">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="90fa3-135">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-135">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-136">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="90fa3-136">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="90fa3-137">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-137">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-138">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="90fa3-138">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="90fa3-139">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-139">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-140">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="90fa3-140">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="90fa3-141">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-141">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-142">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="90fa3-142">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="90fa3-143">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-143">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-144">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="90fa3-144">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="90fa3-145">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-145">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="90fa3-146">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="90fa3-146">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="90fa3-147">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-147">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-148">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="90fa3-148">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="90fa3-149">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-149">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-150">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="90fa3-150">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="90fa3-151">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-151">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-152">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="90fa3-152">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="90fa3-153">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-153">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-154">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="90fa3-154">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="90fa3-155">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-155">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-156">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90fa3-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90fa3-157">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90fa3-157">Not supported.</span></span>|
| <span data-ttu-id="90fa3-158">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90fa3-158">Application</span></span> ||
| <span data-ttu-id="90fa3-159">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="90fa3-159">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="90fa3-160">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-160">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="90fa3-161">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="90fa3-161">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="90fa3-162">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-162">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-163">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="90fa3-163">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="90fa3-164">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-164">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-165">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="90fa3-165">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="90fa3-166">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-166">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-167">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="90fa3-167">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="90fa3-168">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-168">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="90fa3-169">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="90fa3-169">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="90fa3-170">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-170">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-171">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="90fa3-171">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="90fa3-172">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-172">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-173">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="90fa3-173">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="90fa3-174">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-174">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-175">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="90fa3-175">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="90fa3-176">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-176">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-177">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="90fa3-177">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="90fa3-178">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-178">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-179">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="90fa3-179">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="90fa3-180">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-180">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-181">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="90fa3-181">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="90fa3-182">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-182">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-183">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="90fa3-183">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="90fa3-184">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-184">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-185">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="90fa3-185">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="90fa3-186">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-186">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-187">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="90fa3-187">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="90fa3-188">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-188">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="90fa3-189">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="90fa3-189">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="90fa3-190">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-190">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-191">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="90fa3-191">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="90fa3-192">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-192">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-193">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="90fa3-193">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="90fa3-194">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-194">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-195">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="90fa3-195">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="90fa3-196">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-196">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="90fa3-197">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="90fa3-197">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="90fa3-198">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fa3-198">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90fa3-199">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90fa3-199">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="90fa3-200">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90fa3-200">Request headers</span></span>

|<span data-ttu-id="90fa3-201">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90fa3-201">Header</span></span>|<span data-ttu-id="90fa3-202">Valor</span><span class="sxs-lookup"><span data-stu-id="90fa3-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90fa3-203">Autorização</span><span class="sxs-lookup"><span data-stu-id="90fa3-203">Authorization</span></span>|<span data-ttu-id="90fa3-204">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90fa3-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90fa3-205">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90fa3-205">Accept</span></span>|<span data-ttu-id="90fa3-206">application/json</span><span class="sxs-lookup"><span data-stu-id="90fa3-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90fa3-207">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90fa3-207">Request body</span></span>

<span data-ttu-id="90fa3-208">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="90fa3-208">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="90fa3-209">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="90fa3-209">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="90fa3-210">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90fa3-210">Property</span></span>|<span data-ttu-id="90fa3-211">Tipo</span><span class="sxs-lookup"><span data-stu-id="90fa3-211">Type</span></span>|<span data-ttu-id="90fa3-212">Descrição</span><span class="sxs-lookup"><span data-stu-id="90fa3-212">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90fa3-213">id</span><span class="sxs-lookup"><span data-stu-id="90fa3-213">id</span></span>|<span data-ttu-id="90fa3-214">String</span><span class="sxs-lookup"><span data-stu-id="90fa3-214">String</span></span>|<span data-ttu-id="90fa3-215">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="90fa3-215">Unique identifier for the device.</span></span>|
|<span data-ttu-id="90fa3-216">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="90fa3-216">**Device configuration**</span></span>|
|<span data-ttu-id="90fa3-217">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="90fa3-217">intuneAccountId</span></span>|<span data-ttu-id="90fa3-218">GUID</span><span class="sxs-lookup"><span data-stu-id="90fa3-218">GUID</span></span>|<span data-ttu-id="90fa3-219">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="90fa3-219">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="90fa3-220">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="90fa3-220">legacyPcManangementEnabled</span></span>|<span data-ttu-id="90fa3-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="90fa3-221">Boolean</span></span>|<span data-ttu-id="90fa3-222">A propriedade para habilitar o gerenciamento de computador herdado não MDM gerenciado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="90fa3-222">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="90fa3-223">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90fa3-223">This property is read-only.</span></span>|
|<span data-ttu-id="90fa3-224">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="90fa3-224">maximumDepTokens</span></span>|<span data-ttu-id="90fa3-225">Int32</span><span class="sxs-lookup"><span data-stu-id="90fa3-225">Int32</span></span>|<span data-ttu-id="90fa3-226">Número máximo de tokens DEP permitidos por locatário.</span><span class="sxs-lookup"><span data-stu-id="90fa3-226">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="90fa3-227">settings</span><span class="sxs-lookup"><span data-stu-id="90fa3-227">settings</span></span>|[<span data-ttu-id="90fa3-228">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="90fa3-228">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="90fa3-229">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="90fa3-229">Account level settings.</span></span>|
|<span data-ttu-id="90fa3-230">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="90fa3-230">**Device management**</span></span>|
|<span data-ttu-id="90fa3-231">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="90fa3-231">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="90fa3-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90fa3-232">DateTimeOffset</span></span>|<span data-ttu-id="90fa3-233">A data & hora em que os dados do locatário são movidos entre o ScaleUnits.</span><span class="sxs-lookup"><span data-stu-id="90fa3-233">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="90fa3-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="90fa3-234">adminConsent</span></span>|[<span data-ttu-id="90fa3-235">adminConsent</span><span class="sxs-lookup"><span data-stu-id="90fa3-235">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="90fa3-236">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="90fa3-236">Admin consent information.</span></span>|
|<span data-ttu-id="90fa3-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="90fa3-237">deviceProtectionOverview</span></span>|[<span data-ttu-id="90fa3-238">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="90fa3-238">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="90fa3-239">Visão geral da proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="90fa3-239">Device protection overview.</span></span>|
|<span data-ttu-id="90fa3-240">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="90fa3-240">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="90fa3-241">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="90fa3-241">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="90fa3-242">Regra de limpeza de dispositivo</span><span class="sxs-lookup"><span data-stu-id="90fa3-242">Device cleanup rule</span></span>|
|<span data-ttu-id="90fa3-243">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="90fa3-243">subscriptionState</span></span>|[<span data-ttu-id="90fa3-244">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="90fa3-244">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="90fa3-245">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="90fa3-245">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="90fa3-246">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="90fa3-246">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="90fa3-247">assinaturas</span><span class="sxs-lookup"><span data-stu-id="90fa3-247">subscriptions</span></span>|[<span data-ttu-id="90fa3-248">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="90fa3-248">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="90fa3-249">Assinatura do locatário.</span><span class="sxs-lookup"><span data-stu-id="90fa3-249">Tenant's Subscription.</span></span> <span data-ttu-id="90fa3-250">Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="90fa3-250">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="90fa3-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="90fa3-251">windowsMalwareOverview</span></span>|[<span data-ttu-id="90fa3-252">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="90fa3-252">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="90fa3-253">Visão geral de malware para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="90fa3-253">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="90fa3-254">**Integração**</span><span class="sxs-lookup"><span data-stu-id="90fa3-254">**Onboarding**</span></span>|
|<span data-ttu-id="90fa3-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="90fa3-255">intuneBrand</span></span>|[<span data-ttu-id="90fa3-256">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="90fa3-256">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="90fa3-257">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="90fa3-257">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="90fa3-258">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="90fa3-258">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="90fa3-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="90fa3-259">Response</span></span>
<span data-ttu-id="90fa3-260">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90fa3-260">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90fa3-261">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90fa3-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="90fa3-262">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90fa3-262">Request</span></span>

<span data-ttu-id="90fa3-263">Veja a seguir um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="90fa3-263">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="90fa3-264">Resposta</span><span class="sxs-lookup"><span data-stu-id="90fa3-264">Response</span></span>

<span data-ttu-id="90fa3-265">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90fa3-265">Here is an example of the response.</span></span> 

<span data-ttu-id="90fa3-266">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="90fa3-266">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="90fa3-267">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="90fa3-267">Returned properties vary according to workflow and context.</span></span>

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












