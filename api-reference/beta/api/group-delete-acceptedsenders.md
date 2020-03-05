---
title: Remover acceptedSender
description: 'Remover um usuário ou grupo da lista de remetentes aceitos. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f4b82ccaef290efa0bec00785e5f1ad3a30f516f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420574"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="0ee5b-103">Remover acceptedSender</span><span class="sxs-lookup"><span data-stu-id="0ee5b-103">Remove acceptedSender</span></span>

<span data-ttu-id="0ee5b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0ee5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ee5b-105">Remover um usuário ou grupo da lista de remetentes aceitos do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="0ee5b-105">Remove a user or group from the accepted-senders list of the specified group.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0ee5b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ee5b-106">Permissions</span></span>
<span data-ttu-id="0ee5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ee5b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ee5b-109">Permission type</span></span>                        | <span data-ttu-id="0ee5b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ee5b-110">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="0ee5b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ee5b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ee5b-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee5b-112">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="0ee5b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ee5b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ee5b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ee5b-114">Not supported.</span></span>|
| <span data-ttu-id="0ee5b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ee5b-115">Application</span></span>                            | <span data-ttu-id="0ee5b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ee5b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ee5b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ee5b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="0ee5b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee5b-118">Request headers</span></span>
| <span data-ttu-id="0ee5b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ee5b-119">Header</span></span>         | <span data-ttu-id="0ee5b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0ee5b-120">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="0ee5b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ee5b-121">Authorization</span></span>  | <span data-ttu-id="0ee5b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ee5b-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="0ee5b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee5b-124">Request body</span></span>
<span data-ttu-id="0ee5b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ee5b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ee5b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ee5b-126">Response</span></span>
<span data-ttu-id="0ee5b-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ee5b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ee5b-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0ee5b-129">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="0ee5b-130">Exemplo 1: remover um usuário da lista de remetentes aceitos do grupo.</span><span class="sxs-lookup"><span data-stu-id="0ee5b-130">Example 1: Remove a user from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="0ee5b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee5b-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="0ee5b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ee5b-132">Response</span></span>
<span data-ttu-id="0ee5b-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ee5b-133">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="0ee5b-134">Exemplo 2: remover um grupo da lista de remetentes aceitos do grupo.</span><span class="sxs-lookup"><span data-stu-id="0ee5b-134">Example 2: Remove a group from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="0ee5b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ee5b-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="0ee5b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ee5b-136">Response</span></span>
<span data-ttu-id="0ee5b-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ee5b-137">The following is an example of the response.</span></span> 

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
