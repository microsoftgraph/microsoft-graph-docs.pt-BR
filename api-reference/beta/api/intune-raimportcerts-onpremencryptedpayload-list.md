---
title: Listar onPremEncryptedPayloads
description: Listar Propriedades e relações dos objetos onPremEncryptedPayload.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a3895681b59d4bf5d0e2c54c156f77ab4276976
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49233114"
---
# <a name="list-onpremencryptedpayloads"></a><span data-ttu-id="911ee-103">Listar onPremEncryptedPayloads</span><span class="sxs-lookup"><span data-stu-id="911ee-103">List onPremEncryptedPayloads</span></span>

<span data-ttu-id="911ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="911ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="911ee-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="911ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="911ee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="911ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="911ee-107">Listar Propriedades e relações dos objetos [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="911ee-107">List properties and relationships of the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="911ee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="911ee-108">Prerequisites</span></span>
<span data-ttu-id="911ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="911ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="911ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="911ee-111">Permission type</span></span>|<span data-ttu-id="911ee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="911ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="911ee-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="911ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="911ee-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="911ee-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="911ee-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="911ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="911ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="911ee-116">Not supported.</span></span>|
|<span data-ttu-id="911ee-117">Application</span><span class="sxs-lookup"><span data-stu-id="911ee-117">Application</span></span>|<span data-ttu-id="911ee-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="911ee-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="911ee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="911ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="911ee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="911ee-120">Request headers</span></span>
|<span data-ttu-id="911ee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="911ee-121">Header</span></span>|<span data-ttu-id="911ee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="911ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="911ee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="911ee-123">Authorization</span></span>|<span data-ttu-id="911ee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="911ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="911ee-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="911ee-125">Accept</span></span>|<span data-ttu-id="911ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="911ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="911ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="911ee-127">Request body</span></span>
<span data-ttu-id="911ee-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="911ee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="911ee-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="911ee-129">Response</span></span>
<span data-ttu-id="911ee-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="911ee-130">If successful, this method returns a `200 OK` response code and a collection of [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="911ee-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="911ee-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="911ee-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="911ee-132">Request</span></span>
<span data-ttu-id="911ee-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="911ee-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/onPremEncryptedPayloads
```

### <a name="response"></a><span data-ttu-id="911ee-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="911ee-134">Response</span></span>
<span data-ttu-id="911ee-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="911ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




