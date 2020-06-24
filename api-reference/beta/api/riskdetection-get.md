---
title: Obter riskDetection
description: Recupere as propriedades de um objeto **riskdetection** .
localization_priority: Normal
author: cloudhandler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f87245d2f07600afd612273fdf3a28a36db44b78
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863534"
---
# <a name="get-riskdetection"></a><span data-ttu-id="626f7-103">Obter riskDetection</span><span class="sxs-lookup"><span data-stu-id="626f7-103">Get riskDetection</span></span>

<span data-ttu-id="626f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="626f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="626f7-105">Recupere as propriedades de um objeto **riskDetection** .</span><span class="sxs-lookup"><span data-stu-id="626f7-105">Retrieve the properties of a **riskDetection** object.</span></span>

>[!NOTE]
><span data-ttu-id="626f7-106">Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="626f7-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="626f7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="626f7-107">Permissions</span></span>
<span data-ttu-id="626f7-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="626f7-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="626f7-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="626f7-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="626f7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="626f7-110">Permission type</span></span>      | <span data-ttu-id="626f7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="626f7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="626f7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="626f7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="626f7-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="626f7-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="626f7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="626f7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="626f7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="626f7-115">Not supported.</span></span>    |
|<span data-ttu-id="626f7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="626f7-116">Application</span></span> | <span data-ttu-id="626f7-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="626f7-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="626f7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="626f7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections/{id}
GET /identityProtection/riskDetections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="626f7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="626f7-119">Request headers</span></span>
| <span data-ttu-id="626f7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="626f7-120">Name</span></span>      |<span data-ttu-id="626f7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="626f7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="626f7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="626f7-122">Authorization</span></span>  | <span data-ttu-id="626f7-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="626f7-123">Bearer {token}.</span></span> <span data-ttu-id="626f7-124">Required.</span><span class="sxs-lookup"><span data-stu-id="626f7-124">Required.</span></span> |
| <span data-ttu-id="626f7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="626f7-125">Content-Type</span></span> | <span data-ttu-id="626f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="626f7-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="626f7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="626f7-127">Request body</span></span>
<span data-ttu-id="626f7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="626f7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="626f7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="626f7-129">Response</span></span>

<span data-ttu-id="626f7-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [riskDetection](../resources/riskdetection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="626f7-130">If successful, this method returns a `200 OK` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="626f7-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="626f7-131">Examples</span></span>
### <a name="example-1-get-risk-detections"></a><span data-ttu-id="626f7-132">Exemplo 1: obter detecções de risco</span><span class="sxs-lookup"><span data-stu-id="626f7-132">Example 1: Get risk detections</span></span>
#### <a name="request"></a><span data-ttu-id="626f7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="626f7-133">Request</span></span>
<span data-ttu-id="626f7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="626f7-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="626f7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="626f7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="626f7-136">C#</span><span class="sxs-lookup"><span data-stu-id="626f7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="626f7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="626f7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="626f7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="626f7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="626f7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="626f7-139">Response</span></span>
<span data-ttu-id="626f7-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="626f7-140">Here is an example of the response.</span></span>
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
### <a name="example-2-get-risk-detections-for-specific-user"></a><span data-ttu-id="626f7-141">Exemplo 2: obter detecções de risco para um usuário específico</span><span class="sxs-lookup"><span data-stu-id="626f7-141">Example 2: Get risk detections for specific user</span></span>
#### <a name="request"></a><span data-ttu-id="626f7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="626f7-142">Request</span></span>
<span data-ttu-id="626f7-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="626f7-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="626f7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="626f7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="626f7-145">C#</span><span class="sxs-lookup"><span data-stu-id="626f7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="626f7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="626f7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="626f7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="626f7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="626f7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="626f7-148">Response</span></span>
<span data-ttu-id="626f7-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="626f7-149">Here is an example of the response.</span></span>
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

