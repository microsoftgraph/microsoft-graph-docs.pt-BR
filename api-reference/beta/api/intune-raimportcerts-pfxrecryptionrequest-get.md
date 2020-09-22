---
title: Obter pfxRecryptionRequest
description: Leia as propriedades e as relações do objeto pfxRecryptionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1bf1fe7aca0faa0c6db809bae8609ded72200ec5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093214"
---
# <a name="get-pfxrecryptionrequest"></a><span data-ttu-id="7d105-103">Obter pfxRecryptionRequest</span><span class="sxs-lookup"><span data-stu-id="7d105-103">Get pfxRecryptionRequest</span></span>

<span data-ttu-id="7d105-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d105-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d105-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d105-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d105-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d105-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d105-107">Leia as propriedades e as relações do objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="7d105-107">Read properties and relationships of the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d105-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d105-108">Prerequisites</span></span>
<span data-ttu-id="7d105-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d105-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d105-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d105-111">Permission type</span></span>|<span data-ttu-id="7d105-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d105-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d105-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d105-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d105-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d105-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7d105-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d105-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d105-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d105-116">Not supported.</span></span>|
|<span data-ttu-id="7d105-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d105-117">Application</span></span>|<span data-ttu-id="7d105-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d105-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d105-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d105-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d105-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d105-120">Optional query parameters</span></span>
<span data-ttu-id="7d105-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d105-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d105-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d105-122">Request headers</span></span>
|<span data-ttu-id="7d105-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d105-123">Header</span></span>|<span data-ttu-id="7d105-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7d105-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d105-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d105-125">Authorization</span></span>|<span data-ttu-id="7d105-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d105-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d105-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d105-127">Accept</span></span>|<span data-ttu-id="7d105-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7d105-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d105-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d105-129">Request body</span></span>
<span data-ttu-id="7d105-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d105-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d105-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d105-131">Response</span></span>
<span data-ttu-id="7d105-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d105-132">If successful, this method returns a `200 OK` response code and [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d105-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d105-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d105-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d105-134">Request</span></span>
<span data-ttu-id="7d105-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d105-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxRecryptionRequests/{pfxRecryptionRequestsId}
```

### <a name="response"></a><span data-ttu-id="7d105-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d105-136">Response</span></span>
<span data-ttu-id="7d105-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d105-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






