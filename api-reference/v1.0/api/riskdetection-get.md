---
title: Obter riskDetection
description: Leia as propriedades e os relacionamentos de um objeto riskDetection.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f03cc204da67ee99c737cb2df8bd9e21bf16477b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897600"
---
# <a name="get-riskdetection"></a><span data-ttu-id="b609f-103">Obter riskDetection</span><span class="sxs-lookup"><span data-stu-id="b609f-103">Get riskDetection</span></span>
<span data-ttu-id="b609f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b609f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b609f-105">Leia as propriedades e os relacionamentos de um objeto [riskDetection](../resources/riskdetection.md) .</span><span class="sxs-lookup"><span data-stu-id="b609f-105">Read the properties and relationships of a [riskDetection](../resources/riskdetection.md) object.</span></span>

>[!NOTE]
><span data-ttu-id="b609f-106">Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="b609f-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="b609f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b609f-107">Permissions</span></span>
<span data-ttu-id="b609f-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b609f-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b609f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="b609f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="b609f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b609f-110">Permission type</span></span>      | <span data-ttu-id="b609f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b609f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b609f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b609f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b609f-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="b609f-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="b609f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b609f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b609f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b609f-115">Not supported.</span></span>    |
|<span data-ttu-id="b609f-116">Application</span><span class="sxs-lookup"><span data-stu-id="b609f-116">Application</span></span> | <span data-ttu-id="b609f-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="b609f-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b609f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b609f-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskDetections/{riskDetectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b609f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b609f-119">Optional query parameters</span></span>
<span data-ttu-id="b609f-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b609f-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b609f-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b609f-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b609f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b609f-122">Request headers</span></span>
|<span data-ttu-id="b609f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b609f-123">Name</span></span>|<span data-ttu-id="b609f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b609f-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b609f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b609f-125">Authorization</span></span>|<span data-ttu-id="b609f-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b609f-126">Bearer {token}.</span></span> <span data-ttu-id="b609f-127">Required.</span><span class="sxs-lookup"><span data-stu-id="b609f-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b609f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b609f-128">Request body</span></span>
<span data-ttu-id="b609f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b609f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b609f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b609f-130">Response</span></span>

<span data-ttu-id="b609f-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [riskDetection](../resources/riskdetection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b609f-131">If successful, this method returns a `200 OK` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b609f-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b609f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b609f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b609f-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskdetection"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```


### <a name="response"></a><span data-ttu-id="b609f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b609f-134">Response</span></span>
<span data-ttu-id="b609f-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b609f-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskDetection"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

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

