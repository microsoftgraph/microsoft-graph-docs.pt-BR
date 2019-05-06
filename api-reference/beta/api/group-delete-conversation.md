---
title: Excluir conversa
description: Excluir um objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d944c4660cf542535b6a7cd46bde32f042862edd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593362"
---
# <a name="delete-conversation"></a><span data-ttu-id="b9527-103">Excluir conversa</span><span class="sxs-lookup"><span data-stu-id="b9527-103">Delete conversation</span></span>
<span data-ttu-id="b9527-104">Excluir um objeto [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="b9527-104">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9527-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9527-105">Permissions</span></span>
<span data-ttu-id="b9527-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9527-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9527-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9527-108">Permission type</span></span>      | <span data-ttu-id="b9527-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9527-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9527-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9527-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b9527-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9527-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b9527-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9527-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9527-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9527-113">Not supported.</span></span>    |
|<span data-ttu-id="b9527-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9527-114">Application</span></span> | <span data-ttu-id="b9527-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9527-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9527-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9527-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b9527-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9527-117">Request headers</span></span>
| <span data-ttu-id="b9527-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b9527-118">Name</span></span>       | <span data-ttu-id="b9527-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9527-119">Type</span></span> | <span data-ttu-id="b9527-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9527-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b9527-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9527-121">Authorization</span></span>  | <span data-ttu-id="b9527-122">string</span><span class="sxs-lookup"><span data-stu-id="b9527-122">string</span></span>  | <span data-ttu-id="b9527-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9527-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9527-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9527-125">Request body</span></span>
<span data-ttu-id="b9527-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9527-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9527-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9527-127">Response</span></span>
<span data-ttu-id="b9527-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9527-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9527-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9527-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b9527-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9527-131">Request</span></span>
<span data-ttu-id="b9527-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9527-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="b9527-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9527-133">Response</span></span>
<span data-ttu-id="b9527-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b9527-134">The following is an example of the response.</span></span> 
><span data-ttu-id="b9527-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9527-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b9527-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b9527-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b9527-138">Basic</span><span class="sxs-lookup"><span data-stu-id="b9527-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_group_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9527-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9527-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_group_conversation-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-delete-conversation.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete-conversation.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
