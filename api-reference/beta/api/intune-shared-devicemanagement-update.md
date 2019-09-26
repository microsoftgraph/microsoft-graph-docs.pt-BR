---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8f8b3171eaabedfa085f7685b2f4f7aa1ad87a3
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194590"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="c664a-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c664a-103">Update deviceManagement</span></span>

> <span data-ttu-id="c664a-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c664a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c664a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c664a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c664a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c664a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c664a-107">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c664a-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c664a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c664a-108">Prerequisites</span></span>

<span data-ttu-id="c664a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c664a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c664a-111">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c664a-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="c664a-112">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="c664a-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="c664a-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c664a-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="c664a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c664a-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="c664a-115">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="c664a-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="c664a-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="c664a-117">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="c664a-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="c664a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-119">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="c664a-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="c664a-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c664a-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c664a-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-123">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c664a-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="c664a-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c664a-125">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="c664a-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c664a-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-127">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="c664a-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="c664a-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-129">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="c664a-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c664a-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-131">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="c664a-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="c664a-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-133">&nbsp;&nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="c664a-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="c664a-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="c664a-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="c664a-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-137">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="c664a-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c664a-138">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-138">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-139">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c664a-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c664a-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-141">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="c664a-141">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="c664a-142">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-142">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-143">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="c664a-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="c664a-144">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c664a-144">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c664a-145">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="c664a-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="c664a-146">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-146">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-147">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="c664a-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c664a-148">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-148">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-149">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="c664a-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="c664a-150">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-150">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-151">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="c664a-151">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="c664a-152">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-152">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-153">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="c664a-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="c664a-154">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-154">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-155">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c664a-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c664a-156">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c664a-156">Not supported.</span></span>|
| <span data-ttu-id="c664a-157">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c664a-157">Application</span></span> ||
| <span data-ttu-id="c664a-158">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="c664a-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="c664a-159">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-159">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="c664a-160">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="c664a-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="c664a-161">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-161">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-162">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="c664a-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="c664a-163">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-163">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-164">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c664a-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c664a-165">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-165">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-166">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c664a-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="c664a-167">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-167">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c664a-168">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="c664a-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c664a-169">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-169">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-170">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="c664a-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="c664a-171">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-171">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-172">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="c664a-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c664a-173">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-173">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-174">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="c664a-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="c664a-175">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-175">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-176">&nbsp;&nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="c664a-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="c664a-177">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-177">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-178">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="c664a-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="c664a-179">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-179">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-180">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="c664a-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c664a-181">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-181">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-182">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="c664a-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c664a-183">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-183">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-184">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="c664a-184">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="c664a-185">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-185">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-186">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="c664a-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="c664a-187">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c664a-187">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c664a-188">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="c664a-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="c664a-189">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-189">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-190">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="c664a-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c664a-191">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-191">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-192">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="c664a-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="c664a-193">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-193">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-194">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="c664a-194">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="c664a-195">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-195">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="c664a-196">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="c664a-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="c664a-197">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c664a-197">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c664a-198">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c664a-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="c664a-199">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c664a-199">Request headers</span></span>

|<span data-ttu-id="c664a-200">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c664a-200">Header</span></span>|<span data-ttu-id="c664a-201">Valor</span><span class="sxs-lookup"><span data-stu-id="c664a-201">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c664a-202">Autorização</span><span class="sxs-lookup"><span data-stu-id="c664a-202">Authorization</span></span>|<span data-ttu-id="c664a-203">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c664a-203">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c664a-204">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c664a-204">Accept</span></span>|<span data-ttu-id="c664a-205">application/json</span><span class="sxs-lookup"><span data-stu-id="c664a-205">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c664a-206">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c664a-206">Request body</span></span>

