---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: c46fed1c2da3ac246212dbbcdfeb35479699efe6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613040"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="5d332-102">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="5d332-102">Get an item in a list</span></span>

<span data-ttu-id="5d332-103">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="5d332-103">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="5d332-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d332-106">Permissions</span></span>

<span data-ttu-id="5d332-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d332-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d332-109">Permission type</span></span>      | <span data-ttu-id="5d332-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d332-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d332-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d332-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5d332-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d332-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d332-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d332-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d332-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d332-114">Not supported.</span></span>    |
|<span data-ttu-id="5d332-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d332-115">Application</span></span> | <span data-ttu-id="5d332-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d332-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d332-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d332-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="5d332-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d332-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5d332-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d332-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="5d332-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d332-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5d332-121">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="5d332-121">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5d332-122">C#</span><span class="sxs-lookup"><span data-stu-id="5d332-122">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d332-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="5d332-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
