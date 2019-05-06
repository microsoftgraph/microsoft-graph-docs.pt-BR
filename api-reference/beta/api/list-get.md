---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Obter uma lista do SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 3d161245f88954211b07567b326397cabc16716a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598523"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="833f7-102">Obter metadados de uma lista</span><span class="sxs-lookup"><span data-stu-id="833f7-102">Get metadata for a list</span></span>

<span data-ttu-id="833f7-103">Retorna os metadados de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="833f7-103">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="833f7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="833f7-105">Permissions</span></span>

<span data-ttu-id="833f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="833f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="833f7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="833f7-108">Permission type</span></span>      | <span data-ttu-id="833f7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="833f7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="833f7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="833f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="833f7-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="833f7-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="833f7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="833f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="833f7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="833f7-113">Not supported.</span></span>    |
|<span data-ttu-id="833f7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="833f7-114">Application</span></span> | <span data-ttu-id="833f7-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="833f7-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="833f7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="833f7-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="833f7-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="833f7-117">Request body</span></span>

<span data-ttu-id="833f7-118">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="833f7-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="833f7-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="833f7-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="833f7-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="833f7-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="833f7-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="833f7-121">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1234-112-112-4",
  "name": "MicroFeed",
  "createdDateTime": "2016-08-30T08:32:00Z",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "list": {
    "hidden": false,
    "template": "genericList"
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="833f7-122">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="833f7-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="833f7-123">Basic</span><span class="sxs-lookup"><span data-stu-id="833f7-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="833f7-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="833f7-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="833f7-125">Com instruções `select` e `expand`, você pode recuperar metadados de lista, definições de coluna e itens de lista em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="833f7-125">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="833f7-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="833f7-126">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="833f7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="833f7-127">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1234-112-112-4",
  "name": "Inventory",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "columns": [
    {
      "name": "Name",
      "description": "Customer-facing name of the SKU"
    },
    {
      "name": "Color",
      "description": "Color of the item in stock"
    },
    {
      "name": "Quantity",
      "description": "Number of items in stock"
    }
  ],
  "items": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Color": "Red",
        "Quantity": 503
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Color": "Blue",
        "Quantity": 2357
       }
    },
    {
      "id": "7",
      "fields": {
        "Name": "Gizmo",
        "Color": "Green",
        "Quantity": 92
       }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="833f7-128">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="833f7-128">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="833f7-129">Basic</span><span class="sxs-lookup"><span data-stu-id="833f7-129">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-multi-expand-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="833f7-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="833f7-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-multi-expand-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
