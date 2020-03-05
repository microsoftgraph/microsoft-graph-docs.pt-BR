---
title: Listar riskDetection
description: Recupere as propriedades de uma coleção do objeto **riskDetection** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 821fb0fe790982ef83a48a4418af2d4c6a144ee4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453909"
---
# <a name="list-riskdetection"></a><span data-ttu-id="e13d3-103">Listar riskDetection</span><span class="sxs-lookup"><span data-stu-id="e13d3-103">List riskDetection</span></span>

<span data-ttu-id="e13d3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e13d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e13d3-105">Recupere as propriedades de uma coleção de objetos **riskDetection** .</span><span class="sxs-lookup"><span data-stu-id="e13d3-105">Retrieve the properties of a collection of **riskDetection** objects.</span></span>

>[!NOTE]
><span data-ttu-id="e13d3-106">Você deve ter uma licença do Azure AD Premium P1 ou P2 para usar a API de detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="e13d3-106">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="e13d3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e13d3-107">Permissions</span></span>

<span data-ttu-id="e13d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e13d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e13d3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e13d3-110">Permission type</span></span>      | <span data-ttu-id="e13d3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e13d3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e13d3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e13d3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e13d3-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e13d3-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="e13d3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e13d3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e13d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e13d3-115">Not supported.</span></span>    |
|<span data-ttu-id="e13d3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e13d3-116">Application</span></span> | <span data-ttu-id="e13d3-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e13d3-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e13d3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e13d3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e13d3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e13d3-119">Optional query parameters</span></span>

<span data-ttu-id="e13d3-120">Este método oferece `$filter` suporte `$select` e para personalizar a resposta de consulta.</span><span class="sxs-lookup"><span data-stu-id="e13d3-120">This method supports `$filter` and `$select` to customize the query response.</span></span> <span data-ttu-id="e13d3-121">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="e13d3-121">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="e13d3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e13d3-122">Request headers</span></span>

| <span data-ttu-id="e13d3-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e13d3-123">Name</span></span>      |<span data-ttu-id="e13d3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e13d3-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e13d3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e13d3-125">Authorization</span></span>  | <span data-ttu-id="e13d3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e13d3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e13d3-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e13d3-128">Content-Type</span></span> | <span data-ttu-id="e13d3-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e13d3-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e13d3-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e13d3-130">Request body</span></span>

<span data-ttu-id="e13d3-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e13d3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e13d3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e13d3-132">Response</span></span>

<span data-ttu-id="e13d3-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [riskDetection](../resources/riskdetection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e13d3-133">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e13d3-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e13d3-134">Examples</span></span>

### <a name="example-1-list-risk-detections"></a><span data-ttu-id="e13d3-135">Exemplo 1: listar detecções de risco</span><span class="sxs-lookup"><span data-stu-id="e13d3-135">Example 1: List risk detections</span></span>

#### <a name="request"></a><span data-ttu-id="e13d3-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e13d3-136">Request</span></span>

<span data-ttu-id="e13d3-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e13d3-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e13d3-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e13d3-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskDetection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections
```
# <a name="c"></a>[<span data-ttu-id="e13d3-139">C#</span><span class="sxs-lookup"><span data-stu-id="e13d3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskdetection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e13d3-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e13d3-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskdetection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e13d3-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e13d3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskdetection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e13d3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e13d3-142">Response</span></span>

<span data-ttu-id="e13d3-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e13d3-143">Here is an example of the response.</span></span>
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
    "userDisplayName": "User ",
    "userPrincipalName": "user@abcde.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"
    }
    ]
}
```

### <a name="example-2-list-risk-detections-and-filter-the-results"></a><span data-ttu-id="e13d3-144">Exemplo 2: listar detecções de risco e filtrar os resultados</span><span class="sxs-lookup"><span data-stu-id="e13d3-144">Example 2: List risk detections and filter the results</span></span>

#### <a name="request"></a><span data-ttu-id="e13d3-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e13d3-145">Request</span></span>

<span data-ttu-id="e13d3-146">O exemplo a seguir mostra como usar `$filter` o para obter a coleção de detecções de risco onde o nível de risco é médio ou o tipo de evento de risco é unfamilarFeatures, que indica que a entrada estava em um local não familiarizado ou anormal.</span><span class="sxs-lookup"><span data-stu-id="e13d3-146">The following example shows how to use `$filter` to get the collection of risk detections where the risk level is medium or the risk event type is unfamilarFeatures, which indicates the sign-in was in an unfamiliar or anomalous location.</span></span>


# <a name="http"></a>[<span data-ttu-id="e13d3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e13d3-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskDetections"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/riskDetections?$filter=riskType eq 'unfamiliarFeatures' or riskLevel eq 'medium'
```
# <a name="c"></a>[<span data-ttu-id="e13d3-148">C#</span><span class="sxs-lookup"><span data-stu-id="e13d3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskdetections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e13d3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e13d3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskdetections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e13d3-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e13d3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskdetections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e13d3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e13d3-151">Response</span></span>

<span data-ttu-id="e13d3-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e13d3-152">Here is an example of the response.</span></span>
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
    "riskType": "unfamiliarFeatures",
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
