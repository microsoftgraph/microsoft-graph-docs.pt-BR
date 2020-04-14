---
title: Obter Windowsprotectionstate foi
description: Leia as propriedades e as relações do objeto Windowsprotectionstate foi.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 349cfcd0d82928dcb0b1e73924f2b5528cb19199
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43378186"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="1ff75-103">Obter Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="1ff75-103">Get windowsProtectionState</span></span>

<span data-ttu-id="1ff75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ff75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ff75-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ff75-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ff75-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ff75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ff75-107">Leia as propriedades e as relações do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="1ff75-107">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ff75-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ff75-108">Prerequisites</span></span>
<span data-ttu-id="1ff75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ff75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ff75-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ff75-111">Permission type</span></span>|<span data-ttu-id="1ff75-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ff75-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ff75-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ff75-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ff75-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ff75-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1ff75-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ff75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ff75-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ff75-116">Not supported.</span></span>|
|<span data-ttu-id="1ff75-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ff75-117">Application</span></span>|<span data-ttu-id="1ff75-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ff75-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ff75-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff75-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ff75-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1ff75-120">Optional query parameters</span></span>
<span data-ttu-id="1ff75-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1ff75-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ff75-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff75-122">Request headers</span></span>
|<span data-ttu-id="1ff75-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ff75-123">Header</span></span>|<span data-ttu-id="1ff75-124">Valor</span><span class="sxs-lookup"><span data-stu-id="1ff75-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ff75-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ff75-125">Authorization</span></span>|<span data-ttu-id="1ff75-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ff75-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ff75-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ff75-127">Accept</span></span>|<span data-ttu-id="1ff75-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1ff75-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ff75-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff75-129">Request body</span></span>
<span data-ttu-id="1ff75-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1ff75-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ff75-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ff75-131">Response</span></span>
<span data-ttu-id="1ff75-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ff75-132">If successful, this method returns a `200 OK` response code and [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ff75-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ff75-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ff75-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ff75-134">Request</span></span>
<span data-ttu-id="1ff75-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ff75-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
```

### <a name="response"></a><span data-ttu-id="1ff75-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ff75-136">Response</span></span>
<span data-ttu-id="1ff75-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ff75-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 971

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
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
  }
}
```



