---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02ece544ac7b4b78beb8e49bb67e33035a0d0bf9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706321"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="63d57-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="63d57-103">Update deviceManagement</span></span>

<span data-ttu-id="63d57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63d57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63d57-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="63d57-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63d57-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="63d57-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63d57-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63d57-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63d57-108">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="63d57-108">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63d57-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63d57-109">Prerequisites</span></span>

<span data-ttu-id="63d57-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63d57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="63d57-112">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="63d57-112">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="63d57-113">&nbsp;Tipo &nbsp; de permissão (por &nbsp; fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="63d57-113">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="63d57-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63d57-114">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="63d57-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63d57-115">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="63d57-116">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="63d57-116">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="63d57-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-117">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="63d57-118">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="63d57-118">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="63d57-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-119">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-120">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="63d57-120">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="63d57-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-121">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="63d57-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="63d57-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-124">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="63d57-124">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="63d57-125">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-125">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="63d57-126">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="63d57-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="63d57-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-127">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-128">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="63d57-128">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="63d57-129">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-129">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-130">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="63d57-130">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="63d57-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-132">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="63d57-132">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="63d57-133">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-133">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-134">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="63d57-134">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="63d57-135">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-135">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-136">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="63d57-136">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="63d57-137">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-137">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-138">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="63d57-138">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="63d57-139">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-139">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-140">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="63d57-140">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="63d57-141">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-141">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-142">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="63d57-142">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="63d57-143">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-143">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-144">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="63d57-144">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="63d57-145">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63d57-145">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="63d57-146">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="63d57-146">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="63d57-147">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-147">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-148">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="63d57-148">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="63d57-149">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-149">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-150">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="63d57-150">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="63d57-151">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-151">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-152">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="63d57-152">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="63d57-153">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-153">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-154">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="63d57-154">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="63d57-155">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-155">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-156">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63d57-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63d57-157">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63d57-157">Not supported.</span></span>|
| <span data-ttu-id="63d57-158">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63d57-158">Application</span></span> ||
| <span data-ttu-id="63d57-159">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="63d57-159">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="63d57-160">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-160">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="63d57-161">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="63d57-161">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="63d57-162">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-162">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-163">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="63d57-163">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="63d57-164">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-164">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-165">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="63d57-165">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="63d57-166">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-166">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-167">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="63d57-167">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="63d57-168">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-168">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="63d57-169">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="63d57-169">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="63d57-170">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-170">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-171">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="63d57-171">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="63d57-172">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-172">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-173">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="63d57-173">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="63d57-174">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-174">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-175">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="63d57-175">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="63d57-176">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-176">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-177">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="63d57-177">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="63d57-178">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-178">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-179">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="63d57-179">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="63d57-180">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-180">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-181">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="63d57-181">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="63d57-182">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-182">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-183">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="63d57-183">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="63d57-184">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-184">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-185">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="63d57-185">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="63d57-186">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-186">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-187">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="63d57-187">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="63d57-188">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63d57-188">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="63d57-189">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="63d57-189">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="63d57-190">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-190">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-191">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="63d57-191">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="63d57-192">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-192">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-193">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="63d57-193">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="63d57-194">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-194">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-195">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="63d57-195">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="63d57-196">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-196">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="63d57-197">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="63d57-197">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="63d57-198">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63d57-198">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63d57-199">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63d57-199">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="63d57-200">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63d57-200">Request headers</span></span>

|<span data-ttu-id="63d57-201">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63d57-201">Header</span></span>|<span data-ttu-id="63d57-202">Valor</span><span class="sxs-lookup"><span data-stu-id="63d57-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63d57-203">Autorização</span><span class="sxs-lookup"><span data-stu-id="63d57-203">Authorization</span></span>|<span data-ttu-id="63d57-204">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63d57-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63d57-205">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63d57-205">Accept</span></span>|<span data-ttu-id="63d57-206">application/json</span><span class="sxs-lookup"><span data-stu-id="63d57-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63d57-207">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63d57-207">Request body</span></span>

