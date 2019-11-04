---
title: Obter countryNamedLocation
description: Recupere as propriedades e os relacionamentos de um objeto countryNamedlocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cda2dfe66858157be397ecf75e68c7a3b5743bb0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937123"
---
# <a name="get-countrynamedlocation"></a><span data-ttu-id="fc29f-103">Obter countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="fc29f-103">Get countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc29f-104">Recupere as propriedades e os relacionamentos de um objeto [countryNamedLocation](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="fc29f-104">Retrieve the properties and relationships of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc29f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc29f-105">Permissions</span></span>

<span data-ttu-id="fc29f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc29f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc29f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc29f-108">Permission type</span></span>                        | <span data-ttu-id="fc29f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc29f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fc29f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc29f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc29f-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc29f-111">Policy.Read.All</span></span> |
| <span data-ttu-id="fc29f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc29f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc29f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc29f-113">Not supported.</span></span> |
| <span data-ttu-id="fc29f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc29f-114">Application</span></span>                            | <span data-ttu-id="fc29f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc29f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc29f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc29f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc29f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fc29f-117">Optional query parameters</span></span>

<span data-ttu-id="fc29f-118">Este método oferece suporte `select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fc29f-118">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="fc29f-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fc29f-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc29f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc29f-120">Request headers</span></span>

| <span data-ttu-id="fc29f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fc29f-121">Name</span></span>      |<span data-ttu-id="fc29f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc29f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fc29f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc29f-123">Authorization</span></span> | <span data-ttu-id="fc29f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc29f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc29f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc29f-126">Request body</span></span>

<span data-ttu-id="fc29f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc29f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc29f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc29f-128">Response</span></span>

<span data-ttu-id="fc29f-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [countryNamedLocation](../resources/countrynamedlocation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc29f-129">If successful, this method returns a `200 OK` response code and the requested [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc29f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fc29f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc29f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc29f-131">Request</span></span>

<span data-ttu-id="fc29f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc29f-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fc29f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc29f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_countrynamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc29f-134">C#</span><span class="sxs-lookup"><span data-stu-id="fc29f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc29f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc29f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc29f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc29f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fc29f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc29f-137">Response</span></span>

<span data-ttu-id="fc29f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fc29f-138">The following is an example of the response.</span></span>

> <span data-ttu-id="fc29f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc29f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryNamedLocation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#namedLocations/$entity",
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "id": "1c4427fd-0885-4a3d-8b23-09a899ffa959",
    "displayName": "Named location with unknown countries and regions",
    "modifiedDateTime": "2019-09-04T01:08:02.5249255Z",
    "createdDateTime": "2019-09-04T01:08:02.5249255Z",
    "countriesAndRegions": [
        "US",
        "GB"
    ],
    "includeUnknownCountriesAndRegions": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get countryNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
