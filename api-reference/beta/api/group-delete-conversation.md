---
title: Excluir conversa
description: Excluir um objeto conversation.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5da2c54e86cb6d59c8220be89f05681914fd56b7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042020"
---
# <a name="delete-conversation"></a><span data-ttu-id="b050a-103">Excluir conversa</span><span class="sxs-lookup"><span data-stu-id="b050a-103">Delete conversation</span></span>

<span data-ttu-id="b050a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b050a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b050a-105">Excluir um objeto [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="b050a-105">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b050a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b050a-106">Permissions</span></span>
<span data-ttu-id="b050a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b050a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b050a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b050a-109">Permission type</span></span>      | <span data-ttu-id="b050a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b050a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b050a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b050a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b050a-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b050a-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b050a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b050a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b050a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b050a-114">Not supported.</span></span>    |
|<span data-ttu-id="b050a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b050a-115">Application</span></span> | <span data-ttu-id="b050a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b050a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b050a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b050a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b050a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b050a-118">Request headers</span></span>
| <span data-ttu-id="b050a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b050a-119">Name</span></span>       | <span data-ttu-id="b050a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b050a-120">Type</span></span> | <span data-ttu-id="b050a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b050a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b050a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b050a-122">Authorization</span></span>  | <span data-ttu-id="b050a-123">string</span><span class="sxs-lookup"><span data-stu-id="b050a-123">string</span></span>  | <span data-ttu-id="b050a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b050a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b050a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b050a-126">Request body</span></span>
<span data-ttu-id="b050a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b050a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b050a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b050a-128">Response</span></span>
<span data-ttu-id="b050a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b050a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b050a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b050a-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b050a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b050a-132">Request</span></span>
<span data-ttu-id="b050a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b050a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b050a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b050a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="c"></a>[<span data-ttu-id="b050a-135">C#</span><span class="sxs-lookup"><span data-stu-id="b050a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b050a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b050a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b050a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b050a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b050a-138">Java</span><span class="sxs-lookup"><span data-stu-id="b050a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b050a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b050a-139">Response</span></span>
<span data-ttu-id="b050a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b050a-140">The following is an example of the response.</span></span> 
><span data-ttu-id="b050a-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b050a-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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


