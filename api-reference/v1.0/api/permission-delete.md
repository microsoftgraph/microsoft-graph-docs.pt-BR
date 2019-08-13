---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Remover o acesso a um item
localization_priority: Normal
description: Remova o acesso a um DriveItem.
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 84fa03016948b5ac5462e541c98ad12e5705857b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374047"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="3374e-103">Excluir uma permissão de compartilhamento de um arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="3374e-103">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="3374e-104">Remova o acesso a um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3374e-104">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="3374e-105">Somente as permissões de compartilhamento **não** herdadas podem ser excluídas.</span><span class="sxs-lookup"><span data-stu-id="3374e-105">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="3374e-106">A propriedade **inheritedFrom** deve ser `null`.</span><span class="sxs-lookup"><span data-stu-id="3374e-106">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="3374e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3374e-107">Permissions</span></span>

<span data-ttu-id="3374e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3374e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3374e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3374e-110">Permission type</span></span>      | <span data-ttu-id="3374e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3374e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3374e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3374e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3374e-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3374e-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3374e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3374e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3374e-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3374e-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3374e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3374e-116">Application</span></span> | <span data-ttu-id="3374e-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3374e-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3374e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3374e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="3374e-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="3374e-119">Optional request headers</span></span>

| <span data-ttu-id="3374e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3374e-120">Name</span></span>          | <span data-ttu-id="3374e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3374e-121">Type</span></span>   | <span data-ttu-id="3374e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3374e-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3374e-123">if-match</span><span class="sxs-lookup"><span data-stu-id="3374e-123">if-match</span></span>      | <span data-ttu-id="3374e-124">string</span><span class="sxs-lookup"><span data-stu-id="3374e-124">string</span></span> | <span data-ttu-id="3374e-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="3374e-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="3374e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3374e-126">Response</span></span>

<span data-ttu-id="3374e-127">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3374e-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3374e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3374e-128">Example</span></span>

<span data-ttu-id="3374e-129">Este exemplo remove a permissão identificada como {perm-id} de {item-id} do item no OneDrive do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="3374e-129">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3374e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="3374e-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite", "tags": "service.graph" }-->

```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3374e-131">C#</span><span class="sxs-lookup"><span data-stu-id="3374e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3374e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3374e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3374e-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3374e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3374e-134">Java</span><span class="sxs-lookup"><span data-stu-id="3374e-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3374e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3374e-135">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="3374e-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="3374e-136">Remarks</span></span>

* <span data-ttu-id="3374e-137">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="3374e-137">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

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
