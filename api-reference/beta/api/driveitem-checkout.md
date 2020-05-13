---
author: JeremyKelley
description: Confira um recurso driveItem para impedir que outras pessoas editem o documento e suas alterações sejam visíveis até que a documentação esteja marcada.
title: 'driveItem: checkout'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 69f01b949d38d76be24834151c10581589b75e2e
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43227586"
---
# <a name="driveitem-checkout"></a><span data-ttu-id="2b73b-103">driveItem: checkout</span><span class="sxs-lookup"><span data-stu-id="2b73b-103">driveItem: checkout</span></span>

<span data-ttu-id="2b73b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b73b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b73b-105">Confira um recurso **driveItem** para impedir que outras pessoas editem o documento e impedir que as alterações sejam visíveis até que seja [feito o check-in](driveitem-checkin.md)documentado.</span><span class="sxs-lookup"><span data-stu-id="2b73b-105">Check out a **driveItem** resource to prevent others from editing the document, and prevent your changes from being visible until the documented is [checked in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b73b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b73b-106">Permissions</span></span>

<span data-ttu-id="2b73b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b73b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b73b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b73b-109">Permission type</span></span>      | <span data-ttu-id="2b73b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b73b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b73b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b73b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2b73b-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b73b-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b73b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b73b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b73b-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b73b-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2b73b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b73b-115">Application</span></span> | <span data-ttu-id="2b73b-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b73b-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b73b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b73b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="2b73b-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b73b-118">Request body</span></span>

<span data-ttu-id="2b73b-119">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b73b-119">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="2b73b-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b73b-120">Example</span></span>

<span data-ttu-id="2b73b-121">Este exemplo faz check-out de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="2b73b-121">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b73b-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b73b-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="c"></a>[<span data-ttu-id="2b73b-123">C#</span><span class="sxs-lookup"><span data-stu-id="2b73b-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b73b-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b73b-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b73b-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b73b-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="2b73b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b73b-126">Response</span></span>

<span data-ttu-id="2b73b-127">Se tiver êxito, a chamada de API retornará `204 No content` .</span><span class="sxs-lookup"><span data-stu-id="2b73b-127">If successful, the API call returns `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="2b73b-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="2b73b-128">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
