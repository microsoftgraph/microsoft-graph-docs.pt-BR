---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Recuperar itens de uma lista do SharePoint
ms.openlocfilehash: 3c6a8259f17091612cf10e1501a24d9eb60e28d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034413"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="88dd8-102">Enumerar itens em uma lista</span><span class="sxs-lookup"><span data-stu-id="88dd8-102">Enumerate items in a list</span></span>

> <span data-ttu-id="88dd8-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="88dd8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88dd8-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="88dd8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88dd8-105">Obter a coleção de [itens][item] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="88dd8-105">Get the collection of [items][item] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="88dd8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="88dd8-107">Permissions</span></span>

<span data-ttu-id="88dd8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88dd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88dd8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88dd8-110">Permission type</span></span>      | <span data-ttu-id="88dd8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88dd8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88dd8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88dd8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="88dd8-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88dd8-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="88dd8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88dd8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88dd8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88dd8-115">Not supported.</span></span>    |
|<span data-ttu-id="88dd8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88dd8-116">Application</span></span> | <span data-ttu-id="88dd8-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88dd8-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88dd8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88dd8-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="88dd8-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88dd8-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="88dd8-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88dd8-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="88dd8-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="88dd8-121">Response</span></span>

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
