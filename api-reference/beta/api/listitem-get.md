---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1f50d31dd58bb0839113a1954fb16f0d824da5f9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333467"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="f110f-102">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="f110f-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f110f-103">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="f110f-103">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="f110f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f110f-106">Permissions</span></span>

<span data-ttu-id="f110f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f110f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f110f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f110f-109">Permission type</span></span>      | <span data-ttu-id="f110f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f110f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f110f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f110f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f110f-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f110f-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f110f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f110f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f110f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f110f-114">Not supported.</span></span>    |
|<span data-ttu-id="f110f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f110f-115">Application</span></span> | <span data-ttu-id="f110f-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f110f-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f110f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f110f-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="f110f-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f110f-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f110f-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f110f-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="f110f-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="f110f-120">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": []
}
-->
