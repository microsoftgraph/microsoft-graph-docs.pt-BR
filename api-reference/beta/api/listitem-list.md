---
author: JeremyKelley
description: Obter a coleção de itens em uma lista.
ms.date: 09/11/2017
title: Recuperar itens de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: dd188f69ea39acf98117231ad6c153852cb4f5b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993050"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="3814a-103">Enumerar itens em uma lista</span><span class="sxs-lookup"><span data-stu-id="3814a-103">Enumerate items in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3814a-104">Obter a coleção de [itens][item] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="3814a-104">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="3814a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3814a-106">Permissions</span></span>

<span data-ttu-id="3814a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3814a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3814a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3814a-109">Permission type</span></span>      | <span data-ttu-id="3814a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3814a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3814a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3814a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3814a-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3814a-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3814a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3814a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3814a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3814a-114">Not supported.</span></span>    |
|<span data-ttu-id="3814a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3814a-115">Application</span></span> | <span data-ttu-id="3814a-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3814a-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3814a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3814a-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="3814a-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3814a-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3814a-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3814a-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3814a-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="3814a-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3814a-121">C#</span><span class="sxs-lookup"><span data-stu-id="3814a-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3814a-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="3814a-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3814a-123">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3814a-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3814a-124">Java</span><span class="sxs-lookup"><span data-stu-id="3814a-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3814a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3814a-125">Response</span></span>

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
