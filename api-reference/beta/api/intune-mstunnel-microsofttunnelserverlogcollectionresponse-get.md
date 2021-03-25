---
title: Obter microsoftTunnelServerLogCollectionResponse
description: Leia propriedades e relações do objeto microsoftTunnelServerLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a1f384f10f2b91e835628fd1d435bc5bf70a15ae
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153017"
---
# <a name="get-microsofttunnelserverlogcollectionresponse"></a><span data-ttu-id="678be-103">Obter microsoftTunnelServerLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="678be-103">Get microsoftTunnelServerLogCollectionResponse</span></span>

<span data-ttu-id="678be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="678be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="678be-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="678be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="678be-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="678be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="678be-107">Leia propriedades e relações do [objeto microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="678be-107">Read properties and relationships of the [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="678be-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="678be-108">Prerequisites</span></span>
<span data-ttu-id="678be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="678be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="678be-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="678be-111">Permission type</span></span>|<span data-ttu-id="678be-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="678be-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="678be-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="678be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="678be-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="678be-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="678be-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="678be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="678be-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="678be-116">Not supported.</span></span>|
|<span data-ttu-id="678be-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="678be-117">Application</span></span>|<span data-ttu-id="678be-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="678be-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="678be-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="678be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelServerLogCollectionResponses/{microsoftTunnelServerLogCollectionResponseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="678be-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="678be-120">Optional query parameters</span></span>
<span data-ttu-id="678be-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="678be-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="678be-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="678be-122">Request headers</span></span>
|<span data-ttu-id="678be-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="678be-123">Header</span></span>|<span data-ttu-id="678be-124">Valor</span><span class="sxs-lookup"><span data-stu-id="678be-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="678be-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="678be-125">Authorization</span></span>|<span data-ttu-id="678be-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="678be-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="678be-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="678be-127">Accept</span></span>|<span data-ttu-id="678be-128">application/json</span><span class="sxs-lookup"><span data-stu-id="678be-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="678be-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="678be-129">Request body</span></span>
<span data-ttu-id="678be-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="678be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="678be-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="678be-131">Response</span></span>
<span data-ttu-id="678be-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="678be-132">If successful, this method returns a `200 OK` response code and [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="678be-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="678be-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="678be-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="678be-134">Request</span></span>
<span data-ttu-id="678be-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="678be-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelServerLogCollectionResponses/{microsoftTunnelServerLogCollectionResponseId}
```

### <a name="response"></a><span data-ttu-id="678be-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="678be-136">Response</span></span>
<span data-ttu-id="678be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="678be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
    "id": "05dcc2e9-c2e9-05dc-e9c2-dc05e9c2dc05",
    "status": "completed",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
    "sizeInBytes": 11
  }
}
```




