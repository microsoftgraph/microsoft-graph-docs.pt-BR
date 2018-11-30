---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Obter uma lista do SharePoint
ms.openlocfilehash: 8cda18e17197a6f14a3c60903fa0c4ad43ed684d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037404"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="e4f7e-102">Obter metadados de uma lista</span><span class="sxs-lookup"><span data-stu-id="e4f7e-102">Get metadata for a list</span></span>

> <span data-ttu-id="e4f7e-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4f7e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4f7e-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4f7e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4f7e-105">Retorna os metadados de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="e4f7e-105">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="e4f7e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4f7e-107">Permissions</span></span>

<span data-ttu-id="e4f7e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4f7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4f7e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4f7e-110">Permission type</span></span>      | <span data-ttu-id="e4f7e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4f7e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4f7e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4f7e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e4f7e-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4f7e-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4f7e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4f7e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4f7e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4f7e-115">Not supported.</span></span>    |
|<span data-ttu-id="e4f7e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4f7e-116">Application</span></span> | <span data-ttu-id="e4f7e-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4f7e-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4f7e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4f7e-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="e4f7e-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4f7e-119">Request body</span></span>

<span data-ttu-id="e4f7e-120">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="e4f7e-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="e4f7e-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4f7e-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e4f7e-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4f7e-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="e4f7e-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4f7e-123">Response</span></span>

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

<span data-ttu-id="e4f7e-124">Com instruções `select` e `expand`, você pode recuperar metadados de lista, definições de coluna e itens de lista em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4f7e-124">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="e4f7e-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4f7e-125">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="e4f7e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4f7e-126">Response</span></span>

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
