---
title: Obter countryNamedLocation
description: Recupere as propriedades e os relacionamentos de um objeto countryNamedlocation.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c049e8c947d931f4173e7a763b3e6b563e5ba36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009965"
---
# <a name="get-countrynamedlocation"></a><span data-ttu-id="4a3c2-103">Obter countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="4a3c2-103">Get countryNamedLocation</span></span>

<span data-ttu-id="4a3c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a3c2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a3c2-105">Recupere as propriedades e os relacionamentos de um objeto [countryNamedLocation](../resources/countryNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="4a3c2-105">Retrieve the properties and relationships of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a3c2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a3c2-106">Permissions</span></span>

<span data-ttu-id="4a3c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a3c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a3c2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a3c2-109">Permission type</span></span>                        | <span data-ttu-id="4a3c2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a3c2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4a3c2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a3c2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a3c2-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a3c2-112">Policy.Read.All</span></span> |
| <span data-ttu-id="4a3c2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a3c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a3c2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a3c2-114">Not supported.</span></span> |
| <span data-ttu-id="4a3c2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a3c2-115">Application</span></span>                            | <span data-ttu-id="4a3c2-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a3c2-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a3c2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a3c2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a3c2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4a3c2-118">Optional query parameters</span></span>

<span data-ttu-id="4a3c2-119">Este método oferece suporte ao `select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4a3c2-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="4a3c2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4a3c2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a3c2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a3c2-121">Request headers</span></span>

| <span data-ttu-id="4a3c2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4a3c2-122">Name</span></span>      |<span data-ttu-id="4a3c2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a3c2-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a3c2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a3c2-124">Authorization</span></span> | <span data-ttu-id="4a3c2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a3c2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a3c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a3c2-127">Request body</span></span>

<span data-ttu-id="4a3c2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a3c2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a3c2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a3c2-129">Response</span></span>

<span data-ttu-id="4a3c2-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [countryNamedLocation](../resources/countrynamedlocation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a3c2-130">If successful, this method returns a `200 OK` response code and the requested [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a3c2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4a3c2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4a3c2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a3c2-132">Request</span></span>

<span data-ttu-id="4a3c2-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a3c2-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4a3c2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a3c2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_countrynamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
```
# <a name="c"></a>[<span data-ttu-id="4a3c2-135">C#</span><span class="sxs-lookup"><span data-stu-id="4a3c2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a3c2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a3c2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a3c2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a3c2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a3c2-138">Java</span><span class="sxs-lookup"><span data-stu-id="4a3c2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-countrynamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4a3c2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a3c2-139">Response</span></span>

<span data-ttu-id="4a3c2-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a3c2-140">The following is an example of the response.</span></span>

> <span data-ttu-id="4a3c2-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a3c2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryNamedLocation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#namedLocations/$entity",
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

