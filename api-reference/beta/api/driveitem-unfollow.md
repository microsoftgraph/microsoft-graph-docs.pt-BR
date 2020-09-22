---
author: chackman
ms.author: chackman
description: Não siga um item que o usuário está seguindo.
title: Item da unidade não seguir
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 278840415b00270061e04a2aab71beb9f3cb6eb5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981839"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="2c009-103">Item da unidade não seguir</span><span class="sxs-lookup"><span data-stu-id="2c009-103">Unfollow drive item</span></span>

<span data-ttu-id="2c009-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c009-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c009-105">Não seguir um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2c009-105">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="2c009-106">**Observação:** Para seguir um item, consulte [follow item](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="2c009-106">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2c009-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c009-107">Permissions</span></span>

<span data-ttu-id="2c009-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c009-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c009-110">Permission type</span></span>      | <span data-ttu-id="2c009-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c009-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c009-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c009-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2c009-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c009-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c009-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c009-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c009-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c009-115">Not supported.</span></span>    |
|<span data-ttu-id="2c009-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c009-116">Application</span></span> | <span data-ttu-id="2c009-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c009-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c009-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c009-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id}
DELETE /users/{user-id}/drive/following/{item-id}
POST /me/drive/items/{item-id}/unfollow
POST /users/{user-id}/drive/items/{item-id}/unfollow
```

## <a name="request-body"></a><span data-ttu-id="2c009-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c009-119">Request body</span></span>

<span data-ttu-id="2c009-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c009-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="2c009-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c009-121">Response</span></span>

<span data-ttu-id="2c009-122">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2c009-122">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="2c009-123">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c009-123">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c009-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c009-124">Example</span></span>
### <a name="request"></a><span data-ttu-id="2c009-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c009-125">Request</span></span>
<span data-ttu-id="2c009-126">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c009-126">Here is an example of the request.</span></span>
<span data-ttu-id="2c009-127">Este exemplo não segue um item identificado por `{item-id}` .</span><span class="sxs-lookup"><span data-stu-id="2c009-127">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="2c009-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c009-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/items/{item-id}/unfollow
```
# <a name="c"></a>[<span data-ttu-id="2c009-129">C#</span><span class="sxs-lookup"><span data-stu-id="2c009-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c009-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c009-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c009-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c009-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2c009-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c009-132">Response</span></span>
<!-- { 
    "blockType": "response", 
    "truncated": true 
} -->
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
  ]
}
-->


