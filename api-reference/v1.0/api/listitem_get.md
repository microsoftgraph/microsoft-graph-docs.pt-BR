---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
ms.openlocfilehash: 29db5f5a3005aca0003489db4bdb13219e612a96
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="7cf93-102">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="7cf93-102">Represents an item or row in a list.</span></span>

<span data-ttu-id="7cf93-103">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="7cf93-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="7cf93-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7cf93-106">Permissions</span></span>

<span data-ttu-id="7cf93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7cf93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7cf93-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cf93-109">Permission type</span></span>      | <span data-ttu-id="7cf93-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cf93-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cf93-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cf93-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7cf93-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf93-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7cf93-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cf93-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cf93-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cf93-114">Not supported.</span></span>    |
|<span data-ttu-id="7cf93-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cf93-115">Application</span></span> | <span data-ttu-id="7cf93-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf93-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cf93-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cf93-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="7cf93-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cf93-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7cf93-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cf93-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="7cf93-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cf93-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
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