<span data-ttu-id="c664a-207">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c664a-207">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="c664a-208">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c664a-208">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="c664a-209">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c664a-209">Property</span></span>|<span data-ttu-id="c664a-210">Tipo</span><span class="sxs-lookup"><span data-stu-id="c664a-210">Type</span></span>|<span data-ttu-id="c664a-211">Descrição</span><span class="sxs-lookup"><span data-stu-id="c664a-211">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c664a-212">id</span><span class="sxs-lookup"><span data-stu-id="c664a-212">id</span></span>|<span data-ttu-id="c664a-213">String</span><span class="sxs-lookup"><span data-stu-id="c664a-213">String</span></span>|<span data-ttu-id="c664a-214">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c664a-214">Unique identifier for the device.</span></span>|
|<span data-ttu-id="c664a-215">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c664a-215">**Device configuration**</span></span>|
|<span data-ttu-id="c664a-216">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="c664a-216">intuneAccountId</span></span>|<span data-ttu-id="c664a-217">GUID</span><span class="sxs-lookup"><span data-stu-id="c664a-217">GUID</span></span>|<span data-ttu-id="c664a-218">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="c664a-218">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="c664a-219">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="c664a-219">legacyPcManangementEnabled</span></span>|<span data-ttu-id="c664a-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="c664a-220">Boolean</span></span>|<span data-ttu-id="c664a-221">A propriedade para habilitar o gerenciamento de computador herdado não MDM gerenciado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="c664a-221">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="c664a-222">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c664a-222">This property is read-only.</span></span>|
|<span data-ttu-id="c664a-223">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="c664a-223">maximumDepTokens</span></span>|<span data-ttu-id="c664a-224">Int32</span><span class="sxs-lookup"><span data-stu-id="c664a-224">Int32</span></span>|<span data-ttu-id="c664a-225">Número máximo de tokens DEP permitidos por locatário.</span><span class="sxs-lookup"><span data-stu-id="c664a-225">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="c664a-226">settings</span><span class="sxs-lookup"><span data-stu-id="c664a-226">settings</span></span>|[<span data-ttu-id="c664a-227">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="c664a-227">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="c664a-228">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="c664a-228">Account level settings.</span></span>|
|<span data-ttu-id="c664a-229">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="c664a-229">**Device management**</span></span>|
|<span data-ttu-id="c664a-230">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="c664a-230">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="c664a-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c664a-231">DateTimeOffset</span></span>|<span data-ttu-id="c664a-232">A data & hora em que os dados do locatário são movidos entre o ScaleUnits.</span><span class="sxs-lookup"><span data-stu-id="c664a-232">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="c664a-233">adminConsent</span><span class="sxs-lookup"><span data-stu-id="c664a-233">adminConsent</span></span>|[<span data-ttu-id="c664a-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="c664a-234">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="c664a-235">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="c664a-235">Admin consent information.</span></span>|
|<span data-ttu-id="c664a-236">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="c664a-236">deviceProtectionOverview</span></span>|[<span data-ttu-id="c664a-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="c664a-237">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="c664a-238">Visão geral da proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c664a-238">Device protection overview.</span></span>|
|<span data-ttu-id="c664a-239">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="c664a-239">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="c664a-240">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="c664a-240">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="c664a-241">Regra de limpeza de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c664a-241">Device cleanup rule</span></span>|
|<span data-ttu-id="c664a-242">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="c664a-242">subscriptionState</span></span>|[<span data-ttu-id="c664a-243">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="c664a-243">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="c664a-244">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="c664a-244">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="c664a-245">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="c664a-245">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="c664a-246">assinaturas</span><span class="sxs-lookup"><span data-stu-id="c664a-246">subscriptions</span></span>|[<span data-ttu-id="c664a-247">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="c664a-247">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="c664a-248">Assinatura do locatário.</span><span class="sxs-lookup"><span data-stu-id="c664a-248">Tenant's Subscription.</span></span> <span data-ttu-id="c664a-249">Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="c664a-249">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="c664a-250">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="c664a-250">windowsMalwareOverview</span></span>|[<span data-ttu-id="c664a-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="c664a-251">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="c664a-252">Visão geral de malware para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="c664a-252">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="c664a-253">**Integração**</span><span class="sxs-lookup"><span data-stu-id="c664a-253">**Onboarding**</span></span>|
|<span data-ttu-id="c664a-254">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="c664a-254">intuneBrand</span></span>|[<span data-ttu-id="c664a-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="c664a-255">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="c664a-256">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="c664a-256">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="c664a-257">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="c664a-257">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="c664a-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="c664a-258">Response</span></span>
<span data-ttu-id="c664a-259">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c664a-259">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c664a-260">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c664a-260">Example</span></span>

### <a name="request"></a><span data-ttu-id="c664a-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c664a-261">Request</span></span>

<span data-ttu-id="c664a-262">Veja a seguir um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="c664a-262">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="c664a-263">Resposta</span><span class="sxs-lookup"><span data-stu-id="c664a-263">Response</span></span>

<span data-ttu-id="c664a-264">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c664a-264">Here is an example of the response.</span></span> 

<span data-ttu-id="c664a-265">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="c664a-265">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c664a-266">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="c664a-266">Returned properties vary according to workflow and context.</span></span>

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







