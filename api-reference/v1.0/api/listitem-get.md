---
author: JeremyKelley
ms.author: JeremyKelley
title: Obter listItem
description: Retorna os metadados de um item em uma lista do SharePoint.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a498947002247541bebf4fc7cd24147a0ca0df7a
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968783"
---
# <a name="get-listitem"></a><span data-ttu-id="726f8-103">Obter listItem</span><span class="sxs-lookup"><span data-stu-id="726f8-103">Get listItem</span></span>

<span data-ttu-id="726f8-104">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="726f8-104">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="726f8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="726f8-107">Permissions</span></span>

<span data-ttu-id="726f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="726f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="726f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="726f8-110">Permission type</span></span>      | <span data-ttu-id="726f8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="726f8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="726f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="726f8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="726f8-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="726f8-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="726f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="726f8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="726f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="726f8-115">Not supported.</span></span>    |
|<span data-ttu-id="726f8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="726f8-116">Application</span></span> | <span data-ttu-id="726f8-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="726f8-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="726f8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="726f8-118">HTTP request</span></span>

<span data-ttu-id="726f8-119">Obter um listItem</span><span class="sxs-lookup"><span data-stu-id="726f8-119">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="726f8-120">Obter os valores de coluna de um listItem</span><span class="sxs-lookup"><span data-stu-id="726f8-120">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="726f8-121">Obter valores de coluna específicos de um listItem</span><span class="sxs-lookup"><span data-stu-id="726f8-121">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="726f8-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="726f8-122">Optional query parameters</span></span>
<span data-ttu-id="726f8-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="726f8-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="726f8-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="726f8-124">Request headers</span></span>

| <span data-ttu-id="726f8-125">Nome</span><span class="sxs-lookup"><span data-stu-id="726f8-125">Name</span></span>      |<span data-ttu-id="726f8-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="726f8-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="726f8-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="726f8-127">Authorization</span></span>  | <span data-ttu-id="726f8-128">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="726f8-128">Bearer {code}.</span></span> <span data-ttu-id="726f8-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="726f8-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="726f8-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="726f8-130">Request body</span></span>

<span data-ttu-id="726f8-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="726f8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="726f8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="726f8-132">Response</span></span> 

<span data-ttu-id="726f8-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um [item][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="726f8-133">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="726f8-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="726f8-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="726f8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="726f8-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="726f8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="726f8-136">Response</span></span>

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

#### <a name="sdk-sample-code"></a><span data-ttu-id="726f8-137">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="726f8-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="726f8-138">C#</span><span class="sxs-lookup"><span data-stu-id="726f8-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="726f8-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="726f8-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
