---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Recuperar itens de uma lista do SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: b89716d31db34e68e3e54b1b9ef45e6392d63ca6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598080"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="06298-102">Enumerar itens em uma lista</span><span class="sxs-lookup"><span data-stu-id="06298-102">Enumerate items in a list</span></span>

<span data-ttu-id="06298-103">Obter a coleção de [itens][item] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="06298-103">Get the collection of [items][item] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="06298-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="06298-105">Permissions</span></span>

<span data-ttu-id="06298-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06298-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06298-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06298-108">Permission type</span></span>      | <span data-ttu-id="06298-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06298-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06298-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06298-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06298-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06298-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="06298-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06298-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06298-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06298-113">Not supported.</span></span>    |
|<span data-ttu-id="06298-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06298-114">Application</span></span> | <span data-ttu-id="06298-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06298-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06298-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06298-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="06298-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06298-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="06298-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06298-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="06298-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="06298-119">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="06298-120">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="06298-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="06298-121">Basic</span><span class="sxs-lookup"><span data-stu-id="06298-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-items-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06298-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06298-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-items-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