<span data-ttu-id="63d57-208">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="63d57-208">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="63d57-209">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="63d57-209">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="63d57-210">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63d57-210">Property</span></span>|<span data-ttu-id="63d57-211">Tipo</span><span class="sxs-lookup"><span data-stu-id="63d57-211">Type</span></span>|<span data-ttu-id="63d57-212">Descrição</span><span class="sxs-lookup"><span data-stu-id="63d57-212">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63d57-213">id</span><span class="sxs-lookup"><span data-stu-id="63d57-213">id</span></span>|<span data-ttu-id="63d57-214">String</span><span class="sxs-lookup"><span data-stu-id="63d57-214">String</span></span>|<span data-ttu-id="63d57-215">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63d57-215">Unique identifier for the device.</span></span>|
|<span data-ttu-id="63d57-216">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="63d57-216">**Device configuration**</span></span>|
|<span data-ttu-id="63d57-217">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="63d57-217">intuneAccountId</span></span>|<span data-ttu-id="63d57-218">GUID</span><span class="sxs-lookup"><span data-stu-id="63d57-218">GUID</span></span>|<span data-ttu-id="63d57-219">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="63d57-219">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="63d57-220">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="63d57-220">legacyPcManangementEnabled</span></span>|<span data-ttu-id="63d57-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="63d57-221">Boolean</span></span>|<span data-ttu-id="63d57-222">A propriedade para habilitar o gerenciamento de computador herdado não MDM gerenciado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="63d57-222">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="63d57-223">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="63d57-223">This property is read-only.</span></span>|
|<span data-ttu-id="63d57-224">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="63d57-224">maximumDepTokens</span></span>|<span data-ttu-id="63d57-225">Int32</span><span class="sxs-lookup"><span data-stu-id="63d57-225">Int32</span></span>|<span data-ttu-id="63d57-226">Número máximo de tokens DEP permitidos por locatário.</span><span class="sxs-lookup"><span data-stu-id="63d57-226">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="63d57-227">settings</span><span class="sxs-lookup"><span data-stu-id="63d57-227">settings</span></span>|[<span data-ttu-id="63d57-228">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="63d57-228">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="63d57-229">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="63d57-229">Account level settings.</span></span>|
|<span data-ttu-id="63d57-230">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="63d57-230">**Device management**</span></span>|
|<span data-ttu-id="63d57-231">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="63d57-231">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="63d57-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63d57-232">DateTimeOffset</span></span>|<span data-ttu-id="63d57-233">A data & hora em que os dados do locatário são movidos entre o ScaleUnits.</span><span class="sxs-lookup"><span data-stu-id="63d57-233">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="63d57-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="63d57-234">adminConsent</span></span>|[<span data-ttu-id="63d57-235">adminConsent</span><span class="sxs-lookup"><span data-stu-id="63d57-235">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="63d57-236">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="63d57-236">Admin consent information.</span></span>|
|<span data-ttu-id="63d57-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="63d57-237">deviceProtectionOverview</span></span>|[<span data-ttu-id="63d57-238">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="63d57-238">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="63d57-239">Visão geral da proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63d57-239">Device protection overview.</span></span>|
|<span data-ttu-id="63d57-240">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="63d57-240">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="63d57-241">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="63d57-241">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="63d57-242">Regra de limpeza de dispositivo</span><span class="sxs-lookup"><span data-stu-id="63d57-242">Device cleanup rule</span></span>|
|<span data-ttu-id="63d57-243">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="63d57-243">subscriptionState</span></span>|[<span data-ttu-id="63d57-244">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="63d57-244">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="63d57-245">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="63d57-245">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="63d57-246">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="63d57-246">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="63d57-247">assinaturas</span><span class="sxs-lookup"><span data-stu-id="63d57-247">subscriptions</span></span>|[<span data-ttu-id="63d57-248">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="63d57-248">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="63d57-249">Assinatura do locatário.</span><span class="sxs-lookup"><span data-stu-id="63d57-249">Tenant's Subscription.</span></span> <span data-ttu-id="63d57-250">Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="63d57-250">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="63d57-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="63d57-251">windowsMalwareOverview</span></span>|[<span data-ttu-id="63d57-252">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="63d57-252">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="63d57-253">Visão geral de malware para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="63d57-253">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="63d57-254">**Integração**</span><span class="sxs-lookup"><span data-stu-id="63d57-254">**Onboarding**</span></span>|
|<span data-ttu-id="63d57-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="63d57-255">intuneBrand</span></span>|[<span data-ttu-id="63d57-256">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="63d57-256">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="63d57-257">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="63d57-257">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="63d57-258">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="63d57-258">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="63d57-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="63d57-259">Response</span></span>
<span data-ttu-id="63d57-260">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63d57-260">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63d57-261">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63d57-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="63d57-262">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63d57-262">Request</span></span>

<span data-ttu-id="63d57-263">Veja a seguir um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="63d57-263">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="63d57-264">Resposta</span><span class="sxs-lookup"><span data-stu-id="63d57-264">Response</span></span>

<span data-ttu-id="63d57-265">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63d57-265">Here is an example of the response.</span></span>

<span data-ttu-id="63d57-266">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="63d57-266">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="63d57-267">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="63d57-267">Returned properties vary according to workflow and context.</span></span>

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











