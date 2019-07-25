---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Excluir um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9bb6661ff7a43fbf29c80a77e5b909322bfbf569
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881735"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="a88ae-102">Excluir um DriveItem</span><span class="sxs-lookup"><span data-stu-id="a88ae-102">Delete a DriveItem</span></span>

<span data-ttu-id="a88ae-p101">Excluir um [DriveItem](../resources/driveitem.md) usando sua ID ou seu caminho. Observe que a exclusão de itens usando esse método moverá os itens para a Lixeira, ao invés de excluir permanentemente o item.</span><span class="sxs-lookup"><span data-stu-id="a88ae-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="a88ae-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a88ae-105">Permissions</span></span>

<span data-ttu-id="a88ae-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a88ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a88ae-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a88ae-108">Permission type</span></span>      | <span data-ttu-id="a88ae-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a88ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a88ae-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a88ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a88ae-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a88ae-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a88ae-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a88ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a88ae-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a88ae-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a88ae-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a88ae-114">Application</span></span> | <span data-ttu-id="a88ae-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a88ae-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a88ae-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a88ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="a88ae-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="a88ae-117">Optional request headers</span></span>

| <span data-ttu-id="a88ae-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a88ae-118">Name</span></span>          | <span data-ttu-id="a88ae-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a88ae-119">Type</span></span>   | <span data-ttu-id="a88ae-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a88ae-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a88ae-121">if-match</span><span class="sxs-lookup"><span data-stu-id="a88ae-121">if-match</span></span>      | <span data-ttu-id="a88ae-122">String</span><span class="sxs-lookup"><span data-stu-id="a88ae-122">String</span></span> | <span data-ttu-id="a88ae-123">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="a88ae-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="a88ae-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a88ae-124">Example</span></span>

<span data-ttu-id="a88ae-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a88ae-125">Here is an example of how to call this API.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a88ae-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="a88ae-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-drive-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
DELETE /me/drive/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a88ae-127">C#</span><span class="sxs-lookup"><span data-stu-id="a88ae-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-drive-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a88ae-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="a88ae-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-drive-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a88ae-129">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a88ae-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-drive-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a88ae-130">Java</span><span class="sxs-lookup"><span data-stu-id="a88ae-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-drive-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="a88ae-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a88ae-131">Response</span></span>

<span data-ttu-id="a88ae-132">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="a88ae-132">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="a88ae-133">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="a88ae-133">Error responses</span></span>

<span data-ttu-id="a88ae-134">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="a88ae-134">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete",
  "suppressions": [
  ]
} -->
