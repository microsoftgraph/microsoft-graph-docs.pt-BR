---
title: Obter riskDetection
description: Recupere as propriedades de um objeto **riskdetection** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1c35a451e6510292bbffd72132e64c82d6ab7c70
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453915"
---
# <a name="get-riskdetection"></a><span data-ttu-id="c88f6-103">Obter riskDetection</span><span class="sxs-lookup"><span data-stu-id="c88f6-103">Get riskDetection</span></span>

<span data-ttu-id="c88f6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c88f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c88f6-105">Recupere as propriedades de um objeto **riskDetection** .</span><span class="sxs-lookup"><span data-stu-id="c88f6-105">Retrieve the properties of a **riskDetection** object.</span></span>

>[!NOTE]
><span data-ttu-id="c88f6-106">Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="c88f6-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="c88f6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c88f6-107">Permissions</span></span>
<span data-ttu-id="c88f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c88f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c88f6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c88f6-110">Permission type</span></span>      | <span data-ttu-id="c88f6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c88f6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c88f6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c88f6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c88f6-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="c88f6-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="c88f6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c88f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c88f6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c88f6-115">Not supported.</span></span>    |
|<span data-ttu-id="c88f6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c88f6-116">Application</span></span> | <span data-ttu-id="c88f6-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="c88f6-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c88f6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c88f6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c88f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c88f6-119">Request headers</span></span>
| <span data-ttu-id="c88f6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c88f6-120">Name</span></span>      |<span data-ttu-id="c88f6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c88f6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c88f6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c88f6-122">Authorization</span></span>  | <span data-ttu-id="c88f6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c88f6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c88f6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c88f6-125">Content-Type</span></span> | <span data-ttu-id="c88f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c88f6-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c88f6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c88f6-127">Request body</span></span>
<span data-ttu-id="c88f6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c88f6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c88f6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c88f6-129">Response</span></span>

<span data-ttu-id="c88f6-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [riskDetection](../resources/riskdetection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c88f6-130">If successful, this method returns a `200 OK` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c88f6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c88f6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c88f6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c88f6-132">Request</span></span>
<span data-ttu-id="c88f6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c88f6-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c88f6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c88f6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="c88f6-135">C#</span><span class="sxs-lookup"><span data-stu-id="c88f6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c88f6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c88f6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c88f6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c88f6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c88f6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c88f6-138">Response</span></span>
<span data-ttu-id="c88f6-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c88f6-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "6a5874ca-abcd-9d82-5ad39bd71600",
    "requestId": "6a5874ca-abcd-9d82-5ad39bd71600",
    "correlationId": "abcd74ca-9823-4b1c-9d82-5ad39bd71600",
    "riskType": "unfamiliarFeatures",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get riskDetection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

