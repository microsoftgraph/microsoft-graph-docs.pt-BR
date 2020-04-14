---
title: Listar pfxRecryptionRequests
description: Listar Propriedades e relações dos objetos pfxRecryptionRequest.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 428bbe055378a9f39afccd452f73ce5976a52c36
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437739"
---
# <a name="list-pfxrecryptionrequests"></a><span data-ttu-id="b8f15-103">Listar pfxRecryptionRequests</span><span class="sxs-lookup"><span data-stu-id="b8f15-103">List pfxRecryptionRequests</span></span>

<span data-ttu-id="b8f15-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8f15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8f15-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8f15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8f15-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8f15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8f15-107">Listar Propriedades e relações dos objetos [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="b8f15-107">List properties and relationships of the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8f15-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8f15-108">Prerequisites</span></span>
<span data-ttu-id="b8f15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8f15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8f15-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8f15-111">Permission type</span></span>|<span data-ttu-id="b8f15-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8f15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8f15-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8f15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8f15-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8f15-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b8f15-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8f15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8f15-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8f15-116">Not supported.</span></span>|
|<span data-ttu-id="b8f15-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8f15-117">Application</span></span>|<span data-ttu-id="b8f15-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8f15-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8f15-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8f15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="b8f15-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8f15-120">Request headers</span></span>
|<span data-ttu-id="b8f15-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8f15-121">Header</span></span>|<span data-ttu-id="b8f15-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b8f15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8f15-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8f15-123">Authorization</span></span>|<span data-ttu-id="b8f15-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8f15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8f15-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8f15-125">Accept</span></span>|<span data-ttu-id="b8f15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8f15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8f15-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8f15-127">Request body</span></span>
<span data-ttu-id="b8f15-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8f15-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8f15-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8f15-129">Response</span></span>
<span data-ttu-id="b8f15-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8f15-130">If successful, this method returns a `200 OK` response code and a collection of [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8f15-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8f15-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8f15-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8f15-132">Request</span></span>
<span data-ttu-id="b8f15-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8f15-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxRecryptionRequests
```

### <a name="response"></a><span data-ttu-id="b8f15-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8f15-134">Response</span></span>
<span data-ttu-id="b8f15-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8f15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

{
  "value": [
    {
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
  ]
}
```



