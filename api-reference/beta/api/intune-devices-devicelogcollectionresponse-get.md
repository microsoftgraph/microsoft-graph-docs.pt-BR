---
title: Obter deviceLogCollectionResponse
description: Leia as propriedades e as relações do objeto deviceLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1cb0b477e3d6885cbdd359145b99ce03d4914e32
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732791"
---
# <a name="get-devicelogcollectionresponse"></a><span data-ttu-id="0e276-103">Obter deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="0e276-103">Get deviceLogCollectionResponse</span></span>

<span data-ttu-id="0e276-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e276-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e276-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e276-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e276-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e276-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e276-107">Leia as propriedades e as relações do objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="0e276-107">Read properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e276-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e276-108">Prerequisites</span></span>
<span data-ttu-id="0e276-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e276-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e276-111">Permission type</span></span>|<span data-ttu-id="0e276-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0e276-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e276-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e276-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e276-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e276-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0e276-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e276-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e276-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e276-116">Not supported.</span></span>|
|<span data-ttu-id="0e276-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e276-117">Application</span></span>|<span data-ttu-id="0e276-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e276-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e276-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e276-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e276-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0e276-120">Optional query parameters</span></span>
<span data-ttu-id="0e276-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0e276-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e276-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e276-122">Request headers</span></span>
|<span data-ttu-id="0e276-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e276-123">Header</span></span>|<span data-ttu-id="0e276-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0e276-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e276-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e276-125">Authorization</span></span>|<span data-ttu-id="0e276-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e276-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e276-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e276-127">Accept</span></span>|<span data-ttu-id="0e276-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0e276-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e276-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e276-129">Request body</span></span>
<span data-ttu-id="0e276-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e276-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e276-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e276-131">Response</span></span>
<span data-ttu-id="0e276-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e276-132">If successful, this method returns a `200 OK` response code and [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e276-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e276-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e276-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e276-134">Request</span></span>
<span data-ttu-id="0e276-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e276-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

### <a name="response"></a><span data-ttu-id="0e276-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e276-136">Response</span></span>
<span data-ttu-id="0e276-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e276-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





