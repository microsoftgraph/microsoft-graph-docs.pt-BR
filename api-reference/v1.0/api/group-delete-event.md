---
title: Excluir evento
description: Excluir um objeto event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 32822c885b79e60d709d8f583e22b9db68c61164
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448121"
---
# <a name="delete-event"></a><span data-ttu-id="46708-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="46708-103">Delete event</span></span>
<span data-ttu-id="46708-104">Excluir um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="46708-104">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46708-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="46708-105">Permissions</span></span>
<span data-ttu-id="46708-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46708-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46708-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46708-108">Permission type</span></span>      | <span data-ttu-id="46708-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46708-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46708-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46708-110">Delegated (work or school account)</span></span> | <span data-ttu-id="46708-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46708-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="46708-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46708-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46708-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46708-113">Not supported.</span></span>    |
|<span data-ttu-id="46708-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46708-114">Application</span></span> | <span data-ttu-id="46708-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46708-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46708-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46708-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="46708-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46708-117">Request headers</span></span>
| <span data-ttu-id="46708-118">Nome</span><span class="sxs-lookup"><span data-stu-id="46708-118">Name</span></span>       | <span data-ttu-id="46708-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="46708-119">Type</span></span> | <span data-ttu-id="46708-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="46708-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46708-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="46708-121">Authorization</span></span>  | <span data-ttu-id="46708-122">string</span><span class="sxs-lookup"><span data-stu-id="46708-122">string</span></span>  | <span data-ttu-id="46708-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46708-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46708-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46708-125">Request body</span></span>
<span data-ttu-id="46708-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46708-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46708-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="46708-127">Response</span></span>
<span data-ttu-id="46708-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46708-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46708-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46708-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="46708-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46708-131">Request</span></span>
<span data-ttu-id="46708-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46708-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46708-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="46708-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46708-134">C#</span><span class="sxs-lookup"><span data-stu-id="46708-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46708-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="46708-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46708-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="46708-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="46708-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="46708-137">Response</span></span>
<span data-ttu-id="46708-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46708-138">The following is an example of the response.</span></span> 
><span data-ttu-id="46708-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46708-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
