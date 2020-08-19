---
title: Restaura uma versão anterior de um ListItem
description: Restaura uma versão anterior de um ListItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: f8f7aa23a1db378dea805ed5250c0d27e3d0c554
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812699"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="7d888-104">Restaura uma versão anterior de um ListItem</span><span class="sxs-lookup"><span data-stu-id="7d888-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="7d888-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d888-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d888-106">Restaura uma versão anterior de um ListItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="7d888-106">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="7d888-107">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.</span><span class="sxs-lookup"><span data-stu-id="7d888-107">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d888-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d888-108">Permissions</span></span>

<span data-ttu-id="7d888-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d888-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="7d888-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d888-111">Permission type</span></span>             |         <span data-ttu-id="7d888-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d888-112">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="7d888-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d888-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d888-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7d888-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="7d888-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d888-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d888-116">n/d</span><span class="sxs-lookup"><span data-stu-id="7d888-116">n/a</span></span>                                                          |
| <span data-ttu-id="7d888-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d888-117">Application</span></span>                            | <span data-ttu-id="7d888-118">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7d888-118">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d888-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d888-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="7d888-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d888-120">Request body</span></span>

<span data-ttu-id="7d888-121">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d888-121">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="7d888-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d888-122">Example</span></span>

<span data-ttu-id="7d888-123">Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="7d888-123">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="7d888-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d888-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="c"></a>[<span data-ttu-id="7d888-125">C#</span><span class="sxs-lookup"><span data-stu-id="7d888-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d888-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d888-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d888-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d888-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d888-128">Java</span><span class="sxs-lookup"><span data-stu-id="7d888-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="7d888-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d888-129">Response</span></span>

<span data-ttu-id="7d888-130">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7d888-130">If successful, the API call returns a `204 No Content`.</span></span>

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
