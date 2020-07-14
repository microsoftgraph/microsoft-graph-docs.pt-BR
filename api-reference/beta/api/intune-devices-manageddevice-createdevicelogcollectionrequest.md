---
title: ação createDeviceLogCollectionRequest
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 15deac0383992f2045599aff34d097c3555be7f0
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124159"
---
# <a name="createdevicelogcollectionrequest-action"></a><span data-ttu-id="14d56-103">ação createDeviceLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="14d56-103">createDeviceLogCollectionRequest action</span></span>

<span data-ttu-id="14d56-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14d56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14d56-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14d56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14d56-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14d56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14d56-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="14d56-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14d56-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14d56-108">Prerequisites</span></span>
<span data-ttu-id="14d56-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="14d56-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="14d56-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14d56-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14d56-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14d56-111">Permission type</span></span>|<span data-ttu-id="14d56-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14d56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14d56-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14d56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14d56-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14d56-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="14d56-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14d56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14d56-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14d56-116">Not supported.</span></span>|
|<span data-ttu-id="14d56-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14d56-117">Application</span></span>|<span data-ttu-id="14d56-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14d56-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14d56-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14d56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/comanagedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
```

## <a name="request-headers"></a><span data-ttu-id="14d56-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14d56-120">Request headers</span></span>
|<span data-ttu-id="14d56-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14d56-121">Header</span></span>|<span data-ttu-id="14d56-122">Valor</span><span class="sxs-lookup"><span data-stu-id="14d56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14d56-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="14d56-123">Authorization</span></span>|<span data-ttu-id="14d56-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14d56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14d56-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14d56-125">Accept</span></span>|<span data-ttu-id="14d56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14d56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14d56-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14d56-127">Request body</span></span>
<span data-ttu-id="14d56-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="14d56-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="14d56-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="14d56-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="14d56-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14d56-130">Property</span></span>|<span data-ttu-id="14d56-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="14d56-131">Type</span></span>|<span data-ttu-id="14d56-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="14d56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14d56-133">templateType</span><span class="sxs-lookup"><span data-stu-id="14d56-133">templateType</span></span>|[<span data-ttu-id="14d56-134">deviceLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="14d56-134">deviceLogCollectionRequest</span></span>](../resources/intune-devices-devicelogcollectionrequest.md)|<span data-ttu-id="14d56-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="14d56-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="14d56-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="14d56-136">Response</span></span>
<span data-ttu-id="14d56-137">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14d56-137">If successful, this action returns a `200 OK` response code and a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14d56-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14d56-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="14d56-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14d56-139">Request</span></span>
<span data-ttu-id="14d56-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14d56-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest

Content-type: application/json
Content-length: 153

{
  "templateType": {
    "@odata.type": "microsoft.graph.deviceLogCollectionRequest",
    "id": "Id value",
    "templateType": "predefined"
  }
}
```

### <a name="response"></a><span data-ttu-id="14d56-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="14d56-141">Response</span></span>
<span data-ttu-id="14d56-142">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="14d56-142">Here is an example of the response.</span></span> <span data-ttu-id="14d56-143">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="14d56-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="14d56-144">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="14d56-144">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
    "id": "05fb97dc-97dc-05fb-dc97-fb05dc97fb05",
    "status": "Status value",
    "managedDeviceId": "3b336f00-6f00-3b33-006f-333b006f333b",
    "errorCode": 9,
    "requestedDateTimeUTC": "2016-12-31T23:57:40.7845755-08:00",
    "receivedDateTimeUTC": "2016-12-31T23:59:48.6545758-08:00",
    "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
    "expirationDateTimeUTC": "2017-01-01T00:02:49.2157996-08:00",
    "size": 1.3333333333333333
  }
}
```



