---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Criar uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 576c7b8c5f2f3e7b75e336cf898312a24e712903
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613149"
---
# <a name="create-a-new-list"></a><span data-ttu-id="5c0c3-102">Criar uma nova lista</span><span class="sxs-lookup"><span data-stu-id="5c0c3-102">Create a new list</span></span>

<span data-ttu-id="5c0c3-103">Criar uma nova [lista][] em um [site][].</span><span class="sxs-lookup"><span data-stu-id="5c0c3-103">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="5c0c3-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c0c3-104">Permissions</span></span>

<span data-ttu-id="5c0c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c0c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="5c0c3-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c0c3-107">Permission type</span></span>             | <span data-ttu-id="5c0c3-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c0c3-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5c0c3-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c0c3-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c0c3-110">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="5c0c3-110">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="5c0c3-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c0c3-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c0c3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c0c3-112">Not supported.</span></span>                              |
| <span data-ttu-id="5c0c3-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c0c3-113">Application</span></span>                            | <span data-ttu-id="5c0c3-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c0c3-114">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5c0c3-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c0c3-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="5c0c3-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c0c3-116">Request body</span></span>

<span data-ttu-id="5c0c3-117">No corpo da solicitação, forneça uma representação JSON do recurso [lista][] a criar.</span><span class="sxs-lookup"><span data-stu-id="5c0c3-117">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="5c0c3-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c0c3-118">Example</span></span>

<span data-ttu-id="5c0c3-119">Aqui está um exemplo de como criar uma nova lista genérica.</span><span class="sxs-lookup"><span data-stu-id="5c0c3-119">Here is an example of how to create a new generic list.</span></span>

<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "name": "Books",
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

<span data-ttu-id="5c0c3-120">**Observação:** Colunas personalizadas são opcionais.</span><span class="sxs-lookup"><span data-stu-id="5c0c3-120">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="5c0c3-121">Além de todas as colunas especificadas aqui, novas listas são criadas com colunas definidas no **modelo** referenciado.</span><span class="sxs-lookup"><span data-stu-id="5c0c3-121">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="5c0c3-122">Se a faceta **lista** ou **modelo** não for especificada, a lista considera como padrão o modelo `genericList`, que inclui uma coluna _Título_.</span><span class="sxs-lookup"><span data-stu-id="5c0c3-122">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="5c0c3-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c0c3-123">Response</span></span>

<span data-ttu-id="5c0c3-124">Se for bem-sucedido, esse método retornará uma [lista][] no corpo da resposta da lista criada.</span><span class="sxs-lookup"><span data-stu-id="5c0c3-124">If successful, this method returns a [list][] in the response body for the created list.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5c0c3-125">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5c0c3-125">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5c0c3-126">Basic</span><span class="sxs-lookup"><span data-stu-id="5c0c3-126">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c0c3-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c0c3-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-list-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="5c0c3-128">**Observação:** O objeto Response será truncado para mais clareza.</span><span class="sxs-lookup"><span data-stu-id="5c0c3-128">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="5c0c3-129">As propriedades padrão serão retornadas da chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c0c3-129">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create",
  "suppressions": [
    "Error: /api-reference/v1.0/api/list-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
