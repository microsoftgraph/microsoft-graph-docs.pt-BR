---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
ms.openlocfilehash: eaa97e169a8fcfdcb676679bb6dedd3a192925d8
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2017
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="24c29-102">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="24c29-102">Get an item in a list</span></span>

<span data-ttu-id="24c29-103">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="24c29-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="24c29-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24c29-106">Permissions</span></span>

<span data-ttu-id="24c29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="24c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24c29-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24c29-109">Permission type</span></span>      | <span data-ttu-id="24c29-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24c29-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24c29-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24c29-111">Delegated (work or school account)</span></span> | <span data-ttu-id="24c29-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24c29-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="24c29-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24c29-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24c29-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24c29-114">Not supported.</span></span>    |
|<span data-ttu-id="24c29-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24c29-115">Application</span></span> | <span data-ttu-id="24c29-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24c29-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24c29-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24c29-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="24c29-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24c29-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="24c29-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24c29-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="24c29-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="24c29-120">Response</span></span>

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
