---
author: JeremyKelley
description: Obter a coleção de itens em uma lista.
ms.date: 09/11/2017
title: Recuperar itens de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a32e43182bfdd9837ec06da08bdb5aa7c004921f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415370"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="094b4-103">Enumerar itens em uma lista</span><span class="sxs-lookup"><span data-stu-id="094b4-103">Enumerate items in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="094b4-104">Obter a coleção de [itens][item] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="094b4-104">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="094b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="094b4-106">Permissions</span></span>

<span data-ttu-id="094b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="094b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="094b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="094b4-109">Permission type</span></span>      | <span data-ttu-id="094b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="094b4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="094b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="094b4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="094b4-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="094b4-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="094b4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="094b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="094b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="094b4-114">Not supported.</span></span>    |
|<span data-ttu-id="094b4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="094b4-115">Application</span></span> | <span data-ttu-id="094b4-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="094b4-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="094b4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="094b4-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="094b4-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="094b4-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="094b4-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="094b4-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="094b4-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="094b4-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="094b4-121">C#</span><span class="sxs-lookup"><span data-stu-id="094b4-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="094b4-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="094b4-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="094b4-123">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="094b4-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="094b4-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="094b4-124">Response</span></span>

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
