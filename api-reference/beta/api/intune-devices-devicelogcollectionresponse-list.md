---
title: Listar deviceLogCollectionResponses
description: Listar Propriedades e relações dos objetos deviceLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b8abd07487cbd491b6310022757a14d01e160db7
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124162"
---
# <a name="list-devicelogcollectionresponses"></a><span data-ttu-id="1dced-103">Listar deviceLogCollectionResponses</span><span class="sxs-lookup"><span data-stu-id="1dced-103">List deviceLogCollectionResponses</span></span>

<span data-ttu-id="1dced-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dced-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dced-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1dced-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dced-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1dced-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dced-107">Listar Propriedades e relações dos objetos [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="1dced-107">List properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dced-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1dced-108">Prerequisites</span></span>
<span data-ttu-id="1dced-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1dced-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1dced-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dced-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dced-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dced-111">Permission type</span></span>|<span data-ttu-id="1dced-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1dced-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dced-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dced-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1dced-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dced-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1dced-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dced-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dced-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dced-116">Not supported.</span></span>|
|<span data-ttu-id="1dced-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dced-117">Application</span></span>|<span data-ttu-id="1dced-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dced-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dced-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dced-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="1dced-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dced-120">Request headers</span></span>
|<span data-ttu-id="1dced-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1dced-121">Header</span></span>|<span data-ttu-id="1dced-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1dced-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dced-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dced-123">Authorization</span></span>|<span data-ttu-id="1dced-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dced-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dced-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1dced-125">Accept</span></span>|<span data-ttu-id="1dced-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1dced-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dced-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dced-127">Request body</span></span>
<span data-ttu-id="1dced-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1dced-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dced-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dced-129">Response</span></span>
<span data-ttu-id="1dced-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dced-130">If successful, this method returns a `200 OK` response code and a collection of [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dced-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dced-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dced-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dced-132">Request</span></span>
<span data-ttu-id="1dced-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dced-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

### <a name="response"></a><span data-ttu-id="1dced-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dced-134">Response</span></span>
<span data-ttu-id="1dced-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1dced-135">Here is an example of the response.</span></span> <span data-ttu-id="1dced-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1dced-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1dced-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1dced-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 601

{
  "value": [
    {
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
  ]
}
```



