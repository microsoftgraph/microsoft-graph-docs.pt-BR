---
title: Listar riskDetection
description: Recupere as propriedades de uma coleção de **objeto riskDetection.**
localization_priority: Normal
author: cloudhandler
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d6308ba07530d8fd3c13e3d9e9e6e089c008176c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443612"
---
# <a name="list-riskdetection"></a><span data-ttu-id="e4a10-103">Listar riskDetection</span><span class="sxs-lookup"><span data-stu-id="e4a10-103">List riskDetection</span></span>

<span data-ttu-id="e4a10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4a10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4a10-105">Recupere as propriedades de uma coleção de **objetos riskDetection.**</span><span class="sxs-lookup"><span data-stu-id="e4a10-105">Retrieve the properties of a collection of **riskDetection** objects.</span></span>

>[!NOTE]
><span data-ttu-id="e4a10-106">Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de riscos.</span><span class="sxs-lookup"><span data-stu-id="e4a10-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4a10-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4a10-107">Permissions</span></span>

<span data-ttu-id="e4a10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4a10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4a10-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4a10-110">Permission type</span></span>      | <span data-ttu-id="e4a10-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4a10-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4a10-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4a10-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e4a10-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a10-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="e4a10-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4a10-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4a10-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4a10-115">Not supported.</span></span>    |
|<span data-ttu-id="e4a10-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4a10-116">Application</span></span> | <span data-ttu-id="e4a10-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4a10-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4a10-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4a10-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections
GET /identityProtection/riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4a10-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e4a10-119">Optional query parameters</span></span>

<span data-ttu-id="e4a10-120">Este método oferece `$filter` suporte e para personalizar a resposta de `$select` consulta.</span><span class="sxs-lookup"><span data-stu-id="e4a10-120">This method supports `$filter` and `$select` to customize the query response.</span></span> <span data-ttu-id="e4a10-121">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="e4a10-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="e4a10-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a10-122">Request headers</span></span>

| <span data-ttu-id="e4a10-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e4a10-123">Name</span></span>      |<span data-ttu-id="e4a10-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4a10-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e4a10-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4a10-125">Authorization</span></span>  | <span data-ttu-id="e4a10-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4a10-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e4a10-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4a10-128">Content-Type</span></span> | <span data-ttu-id="e4a10-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e4a10-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4a10-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a10-130">Request body</span></span>

<span data-ttu-id="e4a10-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e4a10-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4a10-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4a10-132">Response</span></span>

<span data-ttu-id="e4a10-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos riskDetection](../resources/riskdetection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4a10-133">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4a10-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e4a10-134">Examples</span></span>


### <a name="example-1-list-risk-detections"></a><span data-ttu-id="e4a10-135">Exemplo 1: Listar detecções de risco</span><span class="sxs-lookup"><span data-stu-id="e4a10-135">Example 1: List risk detections</span></span>

#### <a name="request"></a><span data-ttu-id="e4a10-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a10-136">Request</span></span>

<span data-ttu-id="e4a10-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4a10-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e4a10-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4a10-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="e4a10-139">C#</span><span class="sxs-lookup"><span data-stu-id="e4a10-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4a10-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4a10-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4a10-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4a10-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4a10-142">Java</span><span class="sxs-lookup"><span data-stu-id="e4a10-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskdetection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e4a10-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4a10-143">Response</span></span>

<span data-ttu-id="e4a10-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4a10-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
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
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

### <a name="example-2-list-risk-detections-for-a-specific-user"></a><span data-ttu-id="e4a10-145">Exemplo 2: Listar detecções de risco para um usuário específico</span><span class="sxs-lookup"><span data-stu-id="e4a10-145">Example 2: List risk detections for a specific user</span></span>

#### <a name="request"></a><span data-ttu-id="e4a10-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a10-146">Request</span></span>

<span data-ttu-id="e4a10-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4a10-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e4a10-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4a10-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="e4a10-149">C#</span><span class="sxs-lookup"><span data-stu-id="e4a10-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4a10-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4a10-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4a10-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4a10-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4a10-152">Java</span><span class="sxs-lookup"><span data-stu-id="e4a10-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskdetection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e4a10-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4a10-153">Response</span></span>

<span data-ttu-id="e4a10-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4a10-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
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
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

### <a name="example-3-list-risk-detections-and-filter-the-results"></a><span data-ttu-id="e4a10-155">Exemplo 3: Listar detecções de risco e filtrar os resultados</span><span class="sxs-lookup"><span data-stu-id="e4a10-155">Example 3: List risk detections and filter the results</span></span>

#### <a name="request"></a><span data-ttu-id="e4a10-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a10-156">Request</span></span>

<span data-ttu-id="e4a10-157">O exemplo a seguir mostra como usar para obter a coleção de detecções de risco onde o nível de risco é médio ou o tipo de evento de risco é unfamilarFeatures, o que indica que a entrar estava em um local desconhecido ou `$filter` anômalo.</span><span class="sxs-lookup"><span data-stu-id="e4a10-157">The following example shows how to use `$filter` to get the collection of risk detections where the risk level is medium or the risk event type is unfamilarFeatures, which indicates the sign-in was in an unfamiliar or anomalous location.</span></span>


# <a name="http"></a>[<span data-ttu-id="e4a10-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4a10-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskDetections"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections?$filter=riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'
```
# <a name="c"></a>[<span data-ttu-id="e4a10-159">C#</span><span class="sxs-lookup"><span data-stu-id="e4a10-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskdetections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4a10-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4a10-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskdetections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4a10-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4a10-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskdetections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4a10-162">Java</span><span class="sxs-lookup"><span data-stu-id="e4a10-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskdetections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e4a10-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4a10-163">Response</span></span>

<span data-ttu-id="e4a10-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4a10-164">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskDetection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
    "id": "1d68fc3d60d012ff80ad4b16818bf304df1bde295fdf1db31fa5389ba9532cd1",
    "requestId": "3295073e-04b1-4871-9d15-c1f871b41100",
    "correlationId": "f141d8e5-93e9-4fd0-9eb0-c40e5f8fc092",
    "riskEventType": "unfamiliarFeatures",
    "riskState": "atRisk",
    "riskLevel": "medium",
    "riskDetail": "none",
    "source": "Identity Protection",
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
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskDetections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


