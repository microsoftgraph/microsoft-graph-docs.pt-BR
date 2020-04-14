---
title: Obter countryNamedLocation
description: Recupere as propriedades e os relacionamentos de um objeto countryNamedlocation.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f4a5c55cf4130e9a02afd102416c93efcee441f1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387066"
---
# <a name="get-countrynamedlocation"></a><span data-ttu-id="20342-103">Obter countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="20342-103">Get countryNamedLocation</span></span>

<span data-ttu-id="20342-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20342-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20342-105">Recupere as propriedades e os relacionamentos de um objeto [countryNamedLocation](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="20342-105">Retrieve the properties and relationships of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="20342-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20342-106">Permissions</span></span>

<span data-ttu-id="20342-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20342-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20342-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20342-109">Permission type</span></span>                        | <span data-ttu-id="20342-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20342-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="20342-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20342-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="20342-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="20342-112">Policy.Read.All</span></span> |
| <span data-ttu-id="20342-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20342-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20342-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20342-114">Not supported.</span></span> |
| <span data-ttu-id="20342-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20342-115">Application</span></span>                            | <span data-ttu-id="20342-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="20342-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20342-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20342-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20342-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20342-118">Optional query parameters</span></span>

<span data-ttu-id="20342-119">Este método oferece suporte `select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="20342-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="20342-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="20342-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="20342-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20342-121">Request headers</span></span>

| <span data-ttu-id="20342-122">Nome</span><span class="sxs-lookup"><span data-stu-id="20342-122">Name</span></span>      |<span data-ttu-id="20342-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="20342-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20342-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="20342-124">Authorization</span></span> | <span data-ttu-id="20342-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20342-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20342-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20342-127">Request body</span></span>

<span data-ttu-id="20342-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20342-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20342-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="20342-129">Response</span></span>

<span data-ttu-id="20342-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [countryNamedLocation](../resources/countrynamedlocation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20342-130">If successful, this method returns a `200 OK` response code and the requested [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20342-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20342-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20342-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20342-132">Request</span></span>

<span data-ttu-id="20342-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20342-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20342-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="20342-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_countrynamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="c"></a>[<span data-ttu-id="20342-135">C#</span><span class="sxs-lookup"><span data-stu-id="20342-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20342-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20342-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20342-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20342-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20342-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="20342-138">Response</span></span>

<span data-ttu-id="20342-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20342-139">The following is an example of the response.</span></span>

> <span data-ttu-id="20342-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20342-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
