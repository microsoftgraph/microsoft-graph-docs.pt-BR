---
author: JeremyKelley
title: Obter metadados de uma lista
description: Retornar os metadados de uma lista.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1cce486364a0b630cf79f20a7a63aba7c6592f57
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969746"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="76cfd-103">Obter metadados de uma lista</span><span class="sxs-lookup"><span data-stu-id="76cfd-103">Get metadata for a list</span></span>

<span data-ttu-id="76cfd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76cfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76cfd-105">Retornar os metadados de uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="76cfd-105">Return the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="76cfd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="76cfd-107">Permissions</span></span>

<span data-ttu-id="76cfd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76cfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76cfd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76cfd-110">Permission type</span></span>                        | <span data-ttu-id="76cfd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76cfd-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="76cfd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76cfd-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="76cfd-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76cfd-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="76cfd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76cfd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76cfd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76cfd-115">Not supported.</span></span>                              |
| <span data-ttu-id="76cfd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76cfd-116">Application</span></span>                            | <span data-ttu-id="76cfd-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76cfd-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="76cfd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76cfd-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-title}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="76cfd-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76cfd-119">Request body</span></span>

<span data-ttu-id="76cfd-120">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="76cfd-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="76cfd-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76cfd-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="76cfd-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76cfd-122">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="76cfd-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="76cfd-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}
```
# <a name="c"></a>[<span data-ttu-id="76cfd-124">C#</span><span class="sxs-lookup"><span data-stu-id="76cfd-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76cfd-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76cfd-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76cfd-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76cfd-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="76cfd-127">Java</span><span class="sxs-lookup"><span data-stu-id="76cfd-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="76cfd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="76cfd-128">Response</span></span>

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

<span data-ttu-id="76cfd-129">Com instruções `select` e `expand`, você pode recuperar metadados de lista, definições de coluna e itens de lista em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="76cfd-129">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="76cfd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76cfd-130">Request</span></span>
<span data-ttu-id="76cfd-131">O exemplo a seguir mostra como obter uma lista a partir de um título de lista do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="76cfd-131">The following example shows how to get a list from a SharePoint Online list title.</span></span>

# <a name="http"></a>[<span data-ttu-id="76cfd-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="76cfd-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-title}
```
# <a name="c"></a>[<span data-ttu-id="76cfd-133">C#</span><span class="sxs-lookup"><span data-stu-id="76cfd-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76cfd-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76cfd-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76cfd-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76cfd-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="76cfd-136">Java</span><span class="sxs-lookup"><span data-stu-id="76cfd-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="76cfd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="76cfd-137">Response</span></span>

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

<span data-ttu-id="76cfd-138">Com instruções `select` e `expand`, você pode recuperar metadados de lista, definições de coluna e itens de lista em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="76cfd-138">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="76cfd-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76cfd-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="76cfd-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="76cfd-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="c"></a>[<span data-ttu-id="76cfd-141">C#</span><span class="sxs-lookup"><span data-stu-id="76cfd-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76cfd-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76cfd-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76cfd-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76cfd-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="76cfd-144">Java</span><span class="sxs-lookup"><span data-stu-id="76cfd-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="76cfd-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="76cfd-145">Response</span></span>

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
#### <a name="request"></a><span data-ttu-id="76cfd-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76cfd-146">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

<span data-ttu-id="76cfd-147">O exemplo a seguir mostra como obter metadados para uma lista que contém três colunas: Name, Quantity e Category.</span><span class="sxs-lookup"><span data-stu-id="76cfd-147">The following example shows how to get metadata for a list that contains three columns: Name, Quantity, and Category.</span></span>
<span data-ttu-id="76cfd-148">Colunas de [metadados gerenciados](/sharepoint/managed-metadata) como ```Category``` valores de retorno como um par de ID de termo e nome de termo.</span><span class="sxs-lookup"><span data-stu-id="76cfd-148">[Managed Metadata](/sharepoint/managed-metadata) columns like ```Category``` return values as term ID and term name pair.</span></span>
```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Quantity,Category))
```

#### <a name="response"></a><span data-ttu-id="76cfd-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="76cfd-149">Response</span></span>

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
      "name": "Quantity",
      "description": "Number of items in stock"
    },
    {
      "name": "Category",
      "description": "Category of the item"
    }
  ],
  "items": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Quantity": 503,
        "Category": {
          "termId": "791d537a-9c1c-3b05-97b0-1ce7ece7e1a4",
          "name": "Tool"
         }
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Quantity": 2357,
        "Category": {
          "termId": "902e568b-9b2d-4d06-87c2-2cf8ecf9f2b5" ,
          "name": "Mechanical Device"
         }
       }
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
  ]
}
-->


