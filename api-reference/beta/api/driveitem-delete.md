---
author: JeremyKelley
description: Excluir um DriveItem usando sua ID ou seu caminho.
ms.date: 09/10/2017
title: Excluir um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1e1c36b6ebd77cb95b1d0ad360f88e5dcf850bd1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432772"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="a91e8-103">Excluir um DriveItem</span><span class="sxs-lookup"><span data-stu-id="a91e8-103">Delete a DriveItem</span></span>

<span data-ttu-id="a91e8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a91e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a91e8-p101">Excluir um [DriveItem](../resources/driveitem.md) usando sua ID ou seu caminho. Observe que a exclusão de itens usando esse método moverá os itens para a Lixeira, ao invés de excluir permanentemente o item.</span><span class="sxs-lookup"><span data-stu-id="a91e8-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="a91e8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a91e8-107">Permissions</span></span>

<span data-ttu-id="a91e8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a91e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a91e8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a91e8-110">Permission type</span></span>      | <span data-ttu-id="a91e8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a91e8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a91e8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a91e8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a91e8-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a91e8-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a91e8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a91e8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a91e8-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a91e8-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a91e8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a91e8-116">Application</span></span> | <span data-ttu-id="a91e8-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a91e8-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a91e8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a91e8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="a91e8-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="a91e8-119">Optional request headers</span></span>

| <span data-ttu-id="a91e8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a91e8-120">Name</span></span>          | <span data-ttu-id="a91e8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a91e8-121">Type</span></span>   | <span data-ttu-id="a91e8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a91e8-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a91e8-123">if-match</span><span class="sxs-lookup"><span data-stu-id="a91e8-123">if-match</span></span>      | <span data-ttu-id="a91e8-124">String</span><span class="sxs-lookup"><span data-stu-id="a91e8-124">String</span></span> | <span data-ttu-id="a91e8-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="a91e8-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="a91e8-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a91e8-126">Example</span></span>

<span data-ttu-id="a91e8-127">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a91e8-127">Here is an example of how to call this API.</span></span>


# <a name="http"></a>[<span data-ttu-id="a91e8-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="a91e8-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-drive-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="a91e8-129">C#</span><span class="sxs-lookup"><span data-stu-id="a91e8-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-drive-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a91e8-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a91e8-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-drive-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a91e8-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a91e8-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-drive-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="a91e8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a91e8-132">Response</span></span>

<span data-ttu-id="a91e8-133">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="a91e8-133">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="a91e8-134">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="a91e8-134">Error responses</span></span>

<span data-ttu-id="a91e8-135">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="a91e8-135">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
