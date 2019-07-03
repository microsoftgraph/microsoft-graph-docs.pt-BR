---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Criar uma nova entrada em uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8ccb8f1eaca5f32bd7b4820331a9aea5f6898e0d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449208"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="8f46c-102">Criar um novo item em uma lista</span><span class="sxs-lookup"><span data-stu-id="8f46c-102">Create a new item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f46c-103">Criar um novo [listItem][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="8f46c-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="8f46c-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f46c-104">Permissions</span></span>

<span data-ttu-id="8f46c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f46c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f46c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f46c-107">Permission type</span></span>      | <span data-ttu-id="8f46c-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f46c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f46c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f46c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8f46c-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f46c-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f46c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f46c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f46c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f46c-112">Not supported.</span></span>    |
|<span data-ttu-id="8f46c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f46c-113">Application</span></span> | <span data-ttu-id="8f46c-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f46c-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f46c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f46c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="8f46c-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f46c-116">Request body</span></span>

<span data-ttu-id="8f46c-117">No corpo da solicitação, forneça uma representação JSON do recurso [listItem][] a criar.</span><span class="sxs-lookup"><span data-stu-id="8f46c-117">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="8f46c-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f46c-118">Example</span></span>

<span data-ttu-id="8f46c-119">Aqui está um exemplo de como criar um novo item de lista genérica.</span><span class="sxs-lookup"><span data-stu-id="8f46c-119">Here is an example of how to create a new generic list item.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8f46c-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f46c-120">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f46c-121">C#</span><span class="sxs-lookup"><span data-stu-id="8f46c-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f46c-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f46c-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f46c-123">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8f46c-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="8f46c-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f46c-124">Response</span></span>

<span data-ttu-id="8f46c-125">Se for bem-sucedido, esse método retornará um [listItem][] no corpo da resposta da lista criada.</span><span class="sxs-lookup"><span data-stu-id="8f46c-125">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

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

<span data-ttu-id="8f46c-126">**Observação:** O objeto Response será truncado para mais clareza.</span><span class="sxs-lookup"><span data-stu-id="8f46c-126">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="8f46c-127">As propriedades padrão serão retornadas da chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f46c-127">Default properties will be returned from the actual call.</span></span>

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
