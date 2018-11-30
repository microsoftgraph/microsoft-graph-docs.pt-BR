---
title: Get deviceManagement
description: Ler propriedades e relações do objeto deviceManagement.
ms.openlocfilehash: adc45ed789e3e636282fee851997c3fbcc8d8318
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036428"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="f5c0d-103">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f5c0d-103">Get deviceManagement</span></span>

> <span data-ttu-id="f5c0d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5c0d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5c0d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5c0d-107">Ler propriedades e relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="f5c0d-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5c0d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5c0d-108">Prerequisites</span></span>

<span data-ttu-id="f5c0d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5c0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5c0d-111">Permissão&nbsp;tipo&nbsp;(por&nbsp;fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="f5c0d-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="f5c0d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5c0d-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="f5c0d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5c0d-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="f5c0d-114">&nbsp;&nbsp; **Android para o trabalho**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="f5c0d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="f5c0d-116">&nbsp;&nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="f5c0d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="f5c0d-118">&nbsp;&nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="f5c0d-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f5c0d-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f5c0d-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="f5c0d-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f5c0d-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="f5c0d-124">&nbsp;&nbsp; **SIM eletrônico**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-124">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="f5c0d-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-125">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="f5c0d-126">&nbsp; &nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-126">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="f5c0d-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f5c0d-128">&nbsp;&nbsp; **Fencing**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-128">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="f5c0d-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-129">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="f5c0d-130">&nbsp;&nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-130">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="f5c0d-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f5c0d-132">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-132">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f5c0d-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f5c0d-134">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-134">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="f5c0d-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-135">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="f5c0d-136">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-136">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="f5c0d-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-137">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="f5c0d-138">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-138">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="f5c0d-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f5c0d-140">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-140">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="f5c0d-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-141">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f5c0d-142">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-142">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="f5c0d-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-143">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="f5c0d-144">&nbsp;&nbsp; **Proteção de informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="f5c0d-144">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="f5c0d-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5c0d-145">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="f5c0d-146">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5c0d-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5c0d-147">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-147">Not supported.</span></span>|
| <span data-ttu-id="f5c0d-148">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5c0d-148">Application</span></span> | <span data-ttu-id="f5c0d-149">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-149">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="f5c0d-150">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5c0d-150">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f5c0d-151">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f5c0d-151">Optional query parameters</span></span>

<span data-ttu-id="f5c0d-152">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-152">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5c0d-153">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c0d-153">Request headers</span></span>
|<span data-ttu-id="f5c0d-154">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5c0d-154">Header</span></span>|<span data-ttu-id="f5c0d-155">Valor</span><span class="sxs-lookup"><span data-stu-id="f5c0d-155">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5c0d-156">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5c0d-156">Authorization</span></span>|<span data-ttu-id="f5c0d-157">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-157">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5c0d-158">Accept</span><span class="sxs-lookup"><span data-stu-id="f5c0d-158">Accept</span></span>|<span data-ttu-id="f5c0d-159">application/json</span><span class="sxs-lookup"><span data-stu-id="f5c0d-159">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5c0d-160">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c0d-160">Request body</span></span>

<span data-ttu-id="f5c0d-161">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5c0d-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c0d-162">Response</span></span>

<span data-ttu-id="f5c0d-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-163">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5c0d-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5c0d-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5c0d-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5c0d-165">Request</span></span>

<span data-ttu-id="f5c0d-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-166">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="f5c0d-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5c0d-167">Response</span></span>

<span data-ttu-id="f5c0d-168">Eis um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-168">Here are example of the response.</span></span> 

<span data-ttu-id="f5c0d-169">Observação: Os objetos de resposta mostrados aqui podem estar truncados para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-169">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="f5c0d-170">Propriedades apropriadas para o fluxo de trabalho são retornadas.</span><span class="sxs-lookup"><span data-stu-id="f5c0d-170">Properties appropriate for the workflow are returned.</span></span>

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



