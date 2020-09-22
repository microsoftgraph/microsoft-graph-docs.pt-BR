---
title: Excluir conversa
description: Exclua uma conversa.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 36de1d9d40ac2ac4eabd1a5e8f2ee9450c257762
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002815"
---
# <a name="delete-conversation"></a><span data-ttu-id="95170-103">Excluir conversa</span><span class="sxs-lookup"><span data-stu-id="95170-103">Delete conversation</span></span>

<span data-ttu-id="95170-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95170-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95170-105">Exclua uma conversa.</span><span class="sxs-lookup"><span data-stu-id="95170-105">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="95170-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="95170-106">Permissions</span></span>
<span data-ttu-id="95170-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95170-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95170-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95170-109">Permission type</span></span>      | <span data-ttu-id="95170-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95170-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95170-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95170-111">Delegated (work or school account)</span></span> | <span data-ttu-id="95170-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95170-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="95170-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95170-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95170-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95170-114">Not supported.</span></span>    |
|<span data-ttu-id="95170-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95170-115">Application</span></span> | <span data-ttu-id="95170-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95170-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95170-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95170-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="95170-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95170-118">Request headers</span></span>
| <span data-ttu-id="95170-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95170-119">Header</span></span>       | <span data-ttu-id="95170-120">Valor</span><span class="sxs-lookup"><span data-stu-id="95170-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="95170-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="95170-121">Authorization</span></span>  | <span data-ttu-id="95170-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95170-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="95170-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95170-124">Request body</span></span>
<span data-ttu-id="95170-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95170-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95170-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="95170-126">Response</span></span>

<span data-ttu-id="95170-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95170-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95170-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95170-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95170-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95170-130">Request</span></span>
<span data-ttu-id="95170-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95170-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="95170-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="95170-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
# <a name="c"></a>[<span data-ttu-id="95170-133">C#</span><span class="sxs-lookup"><span data-stu-id="95170-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95170-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95170-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95170-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95170-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="95170-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="95170-136">Response</span></span>
<span data-ttu-id="95170-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95170-137">Here is an example of the response.</span></span> 
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


