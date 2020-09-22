---
title: Excluir evento
description: Excluir um objeto event.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 155d755ef443fe623acdd2d6db2c8b13cd2571e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094873"
---
# <a name="delete-event"></a><span data-ttu-id="b6210-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="b6210-103">Delete event</span></span>

<span data-ttu-id="b6210-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6210-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6210-105">Excluir um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="b6210-105">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6210-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6210-106">Permissions</span></span>
<span data-ttu-id="b6210-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6210-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6210-109">Permission type</span></span>      | <span data-ttu-id="b6210-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6210-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6210-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6210-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b6210-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6210-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b6210-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6210-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6210-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6210-114">Not supported.</span></span>    |
|<span data-ttu-id="b6210-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6210-115">Application</span></span> | <span data-ttu-id="b6210-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6210-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6210-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6210-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b6210-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6210-118">Request headers</span></span>
| <span data-ttu-id="b6210-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b6210-119">Name</span></span>       | <span data-ttu-id="b6210-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6210-120">Type</span></span> | <span data-ttu-id="b6210-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6210-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b6210-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6210-122">Authorization</span></span>  | <span data-ttu-id="b6210-123">string</span><span class="sxs-lookup"><span data-stu-id="b6210-123">string</span></span>  | <span data-ttu-id="b6210-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6210-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6210-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6210-126">Request body</span></span>
<span data-ttu-id="b6210-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6210-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6210-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6210-128">Response</span></span>
<span data-ttu-id="b6210-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6210-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6210-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6210-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b6210-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6210-132">Request</span></span>
<span data-ttu-id="b6210-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6210-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6210-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6210-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="c"></a>[<span data-ttu-id="b6210-135">C#</span><span class="sxs-lookup"><span data-stu-id="b6210-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6210-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6210-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6210-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6210-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6210-138">Java</span><span class="sxs-lookup"><span data-stu-id="b6210-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b6210-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6210-139">Response</span></span>
<span data-ttu-id="b6210-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6210-140">The following is an example of the response.</span></span> 
><span data-ttu-id="b6210-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6210-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

