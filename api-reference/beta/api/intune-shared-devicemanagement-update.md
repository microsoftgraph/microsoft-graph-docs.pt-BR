---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01d3c247d968baa2c309c81e0138c287e6f18d74
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939953"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="00e69-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="00e69-103">Update deviceManagement</span></span>

> <span data-ttu-id="00e69-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="00e69-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="00e69-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="00e69-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00e69-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00e69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00e69-107">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="00e69-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00e69-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00e69-108">Prerequisites</span></span>

<span data-ttu-id="00e69-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00e69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="00e69-111">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="00e69-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="00e69-112">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="00e69-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="00e69-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="00e69-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="00e69-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00e69-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="00e69-115">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="00e69-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="00e69-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="00e69-117">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="00e69-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="00e69-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-119">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="00e69-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="00e69-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="00e69-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="00e69-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-123">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="00e69-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="00e69-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="00e69-125">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="00e69-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="00e69-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-127">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="00e69-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="00e69-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-129">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="00e69-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="00e69-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-131">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="00e69-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="00e69-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-133">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="00e69-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="00e69-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="00e69-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="00e69-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-137">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="00e69-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="00e69-138">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-138">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-139">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="00e69-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="00e69-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-141">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="00e69-141">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="00e69-142">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-142">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-143">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="00e69-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="00e69-144">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="00e69-144">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="00e69-145">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="00e69-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="00e69-146">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-146">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-147">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="00e69-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="00e69-148">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-148">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-149">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="00e69-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="00e69-150">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-150">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-151">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="00e69-151">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="00e69-152">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-152">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-153">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="00e69-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="00e69-154">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-154">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-155">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00e69-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00e69-156">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00e69-156">Not supported.</span></span>|
| <span data-ttu-id="00e69-157">Application</span><span class="sxs-lookup"><span data-stu-id="00e69-157">Application</span></span> ||
| <span data-ttu-id="00e69-158">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="00e69-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="00e69-159">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-159">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="00e69-160">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="00e69-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="00e69-161">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-161">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-162">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="00e69-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="00e69-163">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-163">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-164">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="00e69-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="00e69-165">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-165">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-166">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="00e69-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="00e69-167">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-167">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="00e69-168">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="00e69-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="00e69-169">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-169">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-170">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="00e69-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="00e69-171">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-171">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-172">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="00e69-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="00e69-173">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-173">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-174">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="00e69-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="00e69-175">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-175">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-176">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="00e69-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="00e69-177">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-177">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-178">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="00e69-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="00e69-179">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-179">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-180">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="00e69-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="00e69-181">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-181">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-182">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="00e69-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="00e69-183">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-183">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-184">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="00e69-184">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="00e69-185">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-185">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-186">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="00e69-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="00e69-187">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="00e69-187">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="00e69-188">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="00e69-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="00e69-189">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-189">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-190">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="00e69-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="00e69-191">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-191">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-192">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="00e69-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="00e69-193">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-193">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-194">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="00e69-194">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="00e69-195">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-195">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="00e69-196">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="00e69-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="00e69-197">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e69-197">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00e69-198">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00e69-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="00e69-199">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00e69-199">Request headers</span></span>

|<span data-ttu-id="00e69-200">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00e69-200">Header</span></span>|<span data-ttu-id="00e69-201">Valor</span><span class="sxs-lookup"><span data-stu-id="00e69-201">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00e69-202">Autorização</span><span class="sxs-lookup"><span data-stu-id="00e69-202">Authorization</span></span>|<span data-ttu-id="00e69-203">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00e69-203">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00e69-204">Aceitar</span><span class="sxs-lookup"><span data-stu-id="00e69-204">Accept</span></span>|<span data-ttu-id="00e69-205">application/json</span><span class="sxs-lookup"><span data-stu-id="00e69-205">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00e69-206">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00e69-206">Request body</span></span>

