---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Priority
ms.openlocfilehash: ab263c074497d43bb03ea7c69748bb1c64fd9425
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881127"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="c1f87-102">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="c1f87-102">Get an item in a list</span></span>

<span data-ttu-id="c1f87-103">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="c1f87-103">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="c1f87-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1f87-106">Permissions</span></span>

<span data-ttu-id="c1f87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1f87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1f87-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1f87-109">Permission type</span></span>      | <span data-ttu-id="c1f87-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1f87-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1f87-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1f87-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c1f87-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1f87-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1f87-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1f87-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1f87-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1f87-114">Not supported.</span></span>    |
|<span data-ttu-id="c1f87-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1f87-115">Application</span></span> | <span data-ttu-id="c1f87-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1f87-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1f87-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1f87-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="c1f87-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1f87-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c1f87-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1f87-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="c1f87-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1f87-120">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata"
} -->
