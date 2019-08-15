---
author: JeremyKelley
description: Excluir um DriveItem usando sua ID ou seu caminho.
ms.date: 09/10/2017
title: Excluir um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5ff1e8ed83026d5b91738cff8204271bc8739068
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416840"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="c37ea-103">Excluir um DriveItem</span><span class="sxs-lookup"><span data-stu-id="c37ea-103">Delete a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c37ea-p101">Excluir um [DriveItem](../resources/driveitem.md) usando sua ID ou seu caminho. Observe que a exclusão de itens usando esse método moverá os itens para a Lixeira, ao invés de excluir permanentemente o item.</span><span class="sxs-lookup"><span data-stu-id="c37ea-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="c37ea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c37ea-106">Permissions</span></span>

<span data-ttu-id="c37ea-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c37ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c37ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c37ea-109">Permission type</span></span>      | <span data-ttu-id="c37ea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c37ea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c37ea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c37ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c37ea-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c37ea-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c37ea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c37ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c37ea-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c37ea-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c37ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c37ea-115">Application</span></span> | <span data-ttu-id="c37ea-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c37ea-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c37ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c37ea-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="c37ea-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="c37ea-118">Optional request headers</span></span>

| <span data-ttu-id="c37ea-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c37ea-119">Name</span></span>          | <span data-ttu-id="c37ea-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c37ea-120">Type</span></span>   | <span data-ttu-id="c37ea-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c37ea-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c37ea-122">if-match</span><span class="sxs-lookup"><span data-stu-id="c37ea-122">if-match</span></span>      | <span data-ttu-id="c37ea-123">String</span><span class="sxs-lookup"><span data-stu-id="c37ea-123">String</span></span> | <span data-ttu-id="c37ea-124">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="c37ea-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="c37ea-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c37ea-125">Example</span></span>

<span data-ttu-id="c37ea-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c37ea-126">Here is an example of how to call this API.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c37ea-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="c37ea-127">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-drive-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c37ea-128">C#</span><span class="sxs-lookup"><span data-stu-id="c37ea-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-drive-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c37ea-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c37ea-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-drive-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c37ea-130">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c37ea-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-drive-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="c37ea-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c37ea-131">Response</span></span>

<span data-ttu-id="c37ea-132">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="c37ea-132">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="c37ea-133">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="c37ea-133">Error responses</span></span>

<span data-ttu-id="c37ea-134">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="c37ea-134">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete",
  "suppressions": [
  ]
}
-->
