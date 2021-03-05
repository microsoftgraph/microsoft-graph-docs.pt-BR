---
title: Listar riskDetections
description: Obter uma lista dos objetos riskDetection e suas propriedades.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 92e521575e18c51874dc954cd61db18b5c8d5808
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440098"
---
# <a name="list-riskdetections"></a><span data-ttu-id="75fb0-103">Listar riskDetections</span><span class="sxs-lookup"><span data-stu-id="75fb0-103">List riskDetections</span></span>
<span data-ttu-id="75fb0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75fb0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75fb0-105">Obter uma lista dos [objetos riskDetection](../resources/riskdetection.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="75fb0-105">Get a list of the [riskDetection](../resources/riskdetection.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="75fb0-106">Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de riscos.</span><span class="sxs-lookup"><span data-stu-id="75fb0-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="75fb0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="75fb0-107">Permissions</span></span>
<span data-ttu-id="75fb0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="75fb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="75fb0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75fb0-110">Permission type</span></span>      | <span data-ttu-id="75fb0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75fb0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75fb0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75fb0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75fb0-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="75fb0-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="75fb0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75fb0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75fb0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75fb0-115">Not supported.</span></span>    |
|<span data-ttu-id="75fb0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75fb0-116">Application</span></span> | <span data-ttu-id="75fb0-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="75fb0-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="75fb0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75fb0-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75fb0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="75fb0-119">Optional query parameters</span></span>
<span data-ttu-id="75fb0-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="75fb0-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="75fb0-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="75fb0-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="75fb0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75fb0-122">Request headers</span></span>
|<span data-ttu-id="75fb0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="75fb0-123">Name</span></span>|<span data-ttu-id="75fb0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="75fb0-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="75fb0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="75fb0-125">Authorization</span></span>|<span data-ttu-id="75fb0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75fb0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75fb0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75fb0-128">Request body</span></span>
<span data-ttu-id="75fb0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75fb0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75fb0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="75fb0-130">Response</span></span>

<span data-ttu-id="75fb0-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos riskDetection](../resources/riskdetection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75fb0-131">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75fb0-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="75fb0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75fb0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75fb0-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskdetection"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections
```


### <a name="response"></a><span data-ttu-id="75fb0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="75fb0-134">Response</span></span>
<span data-ttu-id="75fb0-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="75fb0-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskDetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
  {
    "@odata.type": "#microsoft.graph.riskDetection",
    "id": "6a5874ca-abcd-9d82-5ad39bd71600",
    "requestId": "6a5874ca-abcd-9d82-5ad39bd71600",
    "correlationId": "abcd74ca-9823-4b1c-9d82-5ad39bd71600",
    "riskEventType": "unfamiliarFeatures",
    "riskState": "remediated",
    "riskLevel": "medium",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "source": "activeDirectory",
    "detectionTimingType": "realtime",
    "activity": "signin",
    "tokenIssuerType": "Azure Active Directory",
    "ipAddress": "123.456.7.89",
    "location": {
        "city": "Seattle",
        "state": "Washington",
        "countryOrRegion": "US",
        "geoCoordinates": null
    },
    "activityDateTime": "2018-09-05T00:09:18.7822851Z",
    "detectedDateTime": "2018-09-05T00:11:27.773602Z",
    "lastUpdatedDateTime": "2018-09-05T00:11:27.773602Z",
    "userId": "abcdefab-af90-4edf-ac4c-742ff06735d0",
    "userDisplayName": "Olivia Lack",
    "userPrincipalName": "olack@adatum.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
  ]
}
```


