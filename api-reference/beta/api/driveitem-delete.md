---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Excluir um arquivo ou pasta
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5b9b48cc5fd0ad3c35a8052571096c24699fdff7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589549"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="76e08-102">Excluir um DriveItem</span><span class="sxs-lookup"><span data-stu-id="76e08-102">Delete a DriveItem</span></span>

<span data-ttu-id="76e08-p101">Excluir um [DriveItem](../resources/driveitem.md) usando sua ID ou seu caminho. Observe que a exclusão de itens usando esse método moverá os itens para a Lixeira, ao invés de excluir permanentemente o item.</span><span class="sxs-lookup"><span data-stu-id="76e08-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="76e08-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="76e08-105">Permissions</span></span>

<span data-ttu-id="76e08-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76e08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76e08-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76e08-108">Permission type</span></span>      | <span data-ttu-id="76e08-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76e08-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76e08-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76e08-110">Delegated (work or school account)</span></span> | <span data-ttu-id="76e08-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e08-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="76e08-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76e08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76e08-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e08-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="76e08-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76e08-114">Application</span></span> | <span data-ttu-id="76e08-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e08-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76e08-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76e08-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="76e08-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="76e08-117">Optional request headers</span></span>

| <span data-ttu-id="76e08-118">Nome</span><span class="sxs-lookup"><span data-stu-id="76e08-118">Name</span></span>          | <span data-ttu-id="76e08-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="76e08-119">Type</span></span>   | <span data-ttu-id="76e08-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="76e08-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="76e08-121">if-match</span><span class="sxs-lookup"><span data-stu-id="76e08-121">if-match</span></span>      | <span data-ttu-id="76e08-122">String</span><span class="sxs-lookup"><span data-stu-id="76e08-122">String</span></span> | <span data-ttu-id="76e08-123">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="76e08-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="76e08-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76e08-124">Example</span></span>

<span data-ttu-id="76e08-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="76e08-125">Here is an example of how to call this API.</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="76e08-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="76e08-126">Response</span></span>

<span data-ttu-id="76e08-127">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="76e08-127">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="76e08-128">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="76e08-128">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="76e08-129">Basic</span><span class="sxs-lookup"><span data-stu-id="76e08-129">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76e08-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76e08-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-responses"></a><span data-ttu-id="76e08-131">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="76e08-131">Error responses</span></span>

<span data-ttu-id="76e08-132">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="76e08-132">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
