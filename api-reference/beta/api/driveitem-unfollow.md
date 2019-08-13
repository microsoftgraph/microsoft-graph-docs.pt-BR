---
author: chackman
ms.author: chackman
description: Não siga um item que o usuário está seguindo.
title: Item da unidade não seguir
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 3ac8e3af809a9e324f69e66d1ef3c6f8f83aa840
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320935"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="b41d9-103">Item da unidade não seguir</span><span class="sxs-lookup"><span data-stu-id="b41d9-103">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b41d9-104">Não seguir um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b41d9-104">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="b41d9-105">**Observação:** Para seguir um item, consulte [follow item](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="b41d9-105">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b41d9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b41d9-106">Permissions</span></span>

<span data-ttu-id="b41d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b41d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b41d9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b41d9-109">Permission type</span></span>      | <span data-ttu-id="b41d9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b41d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b41d9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b41d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b41d9-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b41d9-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b41d9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b41d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b41d9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b41d9-114">Not supported.</span></span>    |
|<span data-ttu-id="b41d9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b41d9-115">Application</span></span> | <span data-ttu-id="b41d9-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b41d9-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b41d9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b41d9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id}
DELETE /users/{user-id}/drive/following/{item-id}
POST /me/drive/items/{item-id}/unfollow
POST /users/{user-id}/drive/items/{item-id}/unfollow
```

## <a name="request-body"></a><span data-ttu-id="b41d9-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b41d9-118">Request body</span></span>

<span data-ttu-id="b41d9-119">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b41d9-119">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="b41d9-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="b41d9-120">Response</span></span>

<span data-ttu-id="b41d9-121">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b41d9-121">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="b41d9-122">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b41d9-122">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b41d9-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b41d9-123">Example</span></span>
### <a name="request"></a><span data-ttu-id="b41d9-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b41d9-124">Request</span></span>
<span data-ttu-id="b41d9-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b41d9-125">Here is an example of the request.</span></span>
<span data-ttu-id="b41d9-126">Este exemplo não segue um item identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="b41d9-126">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b41d9-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="b41d9-127">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/items/{item-id}/unfollow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b41d9-128">C#</span><span class="sxs-lookup"><span data-stu-id="b41d9-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b41d9-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b41d9-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b41d9-130">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b41d9-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b41d9-131">Java</span><span class="sxs-lookup"><span data-stu-id="b41d9-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b41d9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b41d9-132">Response</span></span>
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
