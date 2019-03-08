---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e9d747e5405a5aeaf97dfdf7e9a97f6236164a5a
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480639"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="3d511-102">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="3d511-102">Get an item in a list</span></span>

<span data-ttu-id="3d511-103">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="3d511-103">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="3d511-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d511-106">Permissions</span></span>

<span data-ttu-id="3d511-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d511-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d511-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d511-109">Permission type</span></span>      | <span data-ttu-id="3d511-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d511-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d511-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d511-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3d511-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d511-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d511-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d511-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d511-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d511-114">Not supported.</span></span>    |
|<span data-ttu-id="3d511-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d511-115">Application</span></span> | <span data-ttu-id="3d511-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d511-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d511-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d511-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="3d511-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d511-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3d511-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d511-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="3d511-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d511-120">Response</span></span>

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
