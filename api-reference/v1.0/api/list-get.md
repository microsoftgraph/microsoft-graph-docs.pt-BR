---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Obter uma lista do SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 9e667055b47568d712349c6725bd4ebc70aa63fd
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482347"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="aa586-102">Obter metadados de uma lista</span><span class="sxs-lookup"><span data-stu-id="aa586-102">Get metadata for a list</span></span>

<span data-ttu-id="aa586-103">Retorna os metadados de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="aa586-103">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="aa586-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa586-105">Permissions</span></span>

<span data-ttu-id="aa586-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa586-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa586-108">Permission type</span></span>      | <span data-ttu-id="aa586-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa586-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa586-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa586-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aa586-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa586-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="aa586-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa586-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa586-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa586-113">Not supported.</span></span>    |
|<span data-ttu-id="aa586-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa586-114">Application</span></span> | <span data-ttu-id="aa586-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa586-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa586-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa586-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="aa586-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa586-117">Request body</span></span>

<span data-ttu-id="aa586-118">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="aa586-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="aa586-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa586-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="aa586-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa586-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="aa586-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa586-121">Response</span></span>

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

<span data-ttu-id="aa586-122">Com instruções `select` e `expand`, você pode recuperar metadados de lista, definições de coluna e itens de lista em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa586-122">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="aa586-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa586-123">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="aa586-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa586-124">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata"
} -->
