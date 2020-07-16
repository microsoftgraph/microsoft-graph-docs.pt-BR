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
# <a name="list-devicelogcollectionresponses"></a><span data-ttu-id="d85c6-103">Listar deviceLogCollectionResponses</span><span class="sxs-lookup"><span data-stu-id="d85c6-103">List deviceLogCollectionResponses</span></span>

<span data-ttu-id="d85c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d85c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d85c6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d85c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d85c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d85c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d85c6-107">Listar Propriedades e relações dos objetos [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="d85c6-107">List properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d85c6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d85c6-108">Prerequisites</span></span>
<span data-ttu-id="d85c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d85c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d85c6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d85c6-111">Permission type</span></span>|<span data-ttu-id="d85c6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d85c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d85c6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d85c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d85c6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d85c6-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d85c6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d85c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d85c6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d85c6-116">Not supported.</span></span>|
|<span data-ttu-id="d85c6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d85c6-117">Application</span></span>|<span data-ttu-id="d85c6-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d85c6-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d85c6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d85c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="d85c6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d85c6-120">Request headers</span></span>
|<span data-ttu-id="d85c6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d85c6-121">Header</span></span>|<span data-ttu-id="d85c6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d85c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d85c6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d85c6-123">Authorization</span></span>|<span data-ttu-id="d85c6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d85c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d85c6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d85c6-125">Accept</span></span>|<span data-ttu-id="d85c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d85c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d85c6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d85c6-127">Request body</span></span>
<span data-ttu-id="d85c6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d85c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d85c6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d85c6-129">Response</span></span>
<span data-ttu-id="d85c6-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d85c6-130">If successful, this method returns a `200 OK` response code and a collection of [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d85c6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d85c6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d85c6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d85c6-132">Request</span></span>
<span data-ttu-id="d85c6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d85c6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

### <a name="response"></a><span data-ttu-id="d85c6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d85c6-134">Response</span></span>
<span data-ttu-id="d85c6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d85c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



