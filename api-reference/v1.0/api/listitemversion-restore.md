---
title: Restaura uma versão anterior de um ListItem
description: Restaura uma versão anterior de um ListItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0720b39a6fe91cee7fa6a3e66bb1b3e26891b00e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460704"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="54d3e-104">Restaura uma versão anterior de um ListItem</span><span class="sxs-lookup"><span data-stu-id="54d3e-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="54d3e-105">Restaura uma versão anterior de um ListItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="54d3e-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="54d3e-106">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.</span><span class="sxs-lookup"><span data-stu-id="54d3e-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="54d3e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="54d3e-107">Permissions</span></span>

<span data-ttu-id="54d3e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54d3e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="54d3e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54d3e-110">Permission type</span></span>             |         <span data-ttu-id="54d3e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54d3e-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="54d3e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54d3e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="54d3e-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="54d3e-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="54d3e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54d3e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54d3e-115">n/d</span><span class="sxs-lookup"><span data-stu-id="54d3e-115">n/a</span></span>                                                          |
| <span data-ttu-id="54d3e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54d3e-116">Application</span></span>                            | <span data-ttu-id="54d3e-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="54d3e-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54d3e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54d3e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="54d3e-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54d3e-119">Request body</span></span>

<span data-ttu-id="54d3e-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54d3e-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="54d3e-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54d3e-121">Example</span></span>

<span data-ttu-id="54d3e-122">Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="54d3e-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="54d3e-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="54d3e-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="54d3e-124">C#</span><span class="sxs-lookup"><span data-stu-id="54d3e-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54d3e-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="54d3e-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="54d3e-126">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="54d3e-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="54d3e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="54d3e-127">Response</span></span>

<span data-ttu-id="54d3e-128">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="54d3e-128">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->
