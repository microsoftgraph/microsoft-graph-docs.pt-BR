---
title: Restaura uma versão anterior de um ListItem
description: Restaura uma versão anterior de um ListItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 58430c5bab6ef412f38da70b7f4bed9fe5c1dd36
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326638"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="3adc2-104">Restaura uma versão anterior de um ListItem</span><span class="sxs-lookup"><span data-stu-id="3adc2-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="3adc2-105">Restaura uma versão anterior de um ListItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="3adc2-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="3adc2-106">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.</span><span class="sxs-lookup"><span data-stu-id="3adc2-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="3adc2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3adc2-107">Permissions</span></span>

<span data-ttu-id="3adc2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3adc2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="3adc2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3adc2-110">Permission type</span></span>             |         <span data-ttu-id="3adc2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3adc2-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="3adc2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3adc2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3adc2-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="3adc2-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="3adc2-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3adc2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3adc2-115">n/d</span><span class="sxs-lookup"><span data-stu-id="3adc2-115">n/a</span></span>                                                          |
| <span data-ttu-id="3adc2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3adc2-116">Application</span></span>                            | <span data-ttu-id="3adc2-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="3adc2-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3adc2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3adc2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="3adc2-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3adc2-119">Request body</span></span>

<span data-ttu-id="3adc2-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3adc2-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="3adc2-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3adc2-121">Example</span></span>

<span data-ttu-id="3adc2-122">Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="3adc2-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3adc2-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="3adc2-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3adc2-124">C#</span><span class="sxs-lookup"><span data-stu-id="3adc2-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3adc2-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3adc2-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3adc2-126">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3adc2-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3adc2-127">Java</span><span class="sxs-lookup"><span data-stu-id="3adc2-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="3adc2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3adc2-128">Response</span></span>

<span data-ttu-id="3adc2-129">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3adc2-129">If successful, the API call returns a `204 No Content`.</span></span>

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
