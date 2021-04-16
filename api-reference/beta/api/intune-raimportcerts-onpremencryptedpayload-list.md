---
title: Listar onPremEncryptedPayloads
description: Listar propriedades e relações dos objetos onPremEncryptedPayload.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08da9a9efa869d674ab90a676924a6f99853196a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868253"
---
# <a name="list-onpremencryptedpayloads"></a><span data-ttu-id="a6536-103">Listar onPremEncryptedPayloads</span><span class="sxs-lookup"><span data-stu-id="a6536-103">List onPremEncryptedPayloads</span></span>

<span data-ttu-id="a6536-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6536-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6536-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6536-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6536-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6536-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6536-107">Listar propriedades e relações dos [objetos onPremEncryptedPayload.](../resources/intune-raimportcerts-onpremencryptedpayload.md)</span><span class="sxs-lookup"><span data-stu-id="a6536-107">List properties and relationships of the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6536-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6536-108">Prerequisites</span></span>
<span data-ttu-id="a6536-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6536-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6536-111">Permission type</span></span>|<span data-ttu-id="a6536-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6536-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6536-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6536-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6536-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6536-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6536-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6536-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6536-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6536-116">Not supported.</span></span>|
|<span data-ttu-id="a6536-117">Application</span><span class="sxs-lookup"><span data-stu-id="a6536-117">Application</span></span>|<span data-ttu-id="a6536-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6536-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6536-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6536-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="a6536-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6536-120">Request headers</span></span>
|<span data-ttu-id="a6536-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6536-121">Header</span></span>|<span data-ttu-id="a6536-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6536-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6536-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6536-123">Authorization</span></span>|<span data-ttu-id="a6536-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6536-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6536-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6536-125">Accept</span></span>|<span data-ttu-id="a6536-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6536-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6536-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6536-127">Request body</span></span>
<span data-ttu-id="a6536-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6536-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6536-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6536-129">Response</span></span>
<span data-ttu-id="a6536-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6536-130">If successful, this method returns a `200 OK` response code and a collection of [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6536-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6536-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6536-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6536-132">Request</span></span>
<span data-ttu-id="a6536-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6536-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/onPremEncryptedPayloads
```

### <a name="response"></a><span data-ttu-id="a6536-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6536-134">Response</span></span>
<span data-ttu-id="a6536-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6536-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




