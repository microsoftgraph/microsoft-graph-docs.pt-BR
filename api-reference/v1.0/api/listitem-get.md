---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e9d747e5405a5aeaf97dfdf7e9a97f6236164a5a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563571"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="57a15-102">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="57a15-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57a15-103">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="57a15-103">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="57a15-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="57a15-106">Permissions</span></span>

<span data-ttu-id="57a15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57a15-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57a15-109">Permission type</span></span>      | <span data-ttu-id="57a15-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57a15-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57a15-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57a15-111">Delegated (work or school account)</span></span> | <span data-ttu-id="57a15-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57a15-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="57a15-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57a15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57a15-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57a15-114">Not supported.</span></span>    |
|<span data-ttu-id="57a15-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57a15-115">Application</span></span> | <span data-ttu-id="57a15-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57a15-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57a15-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57a15-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="57a15-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57a15-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="57a15-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57a15-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="57a15-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="57a15-120">Response</span></span>

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
