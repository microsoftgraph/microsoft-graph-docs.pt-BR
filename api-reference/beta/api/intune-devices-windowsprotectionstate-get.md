---
title: Obter windowsProtectionState
description: Leia propriedades e relações do objeto windowsProtectionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c4f0af8b1abe08720f904503b912cae6b7567701
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126315"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="6d997-103">Obter windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="6d997-103">Get windowsProtectionState</span></span>

<span data-ttu-id="6d997-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d997-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d997-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d997-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d997-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d997-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d997-107">Leia propriedades e relações do [objeto windowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)</span><span class="sxs-lookup"><span data-stu-id="6d997-107">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d997-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d997-108">Prerequisites</span></span>
<span data-ttu-id="6d997-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d997-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d997-111">Permission type</span></span>|<span data-ttu-id="6d997-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d997-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d997-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d997-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d997-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d997-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6d997-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d997-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d997-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d997-116">Not supported.</span></span>|
|<span data-ttu-id="6d997-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d997-117">Application</span></span>|<span data-ttu-id="6d997-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d997-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d997-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d997-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d997-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6d997-120">Optional query parameters</span></span>
<span data-ttu-id="6d997-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6d997-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d997-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d997-122">Request headers</span></span>
|<span data-ttu-id="6d997-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d997-123">Header</span></span>|<span data-ttu-id="6d997-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6d997-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d997-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d997-125">Authorization</span></span>|<span data-ttu-id="6d997-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d997-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d997-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d997-127">Accept</span></span>|<span data-ttu-id="6d997-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6d997-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d997-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d997-129">Request body</span></span>
<span data-ttu-id="6d997-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d997-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d997-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d997-131">Response</span></span>
<span data-ttu-id="6d997-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d997-132">If successful, this method returns a `200 OK` response code and [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d997-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d997-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d997-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d997-134">Request</span></span>
<span data-ttu-id="6d997-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d997-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

### <a name="response"></a><span data-ttu-id="6d997-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d997-136">Response</span></span>
<span data-ttu-id="6d997-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d997-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1083

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsProtectionState",
    "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
    "malwareProtectionEnabled": true,
    "deviceState": "fullScanPending",
    "realTimeProtectionEnabled": true,
    "networkInspectionSystemEnabled": true,
    "quickScanOverdue": true,
    "fullScanOverdue": true,
    "signatureUpdateOverdue": true,
    "rebootRequired": true,
    "fullScanRequired": true,
    "engineVersion": "Engine Version value",
    "signatureVersion": "Signature Version value",
    "antiMalwareVersion": "Anti Malware Version value",
    "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
    "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
    "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
    "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "productStatus": "serviceNotRunning",
    "isVirtualMachine": true,
    "tamperProtectionEnabled": true
  }
}
```




