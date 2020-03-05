---
author: JeremyKelley
description: Criar um novo listItem em uma lista.
ms.date: 09/11/2017
title: Criar uma nova entrada em uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 19a415a7e8c24a84202c55fa562646621c22bb6b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457141"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="a1f58-103">Criar um novo item em uma lista</span><span class="sxs-lookup"><span data-stu-id="a1f58-103">Create a new item in a list</span></span>

<span data-ttu-id="a1f58-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a1f58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1f58-105">Criar um novo [listItem][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="a1f58-105">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="a1f58-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1f58-106">Permissions</span></span>

<span data-ttu-id="a1f58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1f58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1f58-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1f58-109">Permission type</span></span>      | <span data-ttu-id="a1f58-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1f58-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1f58-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1f58-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a1f58-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1f58-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a1f58-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1f58-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1f58-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1f58-114">Not supported.</span></span>    |
|<span data-ttu-id="a1f58-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1f58-115">Application</span></span> | <span data-ttu-id="a1f58-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1f58-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1f58-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1f58-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="a1f58-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1f58-118">Request body</span></span>

<span data-ttu-id="a1f58-119">No corpo da solicitação, forneça uma representação JSON do recurso [listItem][] a criar.</span><span class="sxs-lookup"><span data-stu-id="a1f58-119">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="a1f58-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1f58-120">Example</span></span>

<span data-ttu-id="a1f58-121">Aqui está um exemplo de como criar um novo item de lista genérica.</span><span class="sxs-lookup"><span data-stu-id="a1f58-121">Here is an example of how to create a new generic list item.</span></span>


# <a name="http"></a>[<span data-ttu-id="a1f58-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1f58-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```
# <a name="c"></a>[<span data-ttu-id="a1f58-123">C#</span><span class="sxs-lookup"><span data-stu-id="a1f58-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1f58-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1f58-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1f58-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1f58-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="a1f58-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1f58-126">Response</span></span>

<span data-ttu-id="a1f58-127">Se for bem-sucedido, esse método retornará um [listItem][] no corpo da resposta da lista criada.</span><span class="sxs-lookup"><span data-stu-id="a1f58-127">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

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

<span data-ttu-id="a1f58-128">**Observação:** O objeto Response será truncado para mais clareza.</span><span class="sxs-lookup"><span data-stu-id="a1f58-128">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="a1f58-129">As propriedades padrão serão retornadas da chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1f58-129">Default properties will be returned from the actual call.</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create",
  "suppressions": [
  ]
}
-->
