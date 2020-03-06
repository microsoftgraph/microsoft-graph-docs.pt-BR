---
title: Excluir conversationThread
description: Exclua um conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6a35ac0bc0c6149db0f6f5c8cc886b2cd92ae60c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518186"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="50d91-103">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="50d91-103">Delete conversationThread</span></span>

<span data-ttu-id="50d91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50d91-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50d91-105">Exclua um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="50d91-105">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="50d91-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="50d91-106">Permissions</span></span>
<span data-ttu-id="50d91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50d91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50d91-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50d91-109">Permission type</span></span>      | <span data-ttu-id="50d91-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50d91-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50d91-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50d91-111">Delegated (work or school account)</span></span> | <span data-ttu-id="50d91-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d91-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="50d91-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50d91-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50d91-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50d91-114">Not supported.</span></span>    |
|<span data-ttu-id="50d91-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50d91-115">Application</span></span> | <span data-ttu-id="50d91-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d91-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50d91-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50d91-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="50d91-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50d91-118">Request headers</span></span>
| <span data-ttu-id="50d91-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50d91-119">Header</span></span>       | <span data-ttu-id="50d91-120">Valor</span><span class="sxs-lookup"><span data-stu-id="50d91-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="50d91-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="50d91-121">Authorization</span></span>  | <span data-ttu-id="50d91-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50d91-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50d91-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50d91-124">Request body</span></span>
<span data-ttu-id="50d91-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50d91-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50d91-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="50d91-126">Response</span></span>

<span data-ttu-id="50d91-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50d91-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50d91-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50d91-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50d91-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50d91-130">Request</span></span>
<span data-ttu-id="50d91-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50d91-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="50d91-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="50d91-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
# <a name="c"></a>[<span data-ttu-id="50d91-133">C#</span><span class="sxs-lookup"><span data-stu-id="50d91-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50d91-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50d91-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50d91-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50d91-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50d91-136">Java</span><span class="sxs-lookup"><span data-stu-id="50d91-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="50d91-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="50d91-137">Response</span></span>
<span data-ttu-id="50d91-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50d91-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
