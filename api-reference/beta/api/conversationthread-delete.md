---
title: Excluir conversationThread
description: Exclua um conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f82a026cca65e1584cf4c46896ab0526622d5305
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417792"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="e7242-103">Excluir conversationThread</span><span class="sxs-lookup"><span data-stu-id="e7242-103">Delete conversationThread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7242-104">Exclua um conversationThread.</span><span class="sxs-lookup"><span data-stu-id="e7242-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7242-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7242-105">Permissions</span></span>
<span data-ttu-id="e7242-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7242-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7242-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7242-108">Permission type</span></span>      | <span data-ttu-id="e7242-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7242-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7242-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7242-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7242-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7242-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7242-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7242-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7242-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7242-113">Not supported.</span></span>    |
|<span data-ttu-id="e7242-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7242-114">Application</span></span> | <span data-ttu-id="e7242-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7242-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7242-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7242-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="e7242-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7242-117">Request headers</span></span>
| <span data-ttu-id="e7242-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7242-118">Header</span></span>       | <span data-ttu-id="e7242-119">Valor</span><span class="sxs-lookup"><span data-stu-id="e7242-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e7242-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7242-120">Authorization</span></span>  | <span data-ttu-id="e7242-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7242-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7242-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7242-123">Request body</span></span>
<span data-ttu-id="e7242-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7242-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7242-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7242-125">Response</span></span>

<span data-ttu-id="e7242-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7242-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7242-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7242-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7242-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7242-129">Request</span></span>
<span data-ttu-id="e7242-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7242-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e7242-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7242-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7242-132">C#</span><span class="sxs-lookup"><span data-stu-id="e7242-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7242-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7242-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7242-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e7242-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e7242-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7242-135">Response</span></span>
<span data-ttu-id="e7242-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7242-136">Here is an example of the response.</span></span> 
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
