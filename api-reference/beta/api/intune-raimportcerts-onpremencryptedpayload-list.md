---
title: Listar onPremEncryptedPayloads
description: Listar Propriedades e relações dos objetos onPremEncryptedPayload.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a54946f9d24268127778f96257cafdcbd153c2b
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161596"
---
# <a name="list-onpremencryptedpayloads"></a><span data-ttu-id="a77f7-103">Listar onPremEncryptedPayloads</span><span class="sxs-lookup"><span data-stu-id="a77f7-103">List onPremEncryptedPayloads</span></span>

> <span data-ttu-id="a77f7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a77f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a77f7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a77f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a77f7-106">Listar Propriedades e relações dos objetos [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="a77f7-106">List properties and relationships of the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a77f7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a77f7-107">Prerequisites</span></span>
<span data-ttu-id="a77f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a77f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a77f7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a77f7-110">Permission type</span></span>|<span data-ttu-id="a77f7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a77f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a77f7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a77f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a77f7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a77f7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a77f7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a77f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a77f7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a77f7-115">Not supported.</span></span>|
|<span data-ttu-id="a77f7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a77f7-116">Application</span></span>|<span data-ttu-id="a77f7-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a77f7-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a77f7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a77f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="a77f7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a77f7-119">Request headers</span></span>
|<span data-ttu-id="a77f7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a77f7-120">Header</span></span>|<span data-ttu-id="a77f7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a77f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a77f7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a77f7-122">Authorization</span></span>|<span data-ttu-id="a77f7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a77f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a77f7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a77f7-124">Accept</span></span>|<span data-ttu-id="a77f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a77f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a77f7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a77f7-126">Request body</span></span>
<span data-ttu-id="a77f7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a77f7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a77f7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a77f7-128">Response</span></span>
<span data-ttu-id="a77f7-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a77f7-129">If successful, this method returns a `200 OK` response code and a collection of [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a77f7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a77f7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a77f7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a77f7-131">Request</span></span>
<span data-ttu-id="a77f7-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a77f7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/onPremEncryptedPayloads
```

### <a name="response"></a><span data-ttu-id="a77f7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a77f7-133">Response</span></span>
<span data-ttu-id="a77f7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a77f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 882

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
      "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
      "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
      "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
      "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
      "deviceKeyThumbprint": "Device Key Thumbprint value",
      "cert1PayloadUUID": "Cert1Payload UUID value",
      "cert2PayloadUUID": "Cert2Payload UUID value",
      "cert3PayloadUUID": "Cert3Payload UUID value",
      "plistTemplate": "Plist Template value",
      "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
      "payloadVersion": 14,
      "status": 6,
      "createdTime": "2017-01-01T00:03:18.9597073-08:00",
      "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
      "eTag": "ETag value",
      "isDeleted": true
    }
  ]
}
```





