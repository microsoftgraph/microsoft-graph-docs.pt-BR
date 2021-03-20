---
title: Listar riskDetection
description: Recupere as propriedades de uma coleção de **objeto riskDetection.**
localization_priority: Normal
author: cloudhandler
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e7e0bb9eba36a3b6fdbd6ae03db718dc210d5424
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955511"
---
# <a name="list-riskdetection"></a><span data-ttu-id="17f9a-103">Listar riskDetection</span><span class="sxs-lookup"><span data-stu-id="17f9a-103">List riskDetection</span></span>

<span data-ttu-id="17f9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17f9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17f9a-105">Recupere as propriedades de uma coleção de **objetos riskDetection.**</span><span class="sxs-lookup"><span data-stu-id="17f9a-105">Retrieve the properties of a collection of **riskDetection** objects.</span></span>

>[!NOTE]
><span data-ttu-id="17f9a-106">Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de riscos.</span><span class="sxs-lookup"><span data-stu-id="17f9a-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="17f9a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="17f9a-107">Permissions</span></span>

<span data-ttu-id="17f9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17f9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17f9a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17f9a-110">Permission type</span></span>      | <span data-ttu-id="17f9a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17f9a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17f9a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17f9a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="17f9a-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="17f9a-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="17f9a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17f9a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17f9a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17f9a-115">Not supported.</span></span>    |
|<span data-ttu-id="17f9a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17f9a-116">Application</span></span> | <span data-ttu-id="17f9a-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="17f9a-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17f9a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17f9a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections
GET /identityProtection/riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17f9a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="17f9a-119">Optional query parameters</span></span>

<span data-ttu-id="17f9a-120">Este método oferece `$filter` suporte e para personalizar a resposta de `$select` consulta.</span><span class="sxs-lookup"><span data-stu-id="17f9a-120">This method supports `$filter` and `$select` to customize the query response.</span></span> <span data-ttu-id="17f9a-121">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="17f9a-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="17f9a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17f9a-122">Request headers</span></span>

| <span data-ttu-id="17f9a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="17f9a-123">Name</span></span>      |<span data-ttu-id="17f9a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="17f9a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="17f9a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="17f9a-125">Authorization</span></span>  | <span data-ttu-id="17f9a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17f9a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17f9a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17f9a-128">Content-Type</span></span> | <span data-ttu-id="17f9a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="17f9a-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="17f9a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17f9a-130">Request body</span></span>

<span data-ttu-id="17f9a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17f9a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17f9a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="17f9a-132">Response</span></span>

<span data-ttu-id="17f9a-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos riskDetection](../resources/riskdetection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17f9a-133">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="17f9a-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="17f9a-134">Examples</span></span>


### <a name="example-1-list-risk-detections"></a><span data-ttu-id="17f9a-135">Exemplo 1: Listar detecções de risco</span><span class="sxs-lookup"><span data-stu-id="17f9a-135">Example 1: List risk detections</span></span>

#### <a name="request"></a><span data-ttu-id="17f9a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17f9a-136">Request</span></span>

<span data-ttu-id="17f9a-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17f9a-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17f9a-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="17f9a-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="17f9a-139">C#</span><span class="sxs-lookup"><span data-stu-id="17f9a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17f9a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17f9a-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17f9a-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17f9a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17f9a-142">Java</span><span class="sxs-lookup"><span data-stu-id="17f9a-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskdetection-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17f9a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="17f9a-143">Response</span></span>

<span data-ttu-id="17f9a-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17f9a-144">Here is an example of the response.</span></span>
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

### <a name="example-2-list-risk-detections-for-a-specific-user"></a><span data-ttu-id="17f9a-145">Exemplo 2: Listar detecções de risco para um usuário específico</span><span class="sxs-lookup"><span data-stu-id="17f9a-145">Example 2: List risk detections for a specific user</span></span>

#### <a name="request"></a><span data-ttu-id="17f9a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17f9a-146">Request</span></span>

<span data-ttu-id="17f9a-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17f9a-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17f9a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="17f9a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3
```
# <a name="c"></a>[<span data-ttu-id="17f9a-149">C#</span><span class="sxs-lookup"><span data-stu-id="17f9a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17f9a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17f9a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17f9a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17f9a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17f9a-152">Java</span><span class="sxs-lookup"><span data-stu-id="17f9a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskdetection-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17f9a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="17f9a-153">Response</span></span>

<span data-ttu-id="17f9a-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17f9a-154">Here is an example of the response.</span></span>
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

### <a name="example-3-list-risk-detections-and-filter-the-results"></a><span data-ttu-id="17f9a-155">Exemplo 3: Listar detecções de risco e filtrar os resultados</span><span class="sxs-lookup"><span data-stu-id="17f9a-155">Example 3: List risk detections and filter the results</span></span>

#### <a name="request"></a><span data-ttu-id="17f9a-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17f9a-156">Request</span></span>

<span data-ttu-id="17f9a-157">O exemplo a seguir mostra como usar para obter a coleção de detecções de risco onde o nível de risco é médio ou o tipo de evento de risco é unfamilarFeatures, o que indica que a entrar estava em um local desconhecido ou `$filter` anômalo.</span><span class="sxs-lookup"><span data-stu-id="17f9a-157">The following example shows how to use `$filter` to get the collection of risk detections where the risk level is medium or the risk event type is unfamilarFeatures, which indicates the sign-in was in an unfamiliar or anomalous location.</span></span>


# <a name="http"></a>[<span data-ttu-id="17f9a-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="17f9a-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskDetections"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityProtection/riskDetections?$filter=riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'
```
# <a name="c"></a>[<span data-ttu-id="17f9a-159">C#</span><span class="sxs-lookup"><span data-stu-id="17f9a-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskdetections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17f9a-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17f9a-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskdetections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17f9a-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17f9a-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskdetections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17f9a-162">Java</span><span class="sxs-lookup"><span data-stu-id="17f9a-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-filter-riskdetections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17f9a-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="17f9a-163">Response</span></span>

<span data-ttu-id="17f9a-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17f9a-164">Here is an example of the response.</span></span>
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


