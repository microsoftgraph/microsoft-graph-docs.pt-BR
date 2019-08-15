---
author: JeremyKelley
description: Criar uma nova lista em um site.
ms.date: 09/11/2017
title: Criar uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: fc171e95d238f3e2ee6f413bd80a91e4b7f0b8dd
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415460"
---
# <a name="create-a-new-list"></a><span data-ttu-id="91313-103">Criar uma nova lista</span><span class="sxs-lookup"><span data-stu-id="91313-103">Create a new list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91313-104">Criar uma nova [lista][] em um [site][].</span><span class="sxs-lookup"><span data-stu-id="91313-104">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="91313-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="91313-105">Permissions</span></span>

<span data-ttu-id="91313-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="91313-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91313-108">Permission type</span></span>             | <span data-ttu-id="91313-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91313-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="91313-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91313-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="91313-111">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="91313-111">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="91313-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91313-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91313-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91313-113">Not supported.</span></span>                              |
| <span data-ttu-id="91313-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91313-114">Application</span></span>                            | <span data-ttu-id="91313-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91313-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="91313-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91313-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="91313-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91313-117">Request body</span></span>

<span data-ttu-id="91313-118">No corpo da solicitação, forneça uma representação JSON do recurso [lista][] a criar.</span><span class="sxs-lookup"><span data-stu-id="91313-118">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="91313-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91313-119">Example</span></span>

<span data-ttu-id="91313-120">Aqui está um exemplo de como criar uma nova lista genérica.</span><span class="sxs-lookup"><span data-stu-id="91313-120">Here is an example of how to create a new generic list.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="91313-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="91313-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "displayName": "Books",
  "columns": [
    {
      "name": "Author",
      "text": { }
    },
    {
      "name": "PageCount",
      "number": { }
    }
  ],
  "list": {
    "template": "genericList"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="91313-122">C#</span><span class="sxs-lookup"><span data-stu-id="91313-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91313-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91313-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="91313-124">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="91313-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="91313-125">**Observação:** Colunas personalizadas são opcionais.</span><span class="sxs-lookup"><span data-stu-id="91313-125">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="91313-126">Além de todas as colunas especificadas aqui, novas listas são criadas com colunas definidas no **modelo** referenciado.</span><span class="sxs-lookup"><span data-stu-id="91313-126">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="91313-127">Se a faceta **lista** ou **modelo** não for especificada, a lista considera como padrão o modelo `genericList`, que inclui uma coluna _Título_.</span><span class="sxs-lookup"><span data-stu-id="91313-127">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="91313-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="91313-128">Response</span></span>

<span data-ttu-id="91313-129">Se for bem-sucedido, esse método retornará uma [lista][] no corpo da resposta da lista criada.</span><span class="sxs-lookup"><span data-stu-id="91313-129">If successful, this method returns a [list][] in the response body for the created list.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.list", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "22e03ef3-6ef4-424d-a1d3-92a337807c30",
  "createdDateTime": "2017-04-30T01:21:00Z",
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

<span data-ttu-id="91313-130">**Observação:** O objeto Response será truncado para mais clareza.</span><span class="sxs-lookup"><span data-stu-id="91313-130">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="91313-131">As propriedades padrão serão retornadas da chamada real.</span><span class="sxs-lookup"><span data-stu-id="91313-131">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create",
  "suppressions": [
  ]
}
-->
