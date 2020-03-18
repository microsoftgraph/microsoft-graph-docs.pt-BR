---
title: Obter onPremEncryptedPayload
description: Leia as propriedades e as relações do objeto onPremEncryptedPayload.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ba6ad43f3c119d8eb2b9b7df7974661d91abbb5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801933"
---
# <a name="get-onpremencryptedpayload"></a><span data-ttu-id="548e4-103">Obter onPremEncryptedPayload</span><span class="sxs-lookup"><span data-stu-id="548e4-103">Get onPremEncryptedPayload</span></span>

> <span data-ttu-id="548e4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="548e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="548e4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="548e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="548e4-106">Leia as propriedades e as relações do objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) .</span><span class="sxs-lookup"><span data-stu-id="548e4-106">Read properties and relationships of the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="548e4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="548e4-107">Prerequisites</span></span>
<span data-ttu-id="548e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="548e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="548e4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="548e4-110">Permission type</span></span>|<span data-ttu-id="548e4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="548e4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="548e4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="548e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="548e4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="548e4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="548e4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="548e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="548e4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="548e4-115">Not supported.</span></span>|
|<span data-ttu-id="548e4-116">Application</span><span class="sxs-lookup"><span data-stu-id="548e4-116">Application</span></span>|<span data-ttu-id="548e4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="548e4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="548e4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="548e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="548e4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="548e4-119">Optional query parameters</span></span>
<span data-ttu-id="548e4-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="548e4-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="548e4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="548e4-121">Request headers</span></span>
|<span data-ttu-id="548e4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="548e4-122">Header</span></span>|<span data-ttu-id="548e4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="548e4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="548e4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="548e4-124">Authorization</span></span>|<span data-ttu-id="548e4-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="548e4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="548e4-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="548e4-126">Accept</span></span>|<span data-ttu-id="548e4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="548e4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="548e4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="548e4-128">Request body</span></span>
<span data-ttu-id="548e4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="548e4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="548e4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="548e4-130">Response</span></span>
<span data-ttu-id="548e4-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="548e4-131">If successful, this method returns a `200 OK` response code and [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="548e4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="548e4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="548e4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="548e4-133">Request</span></span>
<span data-ttu-id="548e4-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="548e4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

### <a name="response"></a><span data-ttu-id="548e4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="548e4-135">Response</span></span>
<span data-ttu-id="548e4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="548e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": {
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
}
```




