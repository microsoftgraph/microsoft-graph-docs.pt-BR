---
title: Remover acceptedSender
description: 'Remover um usuário ou grupo da lista de remetentes aceitos. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 22e81f8bbbb497b8209e6faa744a54b24029391c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329733"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="a9482-103">Remover acceptedSender</span><span class="sxs-lookup"><span data-stu-id="a9482-103">Remove acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9482-104">Remover um usuário ou grupo da lista de remetentes aceitos do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="a9482-104">Remove a user or group from the accepted-senders list of the specified group.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a9482-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9482-105">Permissions</span></span>
<span data-ttu-id="a9482-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9482-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9482-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9482-108">Permission type</span></span>                        | <span data-ttu-id="a9482-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9482-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="a9482-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9482-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9482-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9482-111">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="a9482-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9482-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9482-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9482-113">Not supported.</span></span>|
| <span data-ttu-id="a9482-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9482-114">Application</span></span>                            | <span data-ttu-id="a9482-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9482-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9482-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9482-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="a9482-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9482-117">Request headers</span></span>
| <span data-ttu-id="a9482-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9482-118">Header</span></span>         | <span data-ttu-id="a9482-119">Valor</span><span class="sxs-lookup"><span data-stu-id="a9482-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="a9482-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9482-120">Authorization</span></span>  | <span data-ttu-id="a9482-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9482-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="a9482-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9482-123">Request body</span></span>
<span data-ttu-id="a9482-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9482-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9482-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9482-125">Response</span></span>
<span data-ttu-id="a9482-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9482-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9482-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a9482-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="a9482-129">Exemplo 1: remover um usuário da lista de remetentes aceitos do grupo.</span><span class="sxs-lookup"><span data-stu-id="a9482-129">Example 1: Remove a user from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="a9482-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9482-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="a9482-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9482-131">Response</span></span>
<span data-ttu-id="a9482-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9482-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="a9482-133">Exemplo 2: remover um grupo da lista de remetentes aceitos do grupo.</span><span class="sxs-lookup"><span data-stu-id="a9482-133">Example 2: Remove a group from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="a9482-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9482-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="a9482-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9482-135">Response</span></span>
<span data-ttu-id="a9482-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9482-136">The following is an example of the response.</span></span> 

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
