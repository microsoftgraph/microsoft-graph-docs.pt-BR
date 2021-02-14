---
author: JeremyKelley
title: Obter uma lista do SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Retorna os metadados de uma lista.
doc_type: apiPageType
ms.openlocfilehash: a1ac1469ab582a6f0b9e1a7e0b78db6bf1b6638f
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238838"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="e015c-103">Obter metadados de uma lista</span><span class="sxs-lookup"><span data-stu-id="e015c-103">Get metadata for a list</span></span>

<span data-ttu-id="e015c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e015c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e015c-105">Retorna os metadados de uma [list][].</span><span class="sxs-lookup"><span data-stu-id="e015c-105">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="e015c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e015c-107">Permissions</span></span>

<span data-ttu-id="e015c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e015c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e015c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e015c-110">Permission type</span></span>                        | <span data-ttu-id="e015c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e015c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e015c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e015c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e015c-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e015c-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="e015c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e015c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e015c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e015c-115">Not supported.</span></span>                              |
| <span data-ttu-id="e015c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e015c-116">Application</span></span>                            | <span data-ttu-id="e015c-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e015c-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="e015c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e015c-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-title}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="e015c-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e015c-119">Request body</span></span>

<span data-ttu-id="e015c-120">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="e015c-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="e015c-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e015c-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e015c-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e015c-122">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e015c-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="e015c-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}
```
# <a name="c"></a>[<span data-ttu-id="e015c-124">C#</span><span class="sxs-lookup"><span data-stu-id="e015c-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e015c-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e015c-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e015c-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e015c-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e015c-127">Java</span><span class="sxs-lookup"><span data-stu-id="e015c-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e015c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e015c-128">Response</span></span>

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

<span data-ttu-id="e015c-129">Com instruções `select` e `expand`, você pode recuperar metadados de lista, definições de coluna e itens de lista em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="e015c-129">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="e015c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e015c-130">Request</span></span>
<span data-ttu-id="e015c-131">O exemplo a seguir mostra como obter uma lista a partir de um título de lista do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="e015c-131">The following example shows how to get a list from a SharePoint Online list title.</span></span>

# <a name="http"></a>[<span data-ttu-id="e015c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e015c-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-title}
```
# <a name="c"></a>[<span data-ttu-id="e015c-133">C#</span><span class="sxs-lookup"><span data-stu-id="e015c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e015c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e015c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e015c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e015c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e015c-136">Java</span><span class="sxs-lookup"><span data-stu-id="e015c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e015c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e015c-137">Response</span></span>

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

<span data-ttu-id="e015c-138">Com instruções `select` e `expand`, você pode recuperar metadados de lista, definições de coluna e itens de lista em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="e015c-138">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="e015c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e015c-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e015c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="e015c-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="c"></a>[<span data-ttu-id="e015c-141">C#</span><span class="sxs-lookup"><span data-stu-id="e015c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e015c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e015c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e015c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e015c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e015c-144">Java</span><span class="sxs-lookup"><span data-stu-id="e015c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e015c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e015c-145">Response</span></span>

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
  "tocPath": "Lists/Get metadata",
  "suppressions": [
  ]
} -->

