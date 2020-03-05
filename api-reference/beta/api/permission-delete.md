---
author: JeremyKelley
description: Remova o acesso a um DriveItem.
ms.date: 09/10/2017
title: Remover o acesso a um item
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: a7990bf666dd18bfc0e04d5874fe176ed48e909b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455971"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="b7b44-103">Excluir uma permissão de compartilhamento de um arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="b7b44-103">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="b7b44-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b7b44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7b44-105">Remova o acesso a um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b7b44-105">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="b7b44-106">Somente as permissões de compartilhamento **não** herdadas podem ser excluídas.</span><span class="sxs-lookup"><span data-stu-id="b7b44-106">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="b7b44-107">A propriedade **inheritedFrom** deve ser `null`.</span><span class="sxs-lookup"><span data-stu-id="b7b44-107">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7b44-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b7b44-108">Permissions</span></span>
<span data-ttu-id="b7b44-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7b44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7b44-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7b44-111">Permission type</span></span>      | <span data-ttu-id="b7b44-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7b44-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7b44-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7b44-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b7b44-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b44-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7b44-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7b44-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7b44-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b44-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7b44-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7b44-117">Application</span></span> | <span data-ttu-id="b7b44-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b44-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7b44-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7b44-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="b7b44-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b7b44-120">Optional request headers</span></span>

| <span data-ttu-id="b7b44-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b7b44-121">Name</span></span>          | <span data-ttu-id="b7b44-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7b44-122">Type</span></span>   | <span data-ttu-id="b7b44-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7b44-123">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b7b44-124">if-match</span><span class="sxs-lookup"><span data-stu-id="b7b44-124">if-match</span></span>      | <span data-ttu-id="b7b44-125">string</span><span class="sxs-lookup"><span data-stu-id="b7b44-125">string</span></span> | <span data-ttu-id="b7b44-126">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="b7b44-126">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="response"></a><span data-ttu-id="b7b44-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7b44-127">Response</span></span>

<span data-ttu-id="b7b44-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b7b44-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b7b44-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7b44-129">Example</span></span>

<span data-ttu-id="b7b44-130">Este exemplo remove a permissão identificada como {perm-id} de {item-id} do item no OneDrive do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="b7b44-130">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>


# <a name="http"></a>[<span data-ttu-id="b7b44-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7b44-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->

```http
DELETE https://graph.microsoft.com/beta/me/drive/root/items/{item-id}/permissions/{perm-id}
```
# <a name="c"></a>[<span data-ttu-id="b7b44-132">C#</span><span class="sxs-lookup"><span data-stu-id="b7b44-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7b44-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7b44-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7b44-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7b44-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b7b44-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7b44-135">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="b7b44-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="b7b44-136">Remarks</span></span>

* <span data-ttu-id="b7b44-137">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="b7b44-137">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission",
  "suppressions": [
  ]
}
-->
