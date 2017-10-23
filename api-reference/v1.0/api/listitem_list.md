---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Recuperar itens de uma lista do SharePoint
ms.openlocfilehash: ff414159015b4731b76626e309418c32cb6640d4
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2017
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="66293-102">Enumerar itens em uma lista</span><span class="sxs-lookup"><span data-stu-id="66293-102">Enumerate items in a list</span></span>

<span data-ttu-id="66293-103">Obter a coleção de [itens][item] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="66293-103">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="66293-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="66293-105">Permissions</span></span>

<span data-ttu-id="66293-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="66293-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="66293-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66293-108">Permission type</span></span>      | <span data-ttu-id="66293-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66293-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66293-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66293-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66293-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66293-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="66293-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66293-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66293-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66293-113">Not supported.</span></span>    |
|<span data-ttu-id="66293-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66293-114">Application</span></span> | <span data-ttu-id="66293-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66293-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66293-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66293-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="66293-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66293-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="66293-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66293-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="66293-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="66293-119">Response</span></span>

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
