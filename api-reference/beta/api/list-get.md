---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Obter uma lista do SharePoint
localization_priority: Normal
ms.openlocfilehash: f3519b707e2e1b5899cbb54b1a52350cc46136ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856956"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="3891d-102">Obter metadados de uma lista</span><span class="sxs-lookup"><span data-stu-id="3891d-102">Get metadata for a list</span></span>

> <span data-ttu-id="3891d-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3891d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3891d-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3891d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3891d-105">Retorna os metadados de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="3891d-105">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="3891d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3891d-107">Permissions</span></span>

<span data-ttu-id="3891d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3891d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3891d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3891d-110">Permission type</span></span>      | <span data-ttu-id="3891d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3891d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3891d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3891d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3891d-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3891d-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3891d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3891d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3891d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3891d-115">Not supported.</span></span>    |
|<span data-ttu-id="3891d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3891d-116">Application</span></span> | <span data-ttu-id="3891d-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3891d-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3891d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3891d-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="3891d-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3891d-119">Request body</span></span>

<span data-ttu-id="3891d-120">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="3891d-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="3891d-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3891d-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3891d-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3891d-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="3891d-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="3891d-123">Response</span></span>

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

<span data-ttu-id="3891d-124">Com instruções `select` e `expand`, você pode recuperar metadados de lista, definições de coluna e itens de lista em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="3891d-124">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="3891d-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3891d-125">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="3891d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3891d-126">Response</span></span>

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
