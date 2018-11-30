---
title: Remover rejectedSender
description: Remove um usuário ou grupo da lista rejectedSenders.
ms.openlocfilehash: f80697b2e9a02b761a1fb9959e0b18cd61a1a4c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005375"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="0a5ed-103">Remover rejectedSender</span><span class="sxs-lookup"><span data-stu-id="0a5ed-103">Remove rejectedSender</span></span>
<span data-ttu-id="0a5ed-104">Remove um usuário ou grupo da lista rejectedSenders.</span><span class="sxs-lookup"><span data-stu-id="0a5ed-104">Remove a user or group from the rejectedSenders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a5ed-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a5ed-105">Permissions</span></span>
<span data-ttu-id="0a5ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a5ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a5ed-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a5ed-108">Permission type</span></span>                        | <span data-ttu-id="0a5ed-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a5ed-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="0a5ed-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a5ed-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a5ed-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a5ed-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="0a5ed-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a5ed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a5ed-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a5ed-113">Not supported.</span></span> |
| <span data-ttu-id="0a5ed-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a5ed-114">Application</span></span>                            | <span data-ttu-id="0a5ed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a5ed-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a5ed-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a5ed-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="0a5ed-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a5ed-117">Request headers</span></span>

| <span data-ttu-id="0a5ed-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a5ed-118">Header</span></span>         | <span data-ttu-id="0a5ed-119">Valor</span><span class="sxs-lookup"><span data-stu-id="0a5ed-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="0a5ed-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a5ed-120">Authorization</span></span>  | <span data-ttu-id="0a5ed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a5ed-p102">Bearer {token}. Required.</span></span> 

## <a name="request-body"></a><span data-ttu-id="0a5ed-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a5ed-123">Request body</span></span>
<span data-ttu-id="0a5ed-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a5ed-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a5ed-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a5ed-125">Response</span></span>
<span data-ttu-id="0a5ed-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a5ed-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a5ed-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a5ed-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0a5ed-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a5ed-129">Request</span></span>
<span data-ttu-id="0a5ed-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a5ed-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="0a5ed-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a5ed-131">Response</span></span>
<span data-ttu-id="0a5ed-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0a5ed-132">The following is an example of the response.</span></span> 
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
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->