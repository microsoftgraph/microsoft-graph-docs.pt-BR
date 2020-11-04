---
author: learafa
ms.author: learafa
description: Não siga um item que o usuário está seguindo.
title: Item da unidade não seguir
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 057ba8e3d75b9e78af19008060426ad695ca5543
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904189"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="600d2-103">Item da unidade não seguir</span><span class="sxs-lookup"><span data-stu-id="600d2-103">Unfollow drive item</span></span>

<span data-ttu-id="600d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="600d2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="600d2-105">Não seguir um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="600d2-105">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="600d2-106">**Observação:** Para seguir um item, consulte [follow item](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="600d2-106">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="600d2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="600d2-107">Permissions</span></span>

<span data-ttu-id="600d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="600d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="600d2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="600d2-110">Permission type</span></span>      | <span data-ttu-id="600d2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="600d2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="600d2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="600d2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="600d2-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="600d2-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="600d2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="600d2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="600d2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="600d2-115">Not supported.</span></span>    |
|<span data-ttu-id="600d2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="600d2-116">Application</span></span> | <span data-ttu-id="600d2-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="600d2-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="600d2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="600d2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id}
DELETE /users/{user-id}/drive/following/{item-id}
POST /me/drive/items/{item-id}/unfollow
POST /users/{user-id}/drive/items/{item-id}/unfollow
```

## <a name="request-body"></a><span data-ttu-id="600d2-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="600d2-119">Request body</span></span>

<span data-ttu-id="600d2-120">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="600d2-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="600d2-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="600d2-121">Response</span></span>

<span data-ttu-id="600d2-122">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="600d2-122">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="600d2-123">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="600d2-123">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="600d2-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="600d2-124">Example</span></span>
### <a name="request"></a><span data-ttu-id="600d2-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="600d2-125">Request</span></span>
<span data-ttu-id="600d2-126">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="600d2-126">Here is an example of the request.</span></span>
<span data-ttu-id="600d2-127">Este exemplo não segue um item identificado por `{item-id}` .</span><span class="sxs-lookup"><span data-stu-id="600d2-127">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="600d2-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="600d2-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
POST /me/drive/items/{item-id}/unfollow
```
# <a name="c"></a>[<span data-ttu-id="600d2-129">C#</span><span class="sxs-lookup"><span data-stu-id="600d2-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="600d2-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="600d2-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="600d2-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="600d2-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="600d2-132">Java</span><span class="sxs-lookup"><span data-stu-id="600d2-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="600d2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="600d2-133">Response</span></span>
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

