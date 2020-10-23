---
title: Listar pfxRecryptionRequests
description: Listar Propriedades e relações dos objetos pfxRecryptionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 993cf5d7c4b33511d3afc32d8643c62df5af826d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734298"
---
# <a name="list-pfxrecryptionrequests"></a><span data-ttu-id="1e5af-103">Listar pfxRecryptionRequests</span><span class="sxs-lookup"><span data-stu-id="1e5af-103">List pfxRecryptionRequests</span></span>

<span data-ttu-id="1e5af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e5af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e5af-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e5af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e5af-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e5af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e5af-107">Listar Propriedades e relações dos objetos [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="1e5af-107">List properties and relationships of the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e5af-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e5af-108">Prerequisites</span></span>
<span data-ttu-id="1e5af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e5af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e5af-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e5af-111">Permission type</span></span>|<span data-ttu-id="1e5af-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e5af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e5af-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e5af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e5af-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e5af-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1e5af-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e5af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e5af-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e5af-116">Not supported.</span></span>|
|<span data-ttu-id="1e5af-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e5af-117">Application</span></span>|<span data-ttu-id="1e5af-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e5af-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e5af-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e5af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="1e5af-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e5af-120">Request headers</span></span>
|<span data-ttu-id="1e5af-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e5af-121">Header</span></span>|<span data-ttu-id="1e5af-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1e5af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e5af-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e5af-123">Authorization</span></span>|<span data-ttu-id="1e5af-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e5af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e5af-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e5af-125">Accept</span></span>|<span data-ttu-id="1e5af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e5af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e5af-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e5af-127">Request body</span></span>
<span data-ttu-id="1e5af-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e5af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e5af-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e5af-129">Response</span></span>
<span data-ttu-id="1e5af-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e5af-130">If successful, this method returns a `200 OK` response code and a collection of [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e5af-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e5af-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e5af-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e5af-132">Request</span></span>
<span data-ttu-id="1e5af-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e5af-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxRecryptionRequests
```

### <a name="response"></a><span data-ttu-id="1e5af-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e5af-134">Response</span></span>
<span data-ttu-id="1e5af-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e5af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





