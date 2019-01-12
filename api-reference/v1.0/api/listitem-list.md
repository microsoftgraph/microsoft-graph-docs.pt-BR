---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Recuperar itens de uma lista do SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 3739997cdc5410ecffbf21277ecff1497b60a190
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968635"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="5c88c-102">Enumerar itens em uma lista</span><span class="sxs-lookup"><span data-stu-id="5c88c-102">Enumerate items in a list</span></span>

<span data-ttu-id="5c88c-103">Obter a coleção de [itens][item] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="5c88c-103">Get the collection of [items][item] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="5c88c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c88c-105">Permissions</span></span>

<span data-ttu-id="5c88c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c88c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c88c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c88c-108">Permission type</span></span>      | <span data-ttu-id="5c88c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c88c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c88c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c88c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c88c-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c88c-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c88c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c88c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c88c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c88c-113">Not supported.</span></span>    |
|<span data-ttu-id="5c88c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c88c-114">Application</span></span> | <span data-ttu-id="5c88c-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c88c-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c88c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c88c-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="5c88c-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c88c-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5c88c-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c88c-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="5c88c-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c88c-119">Response</span></span>

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
  "tocPath": "ListItem/Enumerate"
} -->
