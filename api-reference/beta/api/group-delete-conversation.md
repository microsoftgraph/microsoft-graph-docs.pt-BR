---
title: Excluir conversa
description: Excluir um objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 64caa44bb3d208d06b3e6105eb2081d454f2ae0c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954039"
---
# <a name="delete-conversation"></a><span data-ttu-id="f0c0d-103">Excluir conversa</span><span class="sxs-lookup"><span data-stu-id="f0c0d-103">Delete conversation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0c0d-104">Excluir um objeto [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="f0c0d-104">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0c0d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0c0d-105">Permissions</span></span>
<span data-ttu-id="f0c0d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0c0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0c0d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0c0d-108">Permission type</span></span>      | <span data-ttu-id="f0c0d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0c0d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0c0d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0c0d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f0c0d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0c0d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f0c0d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0c0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0c0d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0c0d-113">Not supported.</span></span>    |
|<span data-ttu-id="f0c0d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0c0d-114">Application</span></span> | <span data-ttu-id="f0c0d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0c0d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0c0d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0c0d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f0c0d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c0d-117">Request headers</span></span>
| <span data-ttu-id="f0c0d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f0c0d-118">Name</span></span>       | <span data-ttu-id="f0c0d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0c0d-119">Type</span></span> | <span data-ttu-id="f0c0d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0c0d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f0c0d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0c0d-121">Authorization</span></span>  | <span data-ttu-id="f0c0d-122">string</span><span class="sxs-lookup"><span data-stu-id="f0c0d-122">string</span></span>  | <span data-ttu-id="f0c0d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0c0d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0c0d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c0d-125">Request body</span></span>
<span data-ttu-id="f0c0d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0c0d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0c0d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0c0d-127">Response</span></span>
<span data-ttu-id="f0c0d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0c0d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0c0d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0c0d-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f0c0d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c0d-131">Request</span></span>
<span data-ttu-id="f0c0d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0c0d-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f0c0d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0c0d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f0c0d-134">C#</span><span class="sxs-lookup"><span data-stu-id="f0c0d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f0c0d-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="f0c0d-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f0c0d-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f0c0d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f0c0d-137">Java</span><span class="sxs-lookup"><span data-stu-id="f0c0d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f0c0d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0c0d-138">Response</span></span>
<span data-ttu-id="f0c0d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f0c0d-139">The following is an example of the response.</span></span> 
><span data-ttu-id="f0c0d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0c0d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
