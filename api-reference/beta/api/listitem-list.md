---
author: JeremyKelley
description: Obter a coleção de itens em uma lista.
ms.date: 09/11/2017
title: Recuperar itens de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 851ccd31068b1cbd9ffa8a237283c79898458fc4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040491"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="36eed-103">Enumerar itens em uma lista</span><span class="sxs-lookup"><span data-stu-id="36eed-103">Enumerate items in a list</span></span>

<span data-ttu-id="36eed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36eed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36eed-105">Obter a coleção de [itens][item] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="36eed-105">Get the collection of [items][item] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="36eed-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="36eed-107">Permissions</span></span>

<span data-ttu-id="36eed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36eed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36eed-110">Permission type</span></span>      | <span data-ttu-id="36eed-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36eed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36eed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36eed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="36eed-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36eed-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="36eed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36eed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36eed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36eed-115">Not supported.</span></span>    |
|<span data-ttu-id="36eed-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36eed-116">Application</span></span> | <span data-ttu-id="36eed-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36eed-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36eed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36eed-118">HTTP request</span></span>

```http
GET /sites/{site-id}/lists/{list-id}/items
GET /sites/{site-id}/lists/{list-id}/items?expand=fields
GET /sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="36eed-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36eed-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="36eed-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36eed-120">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36eed-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="36eed-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="c"></a>[<span data-ttu-id="36eed-122">C#</span><span class="sxs-lookup"><span data-stu-id="36eed-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36eed-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36eed-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36eed-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36eed-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36eed-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="36eed-125">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
  ]
}
-->


