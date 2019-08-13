---
title: Restaurar uma versão anterior de um DriveItem
description: Restaura uma versão anterior de um DriveItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 0a528e3484e0cf6cd7c8a4ad8f1c85287f063106
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370505"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="04ec7-104">Restaurar uma versão anterior de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="04ec7-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="04ec7-105">Restaura uma versão anterior de um DriveItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="04ec7-105">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="04ec7-106">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="04ec7-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="04ec7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="04ec7-107">Permissions</span></span>

<span data-ttu-id="04ec7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04ec7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04ec7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04ec7-110">Permission type</span></span>      | <span data-ttu-id="04ec7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04ec7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04ec7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04ec7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04ec7-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ec7-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="04ec7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04ec7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04ec7-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ec7-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="04ec7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04ec7-116">Application</span></span> | <span data-ttu-id="04ec7-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ec7-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04ec7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04ec7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="04ec7-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04ec7-119">Request body</span></span>

<span data-ttu-id="04ec7-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04ec7-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="04ec7-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04ec7-121">Example</span></span>

<span data-ttu-id="04ec7-122">Este exemplo restaura uma versão de um arquivo identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="04ec7-122">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="04ec7-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="04ec7-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="04ec7-124">C#</span><span class="sxs-lookup"><span data-stu-id="04ec7-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04ec7-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04ec7-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="04ec7-126">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="04ec7-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="04ec7-127">Java</span><span class="sxs-lookup"><span data-stu-id="04ec7-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="04ec7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="04ec7-128">Response</span></span>

<span data-ttu-id="04ec7-129">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04ec7-129">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->
