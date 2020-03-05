---
title: Excluir conversationThread
description: Exclua um conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0f2d5f157c712ed76ebce77c68ac163236a5fdec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436409"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="9a788-103">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="9a788-103">Delete conversationThread</span></span>

<span data-ttu-id="9a788-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9a788-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a788-105">Exclua um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="9a788-105">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a788-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a788-106">Permissions</span></span>
<span data-ttu-id="9a788-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a788-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a788-109">Permission type</span></span>      | <span data-ttu-id="9a788-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a788-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a788-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a788-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a788-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a788-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a788-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a788-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a788-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a788-114">Not supported.</span></span>    |
|<span data-ttu-id="9a788-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a788-115">Application</span></span> | <span data-ttu-id="9a788-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a788-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a788-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a788-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9a788-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a788-118">Request headers</span></span>
| <span data-ttu-id="9a788-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a788-119">Header</span></span>       | <span data-ttu-id="9a788-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9a788-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a788-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a788-121">Authorization</span></span>  | <span data-ttu-id="9a788-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a788-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a788-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a788-124">Request body</span></span>
<span data-ttu-id="9a788-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a788-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a788-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a788-126">Response</span></span>

<span data-ttu-id="9a788-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a788-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a788-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a788-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a788-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a788-130">Request</span></span>
<span data-ttu-id="9a788-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a788-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a788-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a788-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="c"></a>[<span data-ttu-id="9a788-133">C#</span><span class="sxs-lookup"><span data-stu-id="9a788-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a788-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a788-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a788-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a788-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a788-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a788-136">Response</span></span>
<span data-ttu-id="9a788-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a788-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
