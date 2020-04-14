---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75bca64ce38779e0e9c1f905525414e5b0308f81
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390049"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="cd435-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="cd435-103">Update deviceManagement</span></span>

<span data-ttu-id="cd435-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd435-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd435-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd435-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cd435-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd435-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd435-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd435-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd435-108">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cd435-108">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd435-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd435-109">Prerequisites</span></span>

<span data-ttu-id="cd435-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd435-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cd435-112">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="cd435-112">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="cd435-113">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="cd435-113">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="cd435-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cd435-114">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="cd435-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd435-115">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="cd435-116">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="cd435-116">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="cd435-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-117">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="cd435-118">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="cd435-118">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="cd435-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-119">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-120">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="cd435-120">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="cd435-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-121">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="cd435-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="cd435-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-124">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="cd435-124">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="cd435-125">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-125">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="cd435-126">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="cd435-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="cd435-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-127">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-128">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="cd435-128">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="cd435-129">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-129">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-130">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="cd435-130">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="cd435-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-132">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="cd435-132">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="cd435-133">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-133">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-134">&nbsp;&nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="cd435-134">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="cd435-135">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-135">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-136">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="cd435-136">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="cd435-137">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-137">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-138">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="cd435-138">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="cd435-139">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-139">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-140">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="cd435-140">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="cd435-141">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-141">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-142">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="cd435-142">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="cd435-143">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-143">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-144">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="cd435-144">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="cd435-145">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd435-145">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="cd435-146">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="cd435-146">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="cd435-147">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-147">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-148">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="cd435-148">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="cd435-149">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-149">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-150">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="cd435-150">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="cd435-151">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-151">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-152">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="cd435-152">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="cd435-153">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-153">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-154">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="cd435-154">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="cd435-155">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-155">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-156">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd435-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd435-157">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd435-157">Not supported.</span></span>|
| <span data-ttu-id="cd435-158">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd435-158">Application</span></span> ||
| <span data-ttu-id="cd435-159">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="cd435-159">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="cd435-160">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-160">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="cd435-161">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="cd435-161">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="cd435-162">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-162">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-163">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="cd435-163">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="cd435-164">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-164">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-165">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="cd435-165">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="cd435-166">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-166">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-167">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="cd435-167">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="cd435-168">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-168">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="cd435-169">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="cd435-169">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="cd435-170">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-170">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-171">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="cd435-171">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="cd435-172">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-172">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-173">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="cd435-173">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="cd435-174">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-174">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-175">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="cd435-175">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="cd435-176">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-176">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-177">&nbsp;&nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="cd435-177">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="cd435-178">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-178">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-179">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="cd435-179">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="cd435-180">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-180">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-181">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="cd435-181">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="cd435-182">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-182">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-183">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="cd435-183">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="cd435-184">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-184">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-185">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="cd435-185">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="cd435-186">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-186">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-187">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="cd435-187">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="cd435-188">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd435-188">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="cd435-189">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="cd435-189">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="cd435-190">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-190">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-191">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="cd435-191">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="cd435-192">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-192">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-193">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="cd435-193">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="cd435-194">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-194">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-195">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="cd435-195">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="cd435-196">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-196">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="cd435-197">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="cd435-197">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="cd435-198">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd435-198">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd435-199">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd435-199">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="cd435-200">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd435-200">Request headers</span></span>

|<span data-ttu-id="cd435-201">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd435-201">Header</span></span>|<span data-ttu-id="cd435-202">Valor</span><span class="sxs-lookup"><span data-stu-id="cd435-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd435-203">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd435-203">Authorization</span></span>|<span data-ttu-id="cd435-204">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd435-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd435-205">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd435-205">Accept</span></span>|<span data-ttu-id="cd435-206">application/json</span><span class="sxs-lookup"><span data-stu-id="cd435-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd435-207">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd435-207">Request body</span></span>

