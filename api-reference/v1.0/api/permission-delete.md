---
author: JeremyKelley
ms.date: 09/10/2017
title: Remover o acesso a um item
localization_priority: Normal
description: Remova o acesso a um DriveItem.
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c21c3685aa2471026e5d7ff9e10e6f84370c4673
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945094"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="db48b-103">Excluir uma permissão de compartilhamento de um arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="db48b-103">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="db48b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db48b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db48b-105">Remova o acesso a um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="db48b-105">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="db48b-106">Somente as permissões de compartilhamento **não** herdadas podem ser excluídas.</span><span class="sxs-lookup"><span data-stu-id="db48b-106">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="db48b-107">A propriedade **inheritedFrom** deve ser `null`.</span><span class="sxs-lookup"><span data-stu-id="db48b-107">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="db48b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="db48b-108">Permissions</span></span>

<span data-ttu-id="db48b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db48b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db48b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db48b-111">Permission type</span></span>      | <span data-ttu-id="db48b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db48b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db48b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db48b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="db48b-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db48b-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="db48b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db48b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db48b-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db48b-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="db48b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db48b-117">Application</span></span> | <span data-ttu-id="db48b-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db48b-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db48b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db48b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="db48b-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="db48b-120">Optional request headers</span></span>

| <span data-ttu-id="db48b-121">Name</span><span class="sxs-lookup"><span data-stu-id="db48b-121">Name</span></span>          | <span data-ttu-id="db48b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="db48b-122">Type</span></span>   | <span data-ttu-id="db48b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="db48b-123">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="db48b-124">if-match</span><span class="sxs-lookup"><span data-stu-id="db48b-124">if-match</span></span>      | <span data-ttu-id="db48b-125">string</span><span class="sxs-lookup"><span data-stu-id="db48b-125">string</span></span> | <span data-ttu-id="db48b-126">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="db48b-126">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="db48b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="db48b-127">Response</span></span>

<span data-ttu-id="db48b-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="db48b-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="db48b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db48b-129">Example</span></span>

<span data-ttu-id="db48b-130">Este exemplo remove a permissão identificada como {perm-id} de {item-id} do item no OneDrive do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="db48b-130">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="db48b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="db48b-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-permission-1", "scopes": "files.readwrite", "tags": "service.graph" }-->

```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
```
# <a name="c"></a>[<span data-ttu-id="db48b-132">C#</span><span class="sxs-lookup"><span data-stu-id="db48b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db48b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db48b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db48b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db48b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db48b-135">Java</span><span class="sxs-lookup"><span data-stu-id="db48b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permission-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db48b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="db48b-136">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="db48b-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="db48b-137">Remarks</span></span>

* <span data-ttu-id="db48b-138">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="db48b-138">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "Sharing/Remove permissions",
  "suppressions": [
  ]
} -->

