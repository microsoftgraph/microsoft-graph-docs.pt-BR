---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Recuperar itens de uma lista do SharePoint
ms.openlocfilehash: a7f66db11ef201d0ae5afb2cc49887ee10dc89d7
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="07be1-102">Enumerar itens em uma lista</span><span class="sxs-lookup"><span data-stu-id="07be1-102">Enumerate items in a list</span></span>

<span data-ttu-id="07be1-103">Obter a coleção de [itens][item] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="07be1-103">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="07be1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="07be1-105">Permissions</span></span>

<span data-ttu-id="07be1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="07be1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="07be1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07be1-108">Permission type</span></span>      | <span data-ttu-id="07be1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07be1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07be1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07be1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="07be1-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07be1-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="07be1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07be1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07be1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07be1-113">Not supported.</span></span>    |
|<span data-ttu-id="07be1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07be1-114">Application</span></span> | <span data-ttu-id="07be1-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07be1-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07be1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07be1-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="07be1-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07be1-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="07be1-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07be1-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="07be1-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="07be1-119">Response</span></span>

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
