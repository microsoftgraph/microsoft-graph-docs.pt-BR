---
title: Obter riskDetection
description: Recupere as propriedades de um **objeto riskdetection.**
localization_priority: Normal
author: cloudhandler
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 84093741d434686a9957ca657978406fe6156da7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954182"
---
# <a name="get-riskdetection"></a><span data-ttu-id="f0545-103">Obter riskDetection</span><span class="sxs-lookup"><span data-stu-id="f0545-103">Get riskDetection</span></span>

<span data-ttu-id="f0545-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0545-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0545-105">Recupere as propriedades de um **objeto riskDetection.**</span><span class="sxs-lookup"><span data-stu-id="f0545-105">Retrieve the properties of a **riskDetection** object.</span></span>

>[!NOTE]
><span data-ttu-id="f0545-106">Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de riscos.</span><span class="sxs-lookup"><span data-stu-id="f0545-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0545-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0545-107">Permissions</span></span>
<span data-ttu-id="f0545-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0545-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0545-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0545-110">Permission type</span></span>      | <span data-ttu-id="f0545-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0545-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0545-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0545-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f0545-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0545-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="f0545-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0545-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0545-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0545-115">Not supported.</span></span>    |
|<span data-ttu-id="f0545-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0545-116">Application</span></span> | <span data-ttu-id="f0545-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0545-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0545-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0545-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections/{id}
GET /identityProtection/riskDetections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f0545-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0545-119">Request headers</span></span>
| <span data-ttu-id="f0545-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f0545-120">Name</span></span>      |<span data-ttu-id="f0545-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0545-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0545-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0545-122">Authorization</span></span>  | <span data-ttu-id="f0545-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0545-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0545-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0545-125">Content-Type</span></span> | <span data-ttu-id="f0545-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0545-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0545-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0545-127">Request body</span></span>
<span data-ttu-id="f0545-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0545-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0545-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0545-129">Response</span></span>

<span data-ttu-id="f0545-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [riskDetection](../resources/riskdetection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0545-130">If successful, this method returns a `200 OK` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0545-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f0545-131">Examples</span></span>
### <a name="example-1-get-risk-detections"></a><span data-ttu-id="f0545-132">Exemplo 1: Obter detecções de risco</span><span class="sxs-lookup"><span data-stu-id="f0545-132">Example 1: Get risk detections</span></span>
#### <a name="request"></a><span data-ttu-id="f0545-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0545-133">Request</span></span>
<span data-ttu-id="f0545-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0545-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0545-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0545-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection_1",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="f0545-136">C#</span><span class="sxs-lookup"><span data-stu-id="f0545-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0545-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0545-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0545-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0545-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0545-139">Java</span><span class="sxs-lookup"><span data-stu-id="f0545-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskdetection-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f0545-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0545-140">Response</span></span>
<span data-ttu-id="f0545-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0545-141">Here is an example of the response.</span></span>
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
### <a name="example-2-get-risk-detections-for-specific-user"></a><span data-ttu-id="f0545-142">Exemplo 2: Obter detecções de risco para um usuário específico</span><span class="sxs-lookup"><span data-stu-id="f0545-142">Example 2: Get risk detections for specific user</span></span>
#### <a name="request"></a><span data-ttu-id="f0545-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0545-143">Request</span></span>
<span data-ttu-id="f0545-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0545-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0545-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0545-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskDetection_2",
  "sampleKeys": ["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="f0545-146">C#</span><span class="sxs-lookup"><span data-stu-id="f0545-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskdetection-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0545-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0545-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskdetection-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0545-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0545-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskdetection-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0545-149">Java</span><span class="sxs-lookup"><span data-stu-id="f0545-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskdetection-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f0545-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0545-150">Response</span></span>
<span data-ttu-id="f0545-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0545-151">Here is an example of the response.</span></span>
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



