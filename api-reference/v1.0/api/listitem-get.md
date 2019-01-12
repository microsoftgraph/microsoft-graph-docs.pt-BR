---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 1a1117717a0afc0d715da2297d69b0453ef2025e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950540"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="bc944-102">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="bc944-102">Get an item in a list</span></span>

<span data-ttu-id="bc944-103">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="bc944-103">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="bc944-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc944-106">Permissions</span></span>

<span data-ttu-id="bc944-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc944-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc944-109">Permission type</span></span>      | <span data-ttu-id="bc944-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc944-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc944-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc944-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc944-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc944-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc944-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc944-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc944-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc944-114">Not supported.</span></span>    |
|<span data-ttu-id="bc944-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc944-115">Application</span></span> | <span data-ttu-id="bc944-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc944-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc944-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc944-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="bc944-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc944-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bc944-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc944-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="bc944-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc944-120">Response</span></span>

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
