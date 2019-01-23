---
title: Obter windowsProtectionState
description: Leia as propriedades e os relacionamentos do objeto windowsProtectionState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a8cfbbfec55a1eaea37e1e729488b70b73a7c58
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419867"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="30d88-103">Obter windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="30d88-103">Get windowsProtectionState</span></span>

> <span data-ttu-id="30d88-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="30d88-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="30d88-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="30d88-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30d88-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="30d88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30d88-107">Leia as propriedades e os relacionamentos do objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="30d88-107">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30d88-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30d88-108">Prerequisites</span></span>
<span data-ttu-id="30d88-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="30d88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="30d88-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30d88-111">Permission type</span></span>|<span data-ttu-id="30d88-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30d88-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30d88-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30d88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30d88-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="30d88-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="30d88-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30d88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30d88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30d88-116">Not supported.</span></span>|
|<span data-ttu-id="30d88-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30d88-117">Application</span></span>|<span data-ttu-id="30d88-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30d88-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30d88-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30d88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30d88-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="30d88-120">Optional query parameters</span></span>
<span data-ttu-id="30d88-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="30d88-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30d88-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30d88-122">Request headers</span></span>
|<span data-ttu-id="30d88-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30d88-123">Header</span></span>|<span data-ttu-id="30d88-124">Valor</span><span class="sxs-lookup"><span data-stu-id="30d88-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30d88-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="30d88-125">Authorization</span></span>|<span data-ttu-id="30d88-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30d88-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30d88-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30d88-127">Accept</span></span>|<span data-ttu-id="30d88-128">application/json</span><span class="sxs-lookup"><span data-stu-id="30d88-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30d88-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30d88-129">Request body</span></span>
<span data-ttu-id="30d88-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30d88-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30d88-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="30d88-131">Response</span></span>
<span data-ttu-id="30d88-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30d88-132">If successful, this method returns a `200 OK` response code and [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30d88-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30d88-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="30d88-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30d88-134">Request</span></span>
<span data-ttu-id="30d88-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30d88-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
```

### <a name="response"></a><span data-ttu-id="30d88-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="30d88-136">Response</span></span>
<span data-ttu-id="30d88-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30d88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




