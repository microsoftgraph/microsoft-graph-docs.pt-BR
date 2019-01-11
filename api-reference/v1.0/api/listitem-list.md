---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Recuperar itens de uma lista do SharePoint
localization_priority: Priority
ms.openlocfilehash: 865d6040aa2a7daaef1ed62c61c45f1e525ded54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812989"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="8b6b0-102">Enumerar itens em uma lista</span><span class="sxs-lookup"><span data-stu-id="8b6b0-102">Enumerate items in a list</span></span>

<span data-ttu-id="8b6b0-103">Obter a coleção de [itens][item] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="8b6b0-103">Get the collection of [items][item] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="8b6b0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b6b0-105">Permissions</span></span>

<span data-ttu-id="8b6b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b6b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b6b0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b6b0-108">Permission type</span></span>      | <span data-ttu-id="8b6b0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b6b0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b6b0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b6b0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8b6b0-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b6b0-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8b6b0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b6b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b6b0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b6b0-113">Not supported.</span></span>    |
|<span data-ttu-id="8b6b0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b6b0-114">Application</span></span> | <span data-ttu-id="8b6b0-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b6b0-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b6b0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b6b0-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="8b6b0-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b6b0-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8b6b0-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b6b0-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="8b6b0-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b6b0-119">Response</span></span>

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
