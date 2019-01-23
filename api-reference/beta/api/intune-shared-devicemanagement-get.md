---
title: Get deviceManagement
description: Ler propriedades e relações do objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 09563eeced6f557df2c2e40f126623f974cea2d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415863"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="34ba8-103">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="34ba8-103">Get deviceManagement</span></span>

> <span data-ttu-id="34ba8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="34ba8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="34ba8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="34ba8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34ba8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="34ba8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34ba8-107">Ler propriedades e relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="34ba8-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34ba8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34ba8-108">Prerequisites</span></span>

<span data-ttu-id="34ba8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34ba8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34ba8-111">Permissão&nbsp;tipo&nbsp;(por&nbsp;fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="34ba8-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="34ba8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34ba8-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="34ba8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34ba8-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="34ba8-114">&nbsp;&nbsp; **Android para o trabalho**</span><span class="sxs-lookup"><span data-stu-id="34ba8-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="34ba8-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="34ba8-116">&nbsp;&nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="34ba8-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="34ba8-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="34ba8-118">&nbsp;&nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="34ba8-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="34ba8-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="34ba8-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="34ba8-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="34ba8-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="34ba8-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="34ba8-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="34ba8-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="34ba8-124">&nbsp;&nbsp; **SIM eletrônico**</span><span class="sxs-lookup"><span data-stu-id="34ba8-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="34ba8-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="34ba8-126">&nbsp; &nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="34ba8-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="34ba8-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="34ba8-128">&nbsp;&nbsp; **Fencing**</span><span class="sxs-lookup"><span data-stu-id="34ba8-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="34ba8-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="34ba8-130">&nbsp; &nbsp; **Notification**</span><span class="sxs-lookup"><span data-stu-id="34ba8-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="34ba8-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="34ba8-132">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="34ba8-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="34ba8-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="34ba8-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="34ba8-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="34ba8-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="34ba8-136">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="34ba8-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="34ba8-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="34ba8-138">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="34ba8-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="34ba8-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="34ba8-140">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="34ba8-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="34ba8-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="34ba8-142">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="34ba8-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="34ba8-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="34ba8-144">&nbsp;&nbsp; **Proteção de informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="34ba8-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="34ba8-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="34ba8-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="34ba8-146">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34ba8-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34ba8-147">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34ba8-147">Not supported.</span></span>|
| <span data-ttu-id="34ba8-148">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34ba8-148">Application</span></span> | <span data-ttu-id="34ba8-149">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34ba8-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="34ba8-150">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34ba8-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34ba8-151">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34ba8-151">Optional query parameters</span></span>

<span data-ttu-id="34ba8-152">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="34ba8-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34ba8-153">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34ba8-153">Request headers</span></span>
|<span data-ttu-id="34ba8-154">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34ba8-154">Header</span></span>|<span data-ttu-id="34ba8-155">Valor</span><span class="sxs-lookup"><span data-stu-id="34ba8-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34ba8-156">Autorização</span><span class="sxs-lookup"><span data-stu-id="34ba8-156">Authorization</span></span>|<span data-ttu-id="34ba8-157">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34ba8-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34ba8-158">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34ba8-158">Accept</span></span>|<span data-ttu-id="34ba8-159">application/json</span><span class="sxs-lookup"><span data-stu-id="34ba8-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34ba8-160">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34ba8-160">Request body</span></span>

<span data-ttu-id="34ba8-161">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34ba8-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34ba8-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="34ba8-162">Response</span></span>

<span data-ttu-id="34ba8-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34ba8-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34ba8-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34ba8-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="34ba8-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34ba8-165">Request</span></span>

<span data-ttu-id="34ba8-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34ba8-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="34ba8-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="34ba8-167">Response</span></span>

<span data-ttu-id="34ba8-168">Eis um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34ba8-168">Here are example of the response.</span></span> 

<span data-ttu-id="34ba8-169">Observação: Os objetos de resposta mostrados aqui podem estar truncados para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="34ba8-169">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="34ba8-170">Propriedades apropriadas para o fluxo de trabalho são retornadas.</span><span class="sxs-lookup"><span data-stu-id="34ba8-170">Properties appropriate for the workflow are returned.</span></span>

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



