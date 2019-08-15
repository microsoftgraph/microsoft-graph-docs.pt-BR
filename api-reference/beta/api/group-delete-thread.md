---
title: Excluir thread de conversas
description: Excluir um objeto thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 65d46fdbc9a8b449e09e5a1e7ed98b44f82348eb
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420298"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="52dca-103">Excluir thread de conversas</span><span class="sxs-lookup"><span data-stu-id="52dca-103">Delete conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52dca-104">Excluir um objeto [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="52dca-104">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="52dca-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="52dca-105">Permissions</span></span>
<span data-ttu-id="52dca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52dca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52dca-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52dca-108">Permission type</span></span>      | <span data-ttu-id="52dca-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52dca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52dca-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52dca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="52dca-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52dca-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="52dca-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52dca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52dca-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52dca-113">Not supported.</span></span>    |
|<span data-ttu-id="52dca-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52dca-114">Application</span></span> | <span data-ttu-id="52dca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52dca-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52dca-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52dca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="52dca-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52dca-117">Request headers</span></span>
| <span data-ttu-id="52dca-118">Nome</span><span class="sxs-lookup"><span data-stu-id="52dca-118">Name</span></span>       | <span data-ttu-id="52dca-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="52dca-119">Type</span></span> | <span data-ttu-id="52dca-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="52dca-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="52dca-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="52dca-121">Authorization</span></span>  | <span data-ttu-id="52dca-122">string</span><span class="sxs-lookup"><span data-stu-id="52dca-122">string</span></span>  | <span data-ttu-id="52dca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52dca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52dca-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52dca-125">Request body</span></span>
<span data-ttu-id="52dca-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52dca-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52dca-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="52dca-127">Response</span></span>
<span data-ttu-id="52dca-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52dca-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52dca-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52dca-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="52dca-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52dca-131">Request</span></span>
<span data-ttu-id="52dca-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52dca-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="52dca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="52dca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="52dca-134">C#</span><span class="sxs-lookup"><span data-stu-id="52dca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52dca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52dca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52dca-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="52dca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="52dca-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="52dca-137">Response</span></span>
<span data-ttu-id="52dca-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52dca-138">The following is an example of the response.</span></span> 
><span data-ttu-id="52dca-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52dca-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