<span data-ttu-id="cd435-208">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cd435-208">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="cd435-209">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="cd435-209">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="cd435-210">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd435-210">Property</span></span>|<span data-ttu-id="cd435-211">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd435-211">Type</span></span>|<span data-ttu-id="cd435-212">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd435-212">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd435-213">id</span><span class="sxs-lookup"><span data-stu-id="cd435-213">id</span></span>|<span data-ttu-id="cd435-214">String</span><span class="sxs-lookup"><span data-stu-id="cd435-214">String</span></span>|<span data-ttu-id="cd435-215">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd435-215">Unique identifier for the device.</span></span>|
|<span data-ttu-id="cd435-216">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="cd435-216">**Device configuration**</span></span>|
|<span data-ttu-id="cd435-217">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="cd435-217">intuneAccountId</span></span>|<span data-ttu-id="cd435-218">GUID</span><span class="sxs-lookup"><span data-stu-id="cd435-218">GUID</span></span>|<span data-ttu-id="cd435-219">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="cd435-219">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="cd435-220">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="cd435-220">legacyPcManangementEnabled</span></span>|<span data-ttu-id="cd435-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd435-221">Boolean</span></span>|<span data-ttu-id="cd435-222">A propriedade para habilitar o gerenciamento de computador herdado não MDM gerenciado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="cd435-222">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="cd435-223">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd435-223">This property is read-only.</span></span>|
|<span data-ttu-id="cd435-224">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="cd435-224">maximumDepTokens</span></span>|<span data-ttu-id="cd435-225">Int32</span><span class="sxs-lookup"><span data-stu-id="cd435-225">Int32</span></span>|<span data-ttu-id="cd435-226">Número máximo de tokens DEP permitidos por locatário.</span><span class="sxs-lookup"><span data-stu-id="cd435-226">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="cd435-227">settings</span><span class="sxs-lookup"><span data-stu-id="cd435-227">settings</span></span>|[<span data-ttu-id="cd435-228">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="cd435-228">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="cd435-229">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="cd435-229">Account level settings.</span></span>|
|<span data-ttu-id="cd435-230">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="cd435-230">**Device management**</span></span>|
|<span data-ttu-id="cd435-231">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="cd435-231">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="cd435-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd435-232">DateTimeOffset</span></span>|<span data-ttu-id="cd435-233">A data & hora em que os dados do locatário são movidos entre o ScaleUnits.</span><span class="sxs-lookup"><span data-stu-id="cd435-233">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="cd435-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="cd435-234">adminConsent</span></span>|[<span data-ttu-id="cd435-235">adminConsent</span><span class="sxs-lookup"><span data-stu-id="cd435-235">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="cd435-236">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="cd435-236">Admin consent information.</span></span>|
|<span data-ttu-id="cd435-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="cd435-237">deviceProtectionOverview</span></span>|[<span data-ttu-id="cd435-238">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="cd435-238">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="cd435-239">Visão geral da proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cd435-239">Device protection overview.</span></span>|
|<span data-ttu-id="cd435-240">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="cd435-240">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="cd435-241">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="cd435-241">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="cd435-242">Regra de limpeza de dispositivo</span><span class="sxs-lookup"><span data-stu-id="cd435-242">Device cleanup rule</span></span>|
|<span data-ttu-id="cd435-243">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="cd435-243">subscriptionState</span></span>|[<span data-ttu-id="cd435-244">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="cd435-244">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="cd435-245">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="cd435-245">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="cd435-246">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="cd435-246">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="cd435-247">assinaturas</span><span class="sxs-lookup"><span data-stu-id="cd435-247">subscriptions</span></span>|[<span data-ttu-id="cd435-248">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="cd435-248">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="cd435-249">Assinatura do locatário.</span><span class="sxs-lookup"><span data-stu-id="cd435-249">Tenant's Subscription.</span></span> <span data-ttu-id="cd435-250">Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="cd435-250">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="cd435-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="cd435-251">windowsMalwareOverview</span></span>|[<span data-ttu-id="cd435-252">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="cd435-252">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="cd435-253">Visão geral de malware para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="cd435-253">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="cd435-254">**Integração**</span><span class="sxs-lookup"><span data-stu-id="cd435-254">**Onboarding**</span></span>|
|<span data-ttu-id="cd435-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="cd435-255">intuneBrand</span></span>|[<span data-ttu-id="cd435-256">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="cd435-256">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="cd435-257">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="cd435-257">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="cd435-258">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="cd435-258">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="cd435-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd435-259">Response</span></span>
<span data-ttu-id="cd435-260">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd435-260">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd435-261">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd435-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd435-262">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd435-262">Request</span></span>

<span data-ttu-id="cd435-263">Veja a seguir um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="cd435-263">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="cd435-264">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd435-264">Response</span></span>

<span data-ttu-id="cd435-265">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd435-265">Here is an example of the response.</span></span> 

<span data-ttu-id="cd435-266">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="cd435-266">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cd435-267">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="cd435-267">Returned properties vary according to workflow and context.</span></span>

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









