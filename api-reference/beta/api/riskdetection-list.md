---
title: Listar riskDetection
description: Recupere as propriedades de uma coleção do objeto **riskDetection** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e019c9c9984ba7bb99b5f10266a333b8f3a07d52
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349326"
---
# <a name="list-riskdetection"></a><span data-ttu-id="7b87b-103">Listar riskDetection</span><span class="sxs-lookup"><span data-stu-id="7b87b-103">List riskDetection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b87b-104">Recupere as propriedades de uma coleção de objetos **riskDetection** .</span><span class="sxs-lookup"><span data-stu-id="7b87b-104">Retrieve the properties of a collection of **riskDetection** objects.</span></span>

>[!NOTE]
><span data-ttu-id="7b87b-105">Você deve ter uma licença do Azure AD Premium P2 para usar a API de detecção de risco.</span><span class="sxs-lookup"><span data-stu-id="7b87b-105">You must have an Azure AD Premium P2 license to use the risk detection API.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b87b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b87b-106">Permissions</span></span>

<span data-ttu-id="7b87b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b87b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b87b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b87b-109">Permission type</span></span>      | <span data-ttu-id="7b87b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b87b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b87b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b87b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b87b-112">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b87b-112">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="7b87b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b87b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b87b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b87b-114">Not supported.</span></span>    |
|<span data-ttu-id="7b87b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b87b-115">Application</span></span> | <span data-ttu-id="7b87b-116">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b87b-116">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b87b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b87b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /riskDetections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b87b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7b87b-118">Optional query parameters</span></span>

<span data-ttu-id="7b87b-119">Este método oferece `$filter` suporte `$select` e para personalizar a resposta de consulta.</span><span class="sxs-lookup"><span data-stu-id="7b87b-119">This method supports `$filter` and `$select` to customize the query response.</span></span> <span data-ttu-id="7b87b-120">Consulte o exemplo mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="7b87b-120">See the example later in this topic.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="7b87b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b87b-121">Request headers</span></span>

| <span data-ttu-id="7b87b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7b87b-122">Name</span></span>      |<span data-ttu-id="7b87b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b87b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b87b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b87b-124">Authorization</span></span>  | <span data-ttu-id="7b87b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b87b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b87b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b87b-127">Content-Type</span></span> | <span data-ttu-id="7b87b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7b87b-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b87b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b87b-129">Request body</span></span>

<span data-ttu-id="7b87b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b87b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b87b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b87b-131">Response</span></span>

<span data-ttu-id="7b87b-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [riskDetection](../resources/riskDetection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b87b-132">If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskDetection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b87b-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7b87b-133">Examples</span></span>

### <a name="example-1-list-risk-detections"></a><span data-ttu-id="7b87b-134">Exemplo 1: listar detecções de risco</span><span class="sxs-lookup"><span data-stu-id="7b87b-134">Example 1: List risk detections</span></span>

#### <a name="request"></a><span data-ttu-id="7b87b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b87b-135">Request</span></span>

<span data-ttu-id="7b87b-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b87b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskDetection"
}-->

```http
GET https://graph.microsoft.com/beta/riskDetections
```

#### <a name="response"></a><span data-ttu-id="7b87b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b87b-137">Response</span></span>

<span data-ttu-id="7b87b-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b87b-138">Here is an example of the response.</span></span>
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

### <a name="example-2-list-risk-detections-and-filter-the-results"></a><span data-ttu-id="7b87b-139">Exemplo 2: listar detecções de risco e filtrar os resultados</span><span class="sxs-lookup"><span data-stu-id="7b87b-139">Example 2: List risk detections and filter the results</span></span>

#### <a name="request"></a><span data-ttu-id="7b87b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b87b-140">Request</span></span>

<span data-ttu-id="7b87b-141">O exemplo a seguir mostra como usar `$filter` o para obter a coleção de detecções de risco onde o nível de risco é médio ou o tipo de evento de risco é unfamilarFeatures, que indica que a entrada estava em um local não familiarizado ou anormal.</span><span class="sxs-lookup"><span data-stu-id="7b87b-141">The following example shows how to use `$filter` to get the collection of risk detections where the risk level is medium or the risk event type is unfamilarFeatures, which indicates the sign-in was in an unfamiliar or anomalous location.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_filter_riskDetections"
} -->

```http
GET https://graph.microsoft.com/beta/riskDetections?$filter=riskType eq 'unfamiliarFeatures' or riskLevel eq 'medium'
```

#### <a name="response"></a><span data-ttu-id="7b87b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b87b-142">Response</span></span>

<span data-ttu-id="7b87b-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b87b-143">Here is an example of the response.</span></span>
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
