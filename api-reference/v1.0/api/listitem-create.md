---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Criar uma nova entrada em uma lista do SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e2183eff38bdf4237ab4464cfb6bd55e1f88fa16
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272027"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="3f85f-102">Criar um novo item em uma lista</span><span class="sxs-lookup"><span data-stu-id="3f85f-102">Create a new item in a list</span></span>

<span data-ttu-id="3f85f-103">Criar um novo [listItem][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="3f85f-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="3f85f-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f85f-104">Permissions</span></span>

<span data-ttu-id="3f85f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f85f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f85f-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f85f-107">Permission type</span></span>      | <span data-ttu-id="3f85f-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f85f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f85f-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f85f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3f85f-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f85f-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3f85f-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f85f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f85f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f85f-112">Not supported.</span></span>    |
|<span data-ttu-id="3f85f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f85f-113">Application</span></span> | <span data-ttu-id="3f85f-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f85f-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f85f-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f85f-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="3f85f-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f85f-116">Request body</span></span>

<span data-ttu-id="3f85f-117">No corpo da solicitação, forneça uma representação JSON do recurso [listItem][] a criar.</span><span class="sxs-lookup"><span data-stu-id="3f85f-117">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="3f85f-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f85f-118">Example</span></span>

<span data-ttu-id="3f85f-119">Aqui está um exemplo de como criar um novo item de lista genérica.</span><span class="sxs-lookup"><span data-stu-id="3f85f-119">Here is an example of how to create a new generic list item.</span></span>

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a><span data-ttu-id="3f85f-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f85f-120">Response</span></span>

<span data-ttu-id="3f85f-121">Se for bem-sucedido, esse método retornará um [listItem][] no corpo da resposta da lista criada.</span><span class="sxs-lookup"><span data-stu-id="3f85f-121">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3f85f-122">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3f85f-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3f85f-123">C#</span><span class="sxs-lookup"><span data-stu-id="3f85f-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-listitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f85f-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="3f85f-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-listitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3f85f-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f85f-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-listitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="3f85f-126">**Observação:** O objeto Response será truncado para mais clareza.</span><span class="sxs-lookup"><span data-stu-id="3f85f-126">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="3f85f-127">As propriedades padrão serão retornadas da chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f85f-127">Default properties will be returned from the actual call.</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-create.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitem-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
