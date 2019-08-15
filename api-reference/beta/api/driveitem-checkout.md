---
author: JeremyKelley
description: Check-out de um recurso driveItem para impedir que outras pessoas editem o documento e que suas alterações fiquem visíveis até que o documento passe por check-in.
ms.date: 09/10/2017
title: Fazer check-out de arquivos
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: adde2c3deb03bf1f45a673ff6cc5d6d7a844544e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416860"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="b5b4d-103">Fazer check-out do recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="b5b4d-103">Check-out a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5b4d-104">Check-out de um recurso driveItem para impedir que outras pessoas editem o documento e que suas alterações fiquem visíveis até que o documento passe por [check-in](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="b5b4d-104">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5b4d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5b4d-105">Permissions</span></span>

<span data-ttu-id="b5b4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5b4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5b4d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5b4d-108">Permission type</span></span>      | <span data-ttu-id="b5b4d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5b4d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5b4d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5b4d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5b4d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5b4d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5b4d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5b4d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5b4d-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5b4d-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5b4d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5b4d-114">Application</span></span> | <span data-ttu-id="b5b4d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5b4d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5b4d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5b4d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="b5b4d-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5b4d-117">Request body</span></span>

<span data-ttu-id="b5b4d-118">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5b4d-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="b5b4d-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5b4d-119">Example</span></span>

<span data-ttu-id="b5b4d-120">Este exemplo faz check-out de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="b5b4d-120">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5b4d-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5b4d-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5b4d-122">C#</span><span class="sxs-lookup"><span data-stu-id="b5b4d-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5b4d-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5b4d-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5b4d-124">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b5b4d-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="b5b4d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5b4d-125">Response</span></span>

<span data-ttu-id="b5b4d-126">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="b5b4d-126">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="b5b4d-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="b5b4d-127">Remarks</span></span>


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
