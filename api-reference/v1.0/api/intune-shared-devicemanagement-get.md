---
title: Acessar deviceManagement
description: Leia as propriedades e as relações do objeto deviceManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7fccbc17390e9cd481c2fd06af09ba5681a1e56
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732288"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="3c04a-103">Acessar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3c04a-103">Get deviceManagement</span></span>

<span data-ttu-id="3c04a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c04a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c04a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c04a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c04a-106">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="3c04a-106">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c04a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c04a-107">Prerequisites</span></span>
<span data-ttu-id="3c04a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c04a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c04a-110">Tipo &nbsp; de &nbsp; permissão (por fluxo de &nbsp; trabalho)</span><span class="sxs-lookup"><span data-stu-id="3c04a-110">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="3c04a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c04a-111">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="3c04a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c04a-112">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="3c04a-113">&nbsp;&nbsp;Auditoria</span><span class="sxs-lookup"><span data-stu-id="3c04a-113">&nbsp; &nbsp; Auditing</span></span> | <span data-ttu-id="3c04a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="3c04a-115">&nbsp;&nbsp;Termos da empresa</span><span class="sxs-lookup"><span data-stu-id="3c04a-115">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="3c04a-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3c04a-117">&nbsp;&nbsp;Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3c04a-117">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="3c04a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="3c04a-119">&nbsp;&nbsp;Gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="3c04a-119">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="3c04a-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="3c04a-121">&nbsp;&nbsp;Inscrição</span><span class="sxs-lookup"><span data-stu-id="3c04a-121">&nbsp; &nbsp; Enrollment</span></span> | <span data-ttu-id="3c04a-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3c04a-123">&nbsp;&nbsp;Notificação</span><span class="sxs-lookup"><span data-stu-id="3c04a-123">&nbsp; &nbsp; Notification</span></span> | <span data-ttu-id="3c04a-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3c04a-125">&nbsp;&nbsp;Integração</span><span class="sxs-lookup"><span data-stu-id="3c04a-125">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="3c04a-126">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-126">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3c04a-127">&nbsp;&nbsp;RBAC</span><span class="sxs-lookup"><span data-stu-id="3c04a-127">&nbsp; &nbsp; RBAC</span></span> | <span data-ttu-id="3c04a-128">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-128">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="3c04a-129">&nbsp;&nbsp;Assistência remota</span><span class="sxs-lookup"><span data-stu-id="3c04a-129">&nbsp; &nbsp; Remote assistance</span></span> | <span data-ttu-id="3c04a-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3c04a-131">&nbsp;&nbsp;Gerenciamento de despesas de telecomunicações</span><span class="sxs-lookup"><span data-stu-id="3c04a-131">&nbsp; &nbsp; Telecom expense management</span></span> | <span data-ttu-id="3c04a-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="3c04a-133">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="3c04a-133">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="3c04a-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="3c04a-135">&nbsp;&nbsp;Windows Proteção de Informações</span><span class="sxs-lookup"><span data-stu-id="3c04a-135">&nbsp; &nbsp; Windows Information Protection</span></span> | <span data-ttu-id="3c04a-136">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-136">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="3c04a-137">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c04a-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c04a-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c04a-138">Not supported.</span></span>|
| <span data-ttu-id="3c04a-139">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c04a-139">Application</span></span> | <span data-ttu-id="3c04a-140">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c04a-140">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="3c04a-141">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c04a-141">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c04a-142">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c04a-142">Optional query parameters</span></span>
<span data-ttu-id="3c04a-143">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c04a-143">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3c04a-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c04a-144">Request headers</span></span>
|<span data-ttu-id="3c04a-145">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c04a-145">Header</span></span>|<span data-ttu-id="3c04a-146">Valor</span><span class="sxs-lookup"><span data-stu-id="3c04a-146">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c04a-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c04a-147">Authorization</span></span>|<span data-ttu-id="3c04a-148">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c04a-148">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c04a-149">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c04a-149">Accept</span></span>|<span data-ttu-id="3c04a-150">application/json</span><span class="sxs-lookup"><span data-stu-id="3c04a-150">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c04a-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c04a-151">Request body</span></span>
<span data-ttu-id="3c04a-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c04a-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c04a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c04a-153">Response</span></span>
<span data-ttu-id="3c04a-154">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c04a-154">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c04a-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c04a-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c04a-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c04a-156">Request</span></span>
<span data-ttu-id="3c04a-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c04a-157">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="3c04a-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c04a-158">Response</span></span>
<span data-ttu-id="3c04a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c04a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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