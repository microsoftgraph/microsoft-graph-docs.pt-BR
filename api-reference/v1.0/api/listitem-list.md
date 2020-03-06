---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Recuperar itens de uma lista do SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Obter a coleção de itens em uma lista.
doc_type: apiPageType
ms.openlocfilehash: f42973005e552ce84b1f2613c6012d4404fb5b07
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511688"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="7eac6-103">Enumerar itens em uma lista</span><span class="sxs-lookup"><span data-stu-id="7eac6-103">Enumerate items in a list</span></span>

<span data-ttu-id="7eac6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eac6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7eac6-105">Obter a coleção de [itens][item] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="7eac6-105">Get the collection of [items][item] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="7eac6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7eac6-107">Permissions</span></span>

<span data-ttu-id="7eac6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7eac6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7eac6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7eac6-110">Permission type</span></span>      | <span data-ttu-id="7eac6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7eac6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7eac6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7eac6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7eac6-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7eac6-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7eac6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7eac6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7eac6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7eac6-115">Not supported.</span></span>    |
|<span data-ttu-id="7eac6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7eac6-116">Application</span></span> | <span data-ttu-id="7eac6-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7eac6-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7eac6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7eac6-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="7eac6-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7eac6-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7eac6-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7eac6-120">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7eac6-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="7eac6-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="c"></a>[<span data-ttu-id="7eac6-122">C#</span><span class="sxs-lookup"><span data-stu-id="7eac6-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7eac6-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7eac6-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7eac6-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7eac6-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7eac6-125">Java</span><span class="sxs-lookup"><span data-stu-id="7eac6-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7eac6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7eac6-126">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
  ]
} -->
