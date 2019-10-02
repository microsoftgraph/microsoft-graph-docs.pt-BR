---
title: Acessar deviceManagement
description: Leia as propriedades e as relações do objeto deviceManagement.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd689c80863504e5ae3766a11684a83ed89d086b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361466"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="58a08-103">Acessar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="58a08-103">Get deviceManagement</span></span>

> <span data-ttu-id="58a08-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58a08-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58a08-105">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="58a08-105">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58a08-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58a08-106">Prerequisites</span></span>
<span data-ttu-id="58a08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58a08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58a08-109">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="58a08-109">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="58a08-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58a08-110">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="58a08-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58a08-111">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="58a08-112">&nbsp;&nbsp; Auditoria</span><span class="sxs-lookup"><span data-stu-id="58a08-112">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="58a08-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="58a08-114">&nbsp;&nbsp; Termos da empresa</span><span class="sxs-lookup"><span data-stu-id="58a08-114">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="58a08-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="58a08-116">&nbsp;&nbsp; Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="58a08-116">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="58a08-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="58a08-118">&nbsp;&nbsp; Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="58a08-118">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="58a08-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="58a08-120">&nbsp;&nbsp; Registro</span><span class="sxs-lookup"><span data-stu-id="58a08-120">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="58a08-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="58a08-122">&nbsp;&nbsp; Notificação</span><span class="sxs-lookup"><span data-stu-id="58a08-122">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="58a08-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="58a08-124">&nbsp;&nbsp; Integração</span><span class="sxs-lookup"><span data-stu-id="58a08-124">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="58a08-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="58a08-126">&nbsp;&nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="58a08-126">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="58a08-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-127">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="58a08-128">&nbsp;&nbsp; Assistência remota</span><span class="sxs-lookup"><span data-stu-id="58a08-128">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="58a08-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="58a08-130">&nbsp;&nbsp; Gerenciamento de despesas de telecomunicações</span><span class="sxs-lookup"><span data-stu-id="58a08-130">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="58a08-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="58a08-132">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="58a08-132">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="58a08-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="58a08-134">&nbsp;&nbsp; Proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="58a08-134">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="58a08-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a08-135">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="58a08-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58a08-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58a08-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58a08-137">Not supported.</span></span>|
| <span data-ttu-id="58a08-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58a08-138">Application</span></span> | <span data-ttu-id="58a08-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58a08-139">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="58a08-140">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58a08-140">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58a08-141">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58a08-141">Optional query parameters</span></span>
<span data-ttu-id="58a08-142">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="58a08-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="58a08-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58a08-143">Request headers</span></span>
|<span data-ttu-id="58a08-144">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58a08-144">Header</span></span>|<span data-ttu-id="58a08-145">Valor</span><span class="sxs-lookup"><span data-stu-id="58a08-145">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58a08-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="58a08-146">Authorization</span></span>|<span data-ttu-id="58a08-147">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58a08-147">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58a08-148">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58a08-148">Accept</span></span>|<span data-ttu-id="58a08-149">application/json</span><span class="sxs-lookup"><span data-stu-id="58a08-149">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58a08-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58a08-150">Request body</span></span>
<span data-ttu-id="58a08-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58a08-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58a08-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="58a08-152">Response</span></span>
<span data-ttu-id="58a08-153">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58a08-153">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a08-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58a08-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="58a08-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58a08-155">Request</span></span>
<span data-ttu-id="58a08-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58a08-156">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="58a08-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="58a08-157">Response</span></span>
<span data-ttu-id="58a08-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58a08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




