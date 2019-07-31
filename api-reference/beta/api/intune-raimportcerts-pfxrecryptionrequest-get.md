---
title: Obter pfxRecryptionRequest
description: Leia as propriedades e as relações do objeto pfxRecryptionRequest.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e853938bda9881341154572d7a00ceeb251cbb3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984227"
---
# <a name="get-pfxrecryptionrequest"></a><span data-ttu-id="94497-103">Obter pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="94497-103">Get pfxRecryptionRequest</span></span>

> <span data-ttu-id="94497-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94497-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94497-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94497-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94497-106">Leia as propriedades e as relações do objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="94497-106">Read properties and relationships of the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94497-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94497-107">Prerequisites</span></span>
<span data-ttu-id="94497-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94497-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94497-110">Permission type</span></span>|<span data-ttu-id="94497-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94497-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94497-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94497-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94497-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="94497-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="94497-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94497-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94497-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94497-115">Not supported.</span></span>|
|<span data-ttu-id="94497-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94497-116">Application</span></span>|<span data-ttu-id="94497-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94497-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94497-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94497-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94497-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94497-119">Optional query parameters</span></span>
<span data-ttu-id="94497-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94497-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94497-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94497-121">Request headers</span></span>
|<span data-ttu-id="94497-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94497-122">Header</span></span>|<span data-ttu-id="94497-123">Valor</span><span class="sxs-lookup"><span data-stu-id="94497-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94497-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="94497-124">Authorization</span></span>|<span data-ttu-id="94497-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94497-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94497-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94497-126">Accept</span></span>|<span data-ttu-id="94497-127">application/json</span><span class="sxs-lookup"><span data-stu-id="94497-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94497-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94497-128">Request body</span></span>
<span data-ttu-id="94497-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94497-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94497-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="94497-130">Response</span></span>
<span data-ttu-id="94497-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94497-131">If successful, this method returns a `200 OK` response code and [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94497-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94497-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="94497-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94497-133">Request</span></span>
<span data-ttu-id="94497-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94497-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

### <a name="response"></a><span data-ttu-id="94497-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="94497-135">Response</span></span>
<span data-ttu-id="94497-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94497-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

{
  "value": {
    "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
    "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
    "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
    "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
    "profileId": "6389d896-d896-6389-96d8-896396d88963",
    "thumbprint": "Thumbprint value",
    "deviceKeyThumbprint": "Device Key Thumbprint value",
    "status": 6,
    "sourceType": 10,
    "createdTime": "2017-01-01T00:03:18.9597073-08:00",
    "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
    "isDeleted": true,
    "eTag": "ETag value"
  }
}
```





