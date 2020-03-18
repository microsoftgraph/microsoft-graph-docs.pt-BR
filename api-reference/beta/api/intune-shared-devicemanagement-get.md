---
title: Acessar deviceManagement
description: Leia as propriedades e as relações do objeto deviceManagement.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 15b5e1b63cec316de7bd2e6428375a1fd3027b0b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801072"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="ae493-103">Acessar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ae493-103">Get deviceManagement</span></span>

> <span data-ttu-id="ae493-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ae493-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae493-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ae493-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae493-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae493-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae493-107">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ae493-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae493-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae493-108">Prerequisites</span></span>

<span data-ttu-id="ae493-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae493-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae493-111">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="ae493-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="ae493-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae493-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="ae493-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae493-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="ae493-114">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="ae493-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="ae493-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ae493-116">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="ae493-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="ae493-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="ae493-118">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="ae493-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="ae493-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ae493-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ae493-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ae493-122">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ae493-122">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="ae493-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="ae493-124">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ae493-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ae493-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="ae493-126">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="ae493-126">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="ae493-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ae493-128">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="ae493-128">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ae493-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-130">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="ae493-130">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="ae493-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ae493-132">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="ae493-132">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="ae493-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-134">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="ae493-134">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="ae493-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-136">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="ae493-136">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ae493-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-138">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="ae493-138">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ae493-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-140">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="ae493-140">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="ae493-141">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-141">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="ae493-142">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="ae493-142">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="ae493-143">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-143">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ae493-144">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="ae493-144">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="ae493-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-146">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="ae493-146">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="ae493-147">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-147">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-148">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="ae493-148">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="ae493-149">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-149">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-150">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="ae493-150">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ae493-151">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-151">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="ae493-152">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="ae493-152">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="ae493-153">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-153">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="ae493-154">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae493-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae493-155">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae493-155">Not supported.</span></span>|
| <span data-ttu-id="ae493-156">Application</span><span class="sxs-lookup"><span data-stu-id="ae493-156">Application</span></span> | |
| <span data-ttu-id="ae493-157">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="ae493-157">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="ae493-158">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-158">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ae493-159">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="ae493-159">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="ae493-160">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-160">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="ae493-161">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="ae493-161">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="ae493-162">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-162">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-163">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ae493-163">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ae493-164">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-164">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ae493-165">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ae493-165">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="ae493-166">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-166">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="ae493-167">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ae493-167">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ae493-168">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-168">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="ae493-169">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="ae493-169">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="ae493-170">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-170">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ae493-171">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="ae493-171">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ae493-172">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-172">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-173">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="ae493-173">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="ae493-174">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-174">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ae493-175">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="ae493-175">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="ae493-176">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-176">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-177">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="ae493-177">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="ae493-178">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-178">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-179">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="ae493-179">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ae493-180">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-180">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-181">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="ae493-181">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ae493-182">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-182">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-183">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="ae493-183">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="ae493-184">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-184">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="ae493-185">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="ae493-185">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="ae493-186">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-186">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="ae493-187">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="ae493-187">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="ae493-188">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-188">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-189">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="ae493-189">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="ae493-190">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-190">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-191">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="ae493-191">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="ae493-192">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-192">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="ae493-193">&nbsp; &nbsp; **Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="ae493-193">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ae493-194">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-194">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="ae493-195">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="ae493-195">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="ae493-196">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae493-196">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae493-197">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae493-197">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae493-198">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ae493-198">Optional query parameters</span></span>

<span data-ttu-id="ae493-199">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ae493-199">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae493-200">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae493-200">Request headers</span></span>
|<span data-ttu-id="ae493-201">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae493-201">Header</span></span>|<span data-ttu-id="ae493-202">Valor</span><span class="sxs-lookup"><span data-stu-id="ae493-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae493-203">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae493-203">Authorization</span></span>|<span data-ttu-id="ae493-204">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae493-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae493-205">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae493-205">Accept</span></span>|<span data-ttu-id="ae493-206">application/json</span><span class="sxs-lookup"><span data-stu-id="ae493-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae493-207">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae493-207">Request body</span></span>

<span data-ttu-id="ae493-208">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae493-208">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae493-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae493-209">Response</span></span>

<span data-ttu-id="ae493-210">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae493-210">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae493-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae493-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae493-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae493-212">Request</span></span>

<span data-ttu-id="ae493-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae493-213">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="ae493-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae493-214">Response</span></span>

<span data-ttu-id="ae493-215">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae493-215">Here are example of the response.</span></span> 

<span data-ttu-id="ae493-216">Observação: os objetos de resposta mostrados aqui podem ser truncados por brevidade.</span><span class="sxs-lookup"><span data-stu-id="ae493-216">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="ae493-217">As propriedades apropriadas para o fluxo de trabalho são retornadas.</span><span class="sxs-lookup"><span data-stu-id="ae493-217">Properties appropriate for the workflow are returned.</span></span>

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










