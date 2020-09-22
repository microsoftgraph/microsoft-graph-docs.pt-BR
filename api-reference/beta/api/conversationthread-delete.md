---
title: Excluir conversationThread
description: Exclua um conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2e2692b17a0146826d38a033b4b04e6a1119248f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002692"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="4ba45-103">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="4ba45-103">Delete conversationThread</span></span>

<span data-ttu-id="4ba45-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4ba45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ba45-105">Exclua um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="4ba45-105">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ba45-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ba45-106">Permissions</span></span>
<span data-ttu-id="4ba45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ba45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ba45-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ba45-109">Permission type</span></span>      | <span data-ttu-id="4ba45-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ba45-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ba45-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ba45-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ba45-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ba45-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ba45-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ba45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ba45-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ba45-114">Not supported.</span></span>    |
|<span data-ttu-id="4ba45-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ba45-115">Application</span></span> | <span data-ttu-id="4ba45-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ba45-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ba45-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ba45-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="4ba45-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ba45-118">Request headers</span></span>
| <span data-ttu-id="4ba45-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ba45-119">Header</span></span>       | <span data-ttu-id="4ba45-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4ba45-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ba45-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ba45-121">Authorization</span></span>  | <span data-ttu-id="4ba45-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ba45-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ba45-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ba45-124">Request body</span></span>
<span data-ttu-id="4ba45-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ba45-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ba45-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ba45-126">Response</span></span>

<span data-ttu-id="4ba45-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ba45-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ba45-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ba45-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ba45-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ba45-130">Request</span></span>
<span data-ttu-id="4ba45-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ba45-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ba45-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ba45-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="c"></a>[<span data-ttu-id="4ba45-133">C#</span><span class="sxs-lookup"><span data-stu-id="4ba45-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ba45-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ba45-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ba45-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ba45-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4ba45-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ba45-136">Response</span></span>
<span data-ttu-id="4ba45-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ba45-137">Here is an example of the response.</span></span> 
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


