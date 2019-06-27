---
title: Restaura uma versão anterior de um ListItem
description: Restaura uma versão anterior de um ListItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ff3a9149113ee03aade7c7e2ea943a2bd6446a9a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271978"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="6f69e-104">Restaura uma versão anterior de um ListItem</span><span class="sxs-lookup"><span data-stu-id="6f69e-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="6f69e-105">Restaura uma versão anterior de um ListItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="6f69e-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="6f69e-106">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.</span><span class="sxs-lookup"><span data-stu-id="6f69e-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f69e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f69e-107">Permissions</span></span>

<span data-ttu-id="6f69e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f69e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="6f69e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f69e-110">Permission type</span></span>             |         <span data-ttu-id="6f69e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f69e-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="6f69e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f69e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f69e-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6f69e-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="6f69e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f69e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f69e-115">n/d</span><span class="sxs-lookup"><span data-stu-id="6f69e-115">n/a</span></span>                                                          |
| <span data-ttu-id="6f69e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f69e-116">Application</span></span>                            | <span data-ttu-id="6f69e-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6f69e-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f69e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f69e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="6f69e-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f69e-119">Request body</span></span>

<span data-ttu-id="6f69e-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f69e-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="6f69e-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f69e-121">Example</span></span>

<span data-ttu-id="6f69e-122">Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="6f69e-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="6f69e-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f69e-123">Response</span></span>

<span data-ttu-id="6f69e-124">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6f69e-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6f69e-125">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6f69e-125">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6f69e-126">C#</span><span class="sxs-lookup"><span data-stu-id="6f69e-126">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/restore-item-version-listItem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f69e-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="6f69e-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/restore-item-version-listItem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6f69e-128">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6f69e-128">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/restore-item-version-listItem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/listitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitemversion-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
