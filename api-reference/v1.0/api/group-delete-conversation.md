---
title: Excluir conversa
description: Excluir um objeto conversation.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 962216fbb34f63de654de877b2833befab95b739
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682604"
---
# <a name="delete-conversation"></a><span data-ttu-id="6e450-103">Excluir conversa</span><span class="sxs-lookup"><span data-stu-id="6e450-103">Delete conversation</span></span>

<span data-ttu-id="6e450-104">Namespace: microsoft.graph Excluir um [objeto de](../resources/conversation.md) conversa.</span><span class="sxs-lookup"><span data-stu-id="6e450-104">Namespace: microsoft.graph Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e450-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e450-105">Permissions</span></span>
<span data-ttu-id="6e450-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e450-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e450-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e450-108">Permission type</span></span>      | <span data-ttu-id="6e450-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e450-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e450-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e450-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6e450-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e450-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e450-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e450-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e450-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e450-113">Not supported.</span></span>    |
|<span data-ttu-id="6e450-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e450-114">Application</span></span> | <span data-ttu-id="6e450-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e450-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e450-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e450-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6e450-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e450-117">Request headers</span></span>
| <span data-ttu-id="6e450-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6e450-118">Name</span></span>       | <span data-ttu-id="6e450-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e450-119">Type</span></span> | <span data-ttu-id="6e450-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e450-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6e450-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e450-121">Authorization</span></span>  | <span data-ttu-id="6e450-122">string</span><span class="sxs-lookup"><span data-stu-id="6e450-122">string</span></span>  | <span data-ttu-id="6e450-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e450-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e450-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e450-125">Request body</span></span>
<span data-ttu-id="6e450-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e450-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e450-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e450-127">Response</span></span>
<span data-ttu-id="6e450-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e450-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e450-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e450-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6e450-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e450-131">Request</span></span>
<span data-ttu-id="6e450-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e450-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6e450-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e450-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="c"></a>[<span data-ttu-id="6e450-134">C#</span><span class="sxs-lookup"><span data-stu-id="6e450-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e450-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e450-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e450-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e450-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e450-137">Java</span><span class="sxs-lookup"><span data-stu-id="6e450-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6e450-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e450-138">Response</span></span>
<span data-ttu-id="6e450-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6e450-139">The following is an example of the response.</span></span> 
><span data-ttu-id="6e450-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6e450-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

