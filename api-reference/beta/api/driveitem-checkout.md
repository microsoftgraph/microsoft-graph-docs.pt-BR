---
author: JeremyKelley
description: Check-out de um recurso driveItem para impedir que outras pessoas editem o documento e que suas alterações fiquem visíveis até que o documento passe por check-in.
ms.date: 09/10/2017
title: Fazer check-out de arquivos
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4159882b29dc69429a7b99bb89d1e8051d6e9c03
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432940"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="0d33b-103">Fazer check-out do recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="0d33b-103">Check-out a DriveItem resource</span></span>

<span data-ttu-id="0d33b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0d33b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d33b-105">Check-out de um recurso driveItem para impedir que outras pessoas editem o documento e que suas alterações fiquem visíveis até que o documento passe por [check-in](driveitem-checkin.md).</span><span class="sxs-lookup"><span data-stu-id="0d33b-105">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d33b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d33b-106">Permissions</span></span>

<span data-ttu-id="0d33b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d33b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d33b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d33b-109">Permission type</span></span>      | <span data-ttu-id="0d33b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d33b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d33b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d33b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d33b-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d33b-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0d33b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d33b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d33b-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d33b-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0d33b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d33b-115">Application</span></span> | <span data-ttu-id="0d33b-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d33b-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d33b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d33b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="0d33b-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d33b-118">Request body</span></span>

<span data-ttu-id="0d33b-119">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d33b-119">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="0d33b-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d33b-120">Example</span></span>

<span data-ttu-id="0d33b-121">Este exemplo faz check-out de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="0d33b-121">This example checks out a file identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d33b-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d33b-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="c"></a>[<span data-ttu-id="0d33b-123">C#</span><span class="sxs-lookup"><span data-stu-id="0d33b-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d33b-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d33b-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d33b-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d33b-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="0d33b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d33b-126">Response</span></span>

<span data-ttu-id="0d33b-127">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="0d33b-127">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="0d33b-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="0d33b-128">Remarks</span></span>


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
