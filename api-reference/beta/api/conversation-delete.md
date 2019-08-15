---
title: Excluir conversa
description: Exclua uma conversa.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5c4eacb1fa1c07bcb7f92f348340256fc04022a6
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417855"
---
# <a name="delete-conversation"></a><span data-ttu-id="df1ab-103">Excluir conversa</span><span class="sxs-lookup"><span data-stu-id="df1ab-103">Delete conversation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df1ab-104">Exclua uma conversa.</span><span class="sxs-lookup"><span data-stu-id="df1ab-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="df1ab-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="df1ab-105">Permissions</span></span>
<span data-ttu-id="df1ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df1ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df1ab-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df1ab-108">Permission type</span></span>      | <span data-ttu-id="df1ab-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df1ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df1ab-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df1ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="df1ab-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df1ab-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="df1ab-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df1ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df1ab-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df1ab-113">Not supported.</span></span>    |
|<span data-ttu-id="df1ab-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df1ab-114">Application</span></span> | <span data-ttu-id="df1ab-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df1ab-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df1ab-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df1ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="df1ab-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df1ab-117">Request headers</span></span>
| <span data-ttu-id="df1ab-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df1ab-118">Header</span></span>       | <span data-ttu-id="df1ab-119">Valor</span><span class="sxs-lookup"><span data-stu-id="df1ab-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df1ab-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="df1ab-120">Authorization</span></span>  | <span data-ttu-id="df1ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df1ab-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df1ab-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df1ab-123">Request body</span></span>
<span data-ttu-id="df1ab-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df1ab-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df1ab-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="df1ab-125">Response</span></span>

<span data-ttu-id="df1ab-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df1ab-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df1ab-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df1ab-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df1ab-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df1ab-129">Request</span></span>
<span data-ttu-id="df1ab-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df1ab-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="df1ab-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="df1ab-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="df1ab-132">C#</span><span class="sxs-lookup"><span data-stu-id="df1ab-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df1ab-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df1ab-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="df1ab-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="df1ab-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="df1ab-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="df1ab-135">Response</span></span>
<span data-ttu-id="df1ab-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df1ab-136">Here is an example of the response.</span></span> 
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
