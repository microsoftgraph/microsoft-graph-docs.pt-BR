---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Remover o acesso a um item
localization_priority: Normal
ms.openlocfilehash: c93e37010e551cd36e17c2d5b25cf00e84949078
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35454311"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="5027c-102">Excluir uma permissão de compartilhamento de um arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="5027c-102">Delete a sharing permission from a file or folder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5027c-103">Remova o acesso a um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="5027c-103">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="5027c-104">Somente as permissões de compartilhamento **não** herdadas podem ser excluídas.</span><span class="sxs-lookup"><span data-stu-id="5027c-104">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="5027c-105">A propriedade **inheritedFrom** deve ser `null`.</span><span class="sxs-lookup"><span data-stu-id="5027c-105">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="5027c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5027c-106">Permissions</span></span>
<span data-ttu-id="5027c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5027c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5027c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5027c-109">Permission type</span></span>      | <span data-ttu-id="5027c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5027c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5027c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5027c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5027c-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5027c-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5027c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5027c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5027c-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5027c-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5027c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5027c-115">Application</span></span> | <span data-ttu-id="5027c-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5027c-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5027c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5027c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="5027c-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="5027c-118">Optional request headers</span></span>

| <span data-ttu-id="5027c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5027c-119">Name</span></span>          | <span data-ttu-id="5027c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5027c-120">Type</span></span>   | <span data-ttu-id="5027c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5027c-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5027c-122">if-match</span><span class="sxs-lookup"><span data-stu-id="5027c-122">if-match</span></span>      | <span data-ttu-id="5027c-123">string</span><span class="sxs-lookup"><span data-stu-id="5027c-123">string</span></span> | <span data-ttu-id="5027c-124">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="5027c-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="response"></a><span data-ttu-id="5027c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="5027c-125">Response</span></span>

<span data-ttu-id="5027c-126">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5027c-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5027c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5027c-127">Example</span></span>

<span data-ttu-id="5027c-128">Este exemplo remove a permissão identificada como {perm-id} de {item-id} do item no OneDrive do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="5027c-128">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5027c-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="5027c-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->

```http
DELETE https://graph.microsoft.com/beta/me/drive/root/items/{item-id}/permissions/{perm-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5027c-130">C#</span><span class="sxs-lookup"><span data-stu-id="5027c-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5027c-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="5027c-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5027c-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5027c-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5027c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5027c-133">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="5027c-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="5027c-134">Remarks</span></span>

* <span data-ttu-id="5027c-135">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="5027c-135">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

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
