---
title: Obter Windowsprotectionstate foi
description: Leia as propriedades e as relações do objeto Windowsprotectionstate foi.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82a3e50e13f38e02b2d535fc00fac8c28f964feb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724245"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="32cc1-103">Obter Windowsprotectionstate foi</span><span class="sxs-lookup"><span data-stu-id="32cc1-103">Get windowsProtectionState</span></span>

<span data-ttu-id="32cc1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32cc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32cc1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32cc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32cc1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32cc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32cc1-107">Leia as propriedades e as relações do objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="32cc1-107">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32cc1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32cc1-108">Prerequisites</span></span>
<span data-ttu-id="32cc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32cc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32cc1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32cc1-111">Permission type</span></span>|<span data-ttu-id="32cc1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32cc1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32cc1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32cc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32cc1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="32cc1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="32cc1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32cc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32cc1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32cc1-116">Not supported.</span></span>|
|<span data-ttu-id="32cc1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32cc1-117">Application</span></span>|<span data-ttu-id="32cc1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="32cc1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32cc1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32cc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32cc1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="32cc1-120">Optional query parameters</span></span>
<span data-ttu-id="32cc1-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="32cc1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32cc1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32cc1-122">Request headers</span></span>
|<span data-ttu-id="32cc1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32cc1-123">Header</span></span>|<span data-ttu-id="32cc1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="32cc1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32cc1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="32cc1-125">Authorization</span></span>|<span data-ttu-id="32cc1-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32cc1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32cc1-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32cc1-127">Accept</span></span>|<span data-ttu-id="32cc1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="32cc1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32cc1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32cc1-129">Request body</span></span>
<span data-ttu-id="32cc1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32cc1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32cc1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="32cc1-131">Response</span></span>
<span data-ttu-id="32cc1-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsprotectionstate foi](../resources/intune-devices-windowsprotectionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32cc1-132">If successful, this method returns a `200 OK` response code and [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32cc1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32cc1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="32cc1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32cc1-134">Request</span></span>
<span data-ttu-id="32cc1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32cc1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

### <a name="response"></a><span data-ttu-id="32cc1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="32cc1-136">Response</span></span>
<span data-ttu-id="32cc1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32cc1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





