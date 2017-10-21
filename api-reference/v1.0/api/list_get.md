---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Obter uma lista do SharePoint
ms.openlocfilehash: a58a85ed752c00722d2381df10cd7bfb51fbcd3c
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="6b3b4-102">Obter metadados de uma lista</span><span class="sxs-lookup"><span data-stu-id="6b3b4-102">Get metadata for a OneDrive item</span></span>

<span data-ttu-id="6b3b4-103">Retorna os metadados de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="6b3b4-103">Retrieves the metadata for a specified list.</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="6b3b4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b3b4-105">Permissions</span></span>

<span data-ttu-id="6b3b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b3b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6b3b4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b3b4-108">Permission type</span></span>      | <span data-ttu-id="6b3b4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b3b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b3b4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b3b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6b3b4-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b3b4-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b3b4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b3b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b3b4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b3b4-113">Not supported.</span></span>    |
|<span data-ttu-id="6b3b4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3b4-114">Application</span></span> | <span data-ttu-id="6b3b4-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b3b4-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b3b4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b3b4-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="6b3b4-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b3b4-117">Request body</span></span>

<span data-ttu-id="6b3b4-118">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="6b3b4-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="6b3b4-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b3b4-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6b3b4-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b3b4-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="6b3b4-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b3b4-121">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

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

<span data-ttu-id="6b3b4-122">Com instruções `select` e `expand`, você pode recuperar metadados de lista, definições de coluna e itens de lista em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b3b4-122">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="6b3b4-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b3b4-123">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="6b3b4-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b3b4-124">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata"
} -->
