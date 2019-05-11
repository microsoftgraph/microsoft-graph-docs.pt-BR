---
title: Acessar deviceManagement
description: Leia as propriedades e as relações do objeto deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bbbe6c21d602266be2223fbd72b10ae9f51f7818
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898378"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="95bb5-103">Acessar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="95bb5-103">Get deviceManagement</span></span>

> <span data-ttu-id="95bb5-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="95bb5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="95bb5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="95bb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95bb5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95bb5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95bb5-107">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="95bb5-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95bb5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95bb5-108">Prerequisites</span></span>

<span data-ttu-id="95bb5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95bb5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95bb5-111">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="95bb5-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="95bb5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="95bb5-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="95bb5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95bb5-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="95bb5-114">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="95bb5-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="95bb5-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="95bb5-116">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="95bb5-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="95bb5-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="95bb5-118">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="95bb5-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="95bb5-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="95bb5-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="95bb5-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="95bb5-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="95bb5-122">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="95bb5-122">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="95bb5-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="95bb5-124">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="95bb5-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="95bb5-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="95bb5-126">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="95bb5-126">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="95bb5-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="95bb5-128">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="95bb5-128">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="95bb5-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="95bb5-130">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="95bb5-130">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="95bb5-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="95bb5-132">&nbsp;&nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="95bb5-132">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="95bb5-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="95bb5-134">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="95bb5-134">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="95bb5-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="95bb5-136">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="95bb5-136">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="95bb5-137">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-137">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="95bb5-138">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="95bb5-138">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="95bb5-139">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-139">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="95bb5-140">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="95bb5-140">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="95bb5-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="95bb5-142">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="95bb5-142">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="95bb5-143">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-143">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="95bb5-144">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="95bb5-144">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="95bb5-145">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-145">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="95bb5-146">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="95bb5-146">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="95bb5-147">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="95bb5-147">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="95bb5-148">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95bb5-148">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95bb5-149">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95bb5-149">Not supported.</span></span>|
| <span data-ttu-id="95bb5-150">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95bb5-150">Application</span></span> | <span data-ttu-id="95bb5-151">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95bb5-151">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="95bb5-152">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95bb5-152">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="95bb5-153">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="95bb5-153">Optional query parameters</span></span>

<span data-ttu-id="95bb5-154">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="95bb5-154">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95bb5-155">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95bb5-155">Request headers</span></span>
|<span data-ttu-id="95bb5-156">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95bb5-156">Header</span></span>|<span data-ttu-id="95bb5-157">Valor</span><span class="sxs-lookup"><span data-stu-id="95bb5-157">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95bb5-158">Autorização</span><span class="sxs-lookup"><span data-stu-id="95bb5-158">Authorization</span></span>|<span data-ttu-id="95bb5-159">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95bb5-159">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95bb5-160">Aceitar</span><span class="sxs-lookup"><span data-stu-id="95bb5-160">Accept</span></span>|<span data-ttu-id="95bb5-161">application/json</span><span class="sxs-lookup"><span data-stu-id="95bb5-161">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95bb5-162">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95bb5-162">Request body</span></span>

<span data-ttu-id="95bb5-163">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95bb5-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95bb5-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="95bb5-164">Response</span></span>

<span data-ttu-id="95bb5-165">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95bb5-165">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95bb5-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95bb5-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="95bb5-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95bb5-167">Request</span></span>

<span data-ttu-id="95bb5-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95bb5-168">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="95bb5-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="95bb5-169">Response</span></span>

<span data-ttu-id="95bb5-170">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95bb5-170">Here are example of the response.</span></span> 

<span data-ttu-id="95bb5-171">Observação: os objetos de resposta mostrados aqui podem ser truncados por brevidade.</span><span class="sxs-lookup"><span data-stu-id="95bb5-171">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="95bb5-172">As propriedades apropriadas para o fluxo de trabalho são retornadas.</span><span class="sxs-lookup"><span data-stu-id="95bb5-172">Properties appropriate for the workflow are returned.</span></span>

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



