---
author: JeremyKelley
ms.author: JeremyKelley
title: Obter listItem
description: Retorna os metadados de um item em uma lista do SharePoint.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 57d95b67ff27ff58e26310db69f97c027d5e3639
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271992"
---
# <a name="get-listitem"></a><span data-ttu-id="ab68b-103">Obter listItem</span><span class="sxs-lookup"><span data-stu-id="ab68b-103">Get listItem</span></span>

<span data-ttu-id="ab68b-104">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="ab68b-104">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="ab68b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab68b-107">Permissions</span></span>

<span data-ttu-id="ab68b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab68b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab68b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab68b-110">Permission type</span></span>      | <span data-ttu-id="ab68b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab68b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab68b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab68b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ab68b-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab68b-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab68b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab68b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab68b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab68b-115">Not supported.</span></span>    |
|<span data-ttu-id="ab68b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab68b-116">Application</span></span> | <span data-ttu-id="ab68b-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab68b-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab68b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab68b-118">HTTP request</span></span>

<span data-ttu-id="ab68b-119">Obter um listItem</span><span class="sxs-lookup"><span data-stu-id="ab68b-119">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="ab68b-120">Obter os valores de coluna de um listItem</span><span class="sxs-lookup"><span data-stu-id="ab68b-120">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="ab68b-121">Obter valores de coluna específicos de um listItem</span><span class="sxs-lookup"><span data-stu-id="ab68b-121">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ab68b-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab68b-122">Optional query parameters</span></span>
<span data-ttu-id="ab68b-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab68b-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab68b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab68b-124">Request headers</span></span>

| <span data-ttu-id="ab68b-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ab68b-125">Name</span></span>      |<span data-ttu-id="ab68b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab68b-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab68b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab68b-127">Authorization</span></span>  | <span data-ttu-id="ab68b-128">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="ab68b-128">Bearer {code}.</span></span> <span data-ttu-id="ab68b-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab68b-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab68b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab68b-130">Request body</span></span>

<span data-ttu-id="ab68b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab68b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab68b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab68b-132">Response</span></span> 

<span data-ttu-id="ab68b-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um [item][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab68b-133">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab68b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab68b-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab68b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab68b-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="ab68b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab68b-136">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

#### <a name="sdk-sample-code"></a><span data-ttu-id="ab68b-137">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="ab68b-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ab68b-138">C#</span><span class="sxs-lookup"><span data-stu-id="ab68b-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ab68b-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="ab68b-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ab68b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab68b-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