<span data-ttu-id="00e69-207">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="00e69-207">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="00e69-208">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="00e69-208">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="00e69-209">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00e69-209">Property</span></span>|<span data-ttu-id="00e69-210">Tipo</span><span class="sxs-lookup"><span data-stu-id="00e69-210">Type</span></span>|<span data-ttu-id="00e69-211">Descrição</span><span class="sxs-lookup"><span data-stu-id="00e69-211">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00e69-212">id</span><span class="sxs-lookup"><span data-stu-id="00e69-212">id</span></span>|<span data-ttu-id="00e69-213">String</span><span class="sxs-lookup"><span data-stu-id="00e69-213">String</span></span>|<span data-ttu-id="00e69-214">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00e69-214">Unique identifier for the device.</span></span>|
|<span data-ttu-id="00e69-215">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="00e69-215">**Device configuration**</span></span>|
|<span data-ttu-id="00e69-216">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="00e69-216">intuneAccountId</span></span>|<span data-ttu-id="00e69-217">GUID</span><span class="sxs-lookup"><span data-stu-id="00e69-217">GUID</span></span>|<span data-ttu-id="00e69-218">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="00e69-218">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="00e69-219">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="00e69-219">legacyPcManangementEnabled</span></span>|<span data-ttu-id="00e69-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="00e69-220">Boolean</span></span>|<span data-ttu-id="00e69-221">A propriedade para habilitar o gerenciamento de computador herdado não MDM gerenciado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="00e69-221">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="00e69-222">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00e69-222">This property is read-only.</span></span>|
|<span data-ttu-id="00e69-223">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="00e69-223">maximumDepTokens</span></span>|<span data-ttu-id="00e69-224">Int32</span><span class="sxs-lookup"><span data-stu-id="00e69-224">Int32</span></span>|<span data-ttu-id="00e69-225">Número máximo de tokens DEP permitidos por locatário.</span><span class="sxs-lookup"><span data-stu-id="00e69-225">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="00e69-226">settings</span><span class="sxs-lookup"><span data-stu-id="00e69-226">settings</span></span>|[<span data-ttu-id="00e69-227">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="00e69-227">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="00e69-228">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="00e69-228">Account level settings.</span></span>|
|<span data-ttu-id="00e69-229">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="00e69-229">**Device management**</span></span>|
|<span data-ttu-id="00e69-230">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="00e69-230">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="00e69-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00e69-231">DateTimeOffset</span></span>|<span data-ttu-id="00e69-232">A data & hora em que os dados do locatário são movidos entre o ScaleUnits.</span><span class="sxs-lookup"><span data-stu-id="00e69-232">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="00e69-233">adminConsent</span><span class="sxs-lookup"><span data-stu-id="00e69-233">adminConsent</span></span>|[<span data-ttu-id="00e69-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="00e69-234">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="00e69-235">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="00e69-235">Admin consent information.</span></span>|
|<span data-ttu-id="00e69-236">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="00e69-236">deviceProtectionOverview</span></span>|[<span data-ttu-id="00e69-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="00e69-237">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="00e69-238">Visão geral da proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00e69-238">Device protection overview.</span></span>|
|<span data-ttu-id="00e69-239">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="00e69-239">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="00e69-240">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="00e69-240">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="00e69-241">Regra de limpeza de dispositivo</span><span class="sxs-lookup"><span data-stu-id="00e69-241">Device cleanup rule</span></span>|
|<span data-ttu-id="00e69-242">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="00e69-242">subscriptionState</span></span>|[<span data-ttu-id="00e69-243">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="00e69-243">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="00e69-244">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="00e69-244">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="00e69-245">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="00e69-245">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="00e69-246">assinaturas</span><span class="sxs-lookup"><span data-stu-id="00e69-246">subscriptions</span></span>|[<span data-ttu-id="00e69-247">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="00e69-247">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="00e69-248">Assinatura do locatário.</span><span class="sxs-lookup"><span data-stu-id="00e69-248">Tenant's Subscription.</span></span> <span data-ttu-id="00e69-249">Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="00e69-249">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="00e69-250">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="00e69-250">windowsMalwareOverview</span></span>|[<span data-ttu-id="00e69-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="00e69-251">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="00e69-252">Visão geral de malware para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="00e69-252">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="00e69-253">**Integração**</span><span class="sxs-lookup"><span data-stu-id="00e69-253">**Onboarding**</span></span>|
|<span data-ttu-id="00e69-254">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="00e69-254">intuneBrand</span></span>|[<span data-ttu-id="00e69-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="00e69-255">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="00e69-256">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="00e69-256">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="00e69-257">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="00e69-257">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="00e69-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="00e69-258">Response</span></span>
<span data-ttu-id="00e69-259">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00e69-259">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00e69-260">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00e69-260">Example</span></span>

### <a name="request"></a><span data-ttu-id="00e69-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00e69-261">Request</span></span>

<span data-ttu-id="00e69-262">Veja a seguir um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="00e69-262">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="00e69-263">Resposta</span><span class="sxs-lookup"><span data-stu-id="00e69-263">Response</span></span>

<span data-ttu-id="00e69-264">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00e69-264">Here is an example of the response.</span></span> 

<span data-ttu-id="00e69-265">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="00e69-265">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="00e69-266">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="00e69-266">Returned properties vary according to workflow and context.</span></span>

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











