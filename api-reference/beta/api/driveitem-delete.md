---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Excluir um arquivo ou uma pasta
localization_priority: Normal
ms.openlocfilehash: 8357b170023f905494df73ca1e4420f87a914a77
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843362"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="77301-102">Excluir um DriveItem</span><span class="sxs-lookup"><span data-stu-id="77301-102">Delete a DriveItem</span></span>

> <span data-ttu-id="77301-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="77301-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77301-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="77301-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77301-p102">Excluir um [DriveItem](../resources/driveitem.md) usando sua ID ou seu caminho. Observe que a exclusão de itens usando esse método moverá os itens para a Lixeira, ao invés de excluir permanentemente o item.</span><span class="sxs-lookup"><span data-stu-id="77301-p102">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="77301-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="77301-107">Permissions</span></span>

<span data-ttu-id="77301-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77301-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77301-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77301-110">Permission type</span></span>      | <span data-ttu-id="77301-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77301-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77301-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77301-112">Delegated (work or school account)</span></span> | <span data-ttu-id="77301-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77301-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="77301-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77301-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77301-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77301-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="77301-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77301-116">Application</span></span> | <span data-ttu-id="77301-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77301-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77301-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77301-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="77301-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="77301-119">Optional request headers</span></span>

| <span data-ttu-id="77301-120">Nome</span><span class="sxs-lookup"><span data-stu-id="77301-120">Name</span></span>          | <span data-ttu-id="77301-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="77301-121">Type</span></span>   | <span data-ttu-id="77301-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="77301-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="77301-123">if-match</span><span class="sxs-lookup"><span data-stu-id="77301-123">if-match</span></span>      | <span data-ttu-id="77301-124">String</span><span class="sxs-lookup"><span data-stu-id="77301-124">String</span></span> | <span data-ttu-id="77301-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="77301-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="77301-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77301-126">Example</span></span>

<span data-ttu-id="77301-127">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="77301-127">Here is an example of how to call this API.</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="77301-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="77301-128">Response</span></span>

<span data-ttu-id="77301-129">Se bem sucedida, esta chamada retorna uma resposta `204 No Content` para indicar que o recurso foi excluído e que não havia nada a retornar.</span><span class="sxs-lookup"><span data-stu-id="77301-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="77301-130">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="77301-130">Error responses</span></span>

<span data-ttu-id="77301-131">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="77301-131">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete"
} -->
