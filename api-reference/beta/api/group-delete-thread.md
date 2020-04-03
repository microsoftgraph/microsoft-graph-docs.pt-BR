---
title: Excluir thread de conversas
description: Excluir um objeto thread.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ef30de64fe4696388259785132dc7d765aca4d28
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123808"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="9cc9f-103">Excluir thread de conversas</span><span class="sxs-lookup"><span data-stu-id="9cc9f-103">Delete conversation thread</span></span>

<span data-ttu-id="9cc9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cc9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cc9f-105">Excluir um objeto [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="9cc9f-105">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cc9f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cc9f-106">Permissions</span></span>
<span data-ttu-id="9cc9f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cc9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cc9f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cc9f-109">Permission type</span></span>      | <span data-ttu-id="9cc9f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cc9f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cc9f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cc9f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9cc9f-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc9f-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9cc9f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cc9f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cc9f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cc9f-114">Not supported.</span></span>    |
|<span data-ttu-id="9cc9f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cc9f-115">Application</span></span> | <span data-ttu-id="9cc9f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cc9f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cc9f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc9f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9cc9f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc9f-118">Request headers</span></span>
| <span data-ttu-id="9cc9f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9cc9f-119">Name</span></span>       | <span data-ttu-id="9cc9f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cc9f-120">Type</span></span> | <span data-ttu-id="9cc9f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cc9f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9cc9f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cc9f-122">Authorization</span></span>  | <span data-ttu-id="9cc9f-123">string</span><span class="sxs-lookup"><span data-stu-id="9cc9f-123">string</span></span>  | <span data-ttu-id="9cc9f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cc9f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cc9f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc9f-126">Request body</span></span>
<span data-ttu-id="9cc9f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9cc9f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cc9f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc9f-128">Response</span></span>
<span data-ttu-id="9cc9f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc9f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cc9f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9cc9f-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9cc9f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cc9f-132">Request</span></span>
<span data-ttu-id="9cc9f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cc9f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9cc9f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cc9f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="c"></a>[<span data-ttu-id="9cc9f-135">C#</span><span class="sxs-lookup"><span data-stu-id="9cc9f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cc9f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cc9f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cc9f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cc9f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cc9f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cc9f-138">Response</span></span>
<span data-ttu-id="9cc9f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9cc9f-139">The following is an example of the response.</span></span> 
><span data-ttu-id="9cc9f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cc9f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
