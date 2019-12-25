---
author: JeremyKelley
title: Obter metadados de uma lista
description: Retornar os metadados de uma lista.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 9083b4fe61b6603e854fd45b33573731cab65277
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869483"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="61158-103">Obter metadados de uma lista</span><span class="sxs-lookup"><span data-stu-id="61158-103">Get metadata for a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61158-104">Retornar os metadados de uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="61158-104">Return the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="61158-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="61158-106">Permissions</span></span>

<span data-ttu-id="61158-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61158-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61158-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61158-109">Permission type</span></span>      | <span data-ttu-id="61158-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61158-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61158-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61158-111">Delegated (work or school account)</span></span> | <span data-ttu-id="61158-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61158-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="61158-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61158-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61158-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61158-114">Not supported.</span></span>    |
|<span data-ttu-id="61158-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61158-115">Application</span></span> | <span data-ttu-id="61158-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61158-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61158-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61158-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="61158-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61158-118">Request body</span></span>

<span data-ttu-id="61158-119">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="61158-119">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="61158-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61158-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="61158-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61158-121">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="61158-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="61158-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="61158-123">C#</span><span class="sxs-lookup"><span data-stu-id="61158-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="61158-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61158-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="61158-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61158-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="61158-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="61158-126">Response</span></span>

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

<span data-ttu-id="61158-127">Com instruções `select` e `expand`, você pode recuperar metadados de lista, definições de coluna e itens de lista em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="61158-127">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="61158-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61158-128">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="61158-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="61158-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="61158-130">C#</span><span class="sxs-lookup"><span data-stu-id="61158-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="61158-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61158-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="61158-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61158-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="61158-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="61158-133">Response</span></span>

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
#### <a name="request"></a><span data-ttu-id="61158-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61158-134">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

<span data-ttu-id="61158-135">O exemplo a seguir mostra como obter metadados para uma lista que contém três colunas: Name, Quantity e Category.</span><span class="sxs-lookup"><span data-stu-id="61158-135">The following example shows how to get metadata for a list that contains three columns: Name, Quantity, and Category.</span></span>
<span data-ttu-id="61158-136">Colunas de [metadados gerenciados](/sharepoint/managed-metadata) como ```Category``` valores de retorno como um par de ID de termo e nome de termo.</span><span class="sxs-lookup"><span data-stu-id="61158-136">[Managed Metadata](/sharepoint/managed-metadata) columns like ```Category``` return values as term ID and term name pair.</span></span>
```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Quantity,Category))
```

#### <a name="response"></a><span data-ttu-id="61158-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="61158-137">Response</span></span>

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
