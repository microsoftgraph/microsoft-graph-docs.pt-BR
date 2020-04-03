---
title: Remover acceptedSender
description: 'Remover um usuário ou grupo da lista de remetentes aceitos. '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2274d3f5e8dfab42b1df9d6da0510ae7d22de463
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123892"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="39872-103">Remover acceptedSender</span><span class="sxs-lookup"><span data-stu-id="39872-103">Remove acceptedSender</span></span>

<span data-ttu-id="39872-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39872-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39872-105">Remover um usuário ou grupo da lista de remetentes aceitos do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="39872-105">Remove a user or group from the accepted-senders list of the specified group.</span></span> 

## <a name="permissions"></a><span data-ttu-id="39872-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="39872-106">Permissions</span></span>
<span data-ttu-id="39872-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39872-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39872-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39872-109">Permission type</span></span>                        | <span data-ttu-id="39872-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39872-110">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="39872-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39872-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="39872-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39872-112">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="39872-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39872-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39872-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39872-114">Not supported.</span></span>|
| <span data-ttu-id="39872-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39872-115">Application</span></span>                            | <span data-ttu-id="39872-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39872-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39872-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39872-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="39872-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39872-118">Request headers</span></span>
| <span data-ttu-id="39872-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39872-119">Header</span></span>         | <span data-ttu-id="39872-120">Valor</span><span class="sxs-lookup"><span data-stu-id="39872-120">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="39872-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="39872-121">Authorization</span></span>  | <span data-ttu-id="39872-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39872-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="39872-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39872-124">Request body</span></span>
<span data-ttu-id="39872-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="39872-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39872-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="39872-126">Response</span></span>
<span data-ttu-id="39872-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39872-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39872-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="39872-129">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="39872-130">Exemplo 1: remover um usuário da lista de remetentes aceitos do grupo.</span><span class="sxs-lookup"><span data-stu-id="39872-130">Example 1: Remove a user from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="39872-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39872-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="39872-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="39872-132">Response</span></span>
<span data-ttu-id="39872-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="39872-133">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="39872-134">Exemplo 2: remover um grupo da lista de remetentes aceitos do grupo.</span><span class="sxs-lookup"><span data-stu-id="39872-134">Example 2: Remove a group from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="39872-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39872-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="39872-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="39872-136">Response</span></span>
<span data-ttu-id="39872-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="39872-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_group_from_acceptedsenderslist_of_group",
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
  "description": "Remove acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
