---
author: learafa
description: Confira um recurso driveItem para impedir que outras pessoas editem o documento e suas alterações sejam visíveis até que a documentação esteja marcada.
title: 'driveItem: checkout'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 60b9f5de40f925354a0513c1b467295bf24ccb85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009895"
---
# <a name="driveitem-checkout"></a><span data-ttu-id="41919-103">driveItem: checkout</span><span class="sxs-lookup"><span data-stu-id="41919-103">driveItem: checkout</span></span>

<span data-ttu-id="41919-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41919-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41919-105">Confira um recurso **driveItem** para impedir que outras pessoas editem o documento e impedir que as alterações sejam visíveis até que seja [feito o check-in](driveitem-checkin.md)documentado.</span><span class="sxs-lookup"><span data-stu-id="41919-105">Check out a **driveItem** resource to prevent others from editing the document, and prevent your changes from being visible until the documented is [checked in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="41919-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41919-106">Permissions</span></span>

<span data-ttu-id="41919-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41919-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41919-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41919-109">Permission type</span></span>      | <span data-ttu-id="41919-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41919-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41919-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41919-111">Delegated (work or school account)</span></span> | <span data-ttu-id="41919-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41919-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="41919-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41919-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41919-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41919-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="41919-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41919-115">Application</span></span> | <span data-ttu-id="41919-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41919-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41919-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41919-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

## <a name="request-body"></a><span data-ttu-id="41919-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41919-118">Request body</span></span>

<span data-ttu-id="41919-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41919-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41919-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="41919-120">Response</span></span>

<span data-ttu-id="41919-121">Se tiver êxito, a chamada de API retornará `204 No content` .</span><span class="sxs-lookup"><span data-stu-id="41919-121">If successful, the API call returns `204 No content`.</span></span>

## <a name="example"></a><span data-ttu-id="41919-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41919-122">Example</span></span>

<span data-ttu-id="41919-123">Este exemplo faz check-out de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="41919-123">This example checks out a file identified by `{item-id}`.</span></span>

### <a name="request"></a><span data-ttu-id="41919-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41919-124">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="41919-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="41919-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```
# <a name="c"></a>[<span data-ttu-id="41919-126">C#</span><span class="sxs-lookup"><span data-stu-id="41919-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkout-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41919-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41919-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkout-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41919-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41919-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkout-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41919-129">Java</span><span class="sxs-lookup"><span data-stu-id="41919-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkout-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41919-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="41919-130">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```


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

