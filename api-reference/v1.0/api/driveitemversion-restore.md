---
title: Restaurar uma versão anterior de um DriveItem
description: Restaura uma versão anterior de um DriveItem para ser a versão atual. Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 37f4928e6e3550cb7e022ed4b0ea1ab969a43ec3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517633"
---
# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="d0da6-104">Restaurar uma versão anterior de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="d0da6-104">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="d0da6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0da6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0da6-106">Restaura uma versão anterior de um DriveItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="d0da6-106">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="d0da6-107">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="d0da6-107">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0da6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0da6-108">Permissions</span></span>

<span data-ttu-id="d0da6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0da6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0da6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0da6-111">Permission type</span></span>      | <span data-ttu-id="d0da6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0da6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0da6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0da6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d0da6-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0da6-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0da6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0da6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0da6-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0da6-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0da6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0da6-117">Application</span></span> | <span data-ttu-id="d0da6-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0da6-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0da6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0da6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="d0da6-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0da6-120">Request body</span></span>

<span data-ttu-id="d0da6-121">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0da6-121">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="d0da6-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0da6-122">Example</span></span>

<span data-ttu-id="d0da6-123">Este exemplo restaura uma versão de um arquivo identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="d0da6-123">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="d0da6-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0da6-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="c"></a>[<span data-ttu-id="d0da6-125">C#</span><span class="sxs-lookup"><span data-stu-id="d0da6-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0da6-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0da6-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0da6-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0da6-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0da6-128">Java</span><span class="sxs-lookup"><span data-stu-id="d0da6-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="d0da6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0da6-129">Response</span></span>

<span data-ttu-id="d0da6-130">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d0da6-130">If successful, the API call returns a `204 No Content`.</span></span>

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
