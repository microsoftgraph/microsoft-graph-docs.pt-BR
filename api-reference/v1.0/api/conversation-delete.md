---
title: Excluir conversa
description: Exclua uma conversa.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: af498b79b42e4f56d8ed9c9ca5897cc0f2e1a03b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273833"
---
# <a name="delete-conversation"></a><span data-ttu-id="4d8a2-103">Excluir conversa</span><span class="sxs-lookup"><span data-stu-id="4d8a2-103">Delete conversation</span></span>

<span data-ttu-id="4d8a2-104">Exclua uma conversa.</span><span class="sxs-lookup"><span data-stu-id="4d8a2-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d8a2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d8a2-105">Permissions</span></span>
<span data-ttu-id="4d8a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d8a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d8a2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d8a2-108">Permission type</span></span>      | <span data-ttu-id="4d8a2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d8a2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d8a2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d8a2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d8a2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d8a2-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d8a2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d8a2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d8a2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d8a2-113">Not supported.</span></span>    |
|<span data-ttu-id="4d8a2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d8a2-114">Application</span></span> | <span data-ttu-id="4d8a2-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d8a2-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d8a2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d8a2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4d8a2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d8a2-117">Request headers</span></span>
| <span data-ttu-id="4d8a2-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d8a2-118">Header</span></span>       | <span data-ttu-id="4d8a2-119">Valor</span><span class="sxs-lookup"><span data-stu-id="4d8a2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d8a2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d8a2-120">Authorization</span></span>  | <span data-ttu-id="4d8a2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d8a2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d8a2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d8a2-123">Request body</span></span>
<span data-ttu-id="4d8a2-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d8a2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d8a2-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d8a2-125">Response</span></span>

<span data-ttu-id="4d8a2-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d8a2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d8a2-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d8a2-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d8a2-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d8a2-129">Request</span></span>
<span data-ttu-id="4d8a2-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d8a2-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="4d8a2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d8a2-131">Response</span></span>
<span data-ttu-id="4d8a2-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d8a2-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4d8a2-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4d8a2-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4d8a2-134">C#</span><span class="sxs-lookup"><span data-stu-id="4d8a2-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d8a2-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d8a2-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_conversation-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4d8a2-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4d8a2-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_conversation-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
