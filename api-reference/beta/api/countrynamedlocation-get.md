---
title: Obter countryNamedLocation
description: Recupere as propriedades e as relações de um objeto countryNamedlocation.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6cf9cb310db478ef7481ff514917fc49d5a4b8b9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046997"
---
# <a name="get-countrynamedlocation"></a><span data-ttu-id="42d3e-103">Obter countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="42d3e-103">Get countryNamedLocation</span></span>

<span data-ttu-id="42d3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42d3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42d3e-105">Recupere as propriedades e as relações de um [objeto countryNamedLocation.](../resources/countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="42d3e-105">Retrieve the properties and relationships of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="42d3e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="42d3e-106">Permissions</span></span>

<span data-ttu-id="42d3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42d3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42d3e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42d3e-109">Permission type</span></span>                        | <span data-ttu-id="42d3e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42d3e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="42d3e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42d3e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42d3e-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="42d3e-112">Policy.Read.All</span></span> |
| <span data-ttu-id="42d3e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42d3e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42d3e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42d3e-114">Not supported.</span></span> |
| <span data-ttu-id="42d3e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42d3e-115">Application</span></span>                            | <span data-ttu-id="42d3e-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="42d3e-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42d3e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42d3e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42d3e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="42d3e-118">Optional query parameters</span></span>

<span data-ttu-id="42d3e-119">Este método dá suporte ao `select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="42d3e-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="42d3e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="42d3e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="42d3e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42d3e-121">Request headers</span></span>

| <span data-ttu-id="42d3e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="42d3e-122">Name</span></span>      |<span data-ttu-id="42d3e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="42d3e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42d3e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="42d3e-124">Authorization</span></span> | <span data-ttu-id="42d3e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42d3e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42d3e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42d3e-127">Request body</span></span>

<span data-ttu-id="42d3e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42d3e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42d3e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d3e-129">Response</span></span>

<span data-ttu-id="42d3e-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [countryNamedLocation](../resources/countrynamedlocation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42d3e-130">If successful, this method returns a `200 OK` response code and the requested [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42d3e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="42d3e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42d3e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42d3e-132">Request</span></span>

<span data-ttu-id="42d3e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42d3e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42d3e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="42d3e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_countrynamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="c"></a>[<span data-ttu-id="42d3e-135">C#</span><span class="sxs-lookup"><span data-stu-id="42d3e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42d3e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42d3e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42d3e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42d3e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42d3e-138">Java</span><span class="sxs-lookup"><span data-stu-id="42d3e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-countrynamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42d3e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d3e-139">Response</span></span>

<span data-ttu-id="42d3e-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42d3e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="42d3e-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="42d3e-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


