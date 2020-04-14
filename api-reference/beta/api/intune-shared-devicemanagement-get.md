---
title: Acessar deviceManagement
description: Leia as propriedades e as relações do objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 59d83dbe212c924d74308c6f9c47ce4bfdd864b1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390235"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="88803-103">Acessar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="88803-103">Get deviceManagement</span></span>

<span data-ttu-id="88803-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88803-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88803-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="88803-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88803-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="88803-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88803-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88803-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88803-108">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="88803-108">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88803-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88803-109">Prerequisites</span></span>

<span data-ttu-id="88803-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88803-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="88803-112">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="88803-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="88803-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88803-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="88803-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88803-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="88803-115">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="88803-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="88803-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88803-117">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="88803-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="88803-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="88803-119">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="88803-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="88803-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="88803-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="88803-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88803-123">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="88803-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="88803-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="88803-125">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="88803-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="88803-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="88803-127">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="88803-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="88803-128">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-128">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88803-129">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="88803-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="88803-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-131">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="88803-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="88803-132">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-132">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88803-133">&nbsp;&nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="88803-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="88803-134">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-134">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="88803-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="88803-136">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-136">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-137">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="88803-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="88803-138">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-138">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-139">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="88803-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="88803-140">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-140">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-141">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="88803-141">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="88803-142">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-142">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="88803-143">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="88803-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="88803-144">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-144">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88803-145">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="88803-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="88803-146">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-146">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-147">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="88803-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="88803-148">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-148">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-149">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="88803-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="88803-150">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-150">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-151">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="88803-151">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="88803-152">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-152">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="88803-153">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="88803-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="88803-154">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-154">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="88803-155">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88803-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88803-156">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88803-156">Not supported.</span></span>|
| <span data-ttu-id="88803-157">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88803-157">Application</span></span> | |
| <span data-ttu-id="88803-158">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="88803-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="88803-159">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-159">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88803-160">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="88803-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="88803-161">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-161">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="88803-162">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="88803-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="88803-163">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-163">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-164">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="88803-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="88803-165">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-165">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88803-166">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="88803-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="88803-167">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-167">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="88803-168">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="88803-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="88803-169">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-169">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="88803-170">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="88803-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="88803-171">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-171">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88803-172">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="88803-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="88803-173">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-173">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-174">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="88803-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="88803-175">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-175">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88803-176">&nbsp;&nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="88803-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="88803-177">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-177">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-178">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="88803-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="88803-179">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-179">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-180">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="88803-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="88803-181">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-181">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-182">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="88803-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="88803-183">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-183">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-184">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="88803-184">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="88803-185">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-185">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="88803-186">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="88803-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="88803-187">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-187">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88803-188">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="88803-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="88803-189">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-189">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-190">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="88803-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="88803-191">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-191">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-192">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="88803-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="88803-193">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-193">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="88803-194">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="88803-194">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="88803-195">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-195">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="88803-196">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="88803-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="88803-197">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="88803-197">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88803-198">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88803-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88803-199">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88803-199">Optional query parameters</span></span>

<span data-ttu-id="88803-200">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="88803-200">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88803-201">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88803-201">Request headers</span></span>
|<span data-ttu-id="88803-202">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88803-202">Header</span></span>|<span data-ttu-id="88803-203">Valor</span><span class="sxs-lookup"><span data-stu-id="88803-203">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88803-204">Autorização</span><span class="sxs-lookup"><span data-stu-id="88803-204">Authorization</span></span>|<span data-ttu-id="88803-205">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88803-205">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88803-206">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88803-206">Accept</span></span>|<span data-ttu-id="88803-207">application/json</span><span class="sxs-lookup"><span data-stu-id="88803-207">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88803-208">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88803-208">Request body</span></span>

<span data-ttu-id="88803-209">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88803-209">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88803-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="88803-210">Response</span></span>

<span data-ttu-id="88803-211">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88803-211">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88803-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88803-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="88803-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88803-213">Request</span></span>

<span data-ttu-id="88803-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88803-214">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="88803-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="88803-215">Response</span></span>

<span data-ttu-id="88803-216">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88803-216">Here are example of the response.</span></span> 

<span data-ttu-id="88803-217">Observação: os objetos de resposta mostrados aqui podem ser truncados por brevidade.</span><span class="sxs-lookup"><span data-stu-id="88803-217">Note: The response objects shown here may be truncated for brevity.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

<span data-ttu-id="88803-218">As propriedades apropriadas para o fluxo de trabalho são retornadas.</span><span class="sxs-lookup"><span data-stu-id="88803-218">Properties appropriate for the workflow are returned.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
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
}
```









