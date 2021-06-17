---
title: Remover membro do bate-papo
description: Remover um conversationMember de um bate-papo.
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 77325f4da4033cbb5d5565be9a116dca0d9546ee
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971353"
---
# <a name="remove-member-from-chat"></a><span data-ttu-id="f2c5d-103">Remover membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="f2c5d-103">Remove member from chat</span></span>
<span data-ttu-id="f2c5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2c5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2c5d-105">Remover um [conversationMember](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="f2c5d-105">Remove a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2c5d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2c5d-106">Permissions</span></span>
<span data-ttu-id="f2c5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2c5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2c5d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2c5d-109">Permission type</span></span>|<span data-ttu-id="f2c5d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2c5d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2c5d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2c5d-111">Delegated (work or school account)</span></span>| <span data-ttu-id="f2c5d-112">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2c5d-112">ChatMember.ReadWrite.All</span></span> |
|<span data-ttu-id="f2c5d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2c5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2c5d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-114">Not supported.</span></span>    |
|<span data-ttu-id="f2c5d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2c5d-115">Application</span></span>| <span data-ttu-id="f2c5d-116">Chat.Manage.Chat\*, ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2c5d-116">Chat.Manage.Chat\*, ChatMember.ReadWrite.All</span></span> |

> <span data-ttu-id="f2c5d-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="f2c5d-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="f2c5d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2c5d-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /chats/{chat-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="f2c5d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c5d-119">Request headers</span></span>
|<span data-ttu-id="f2c5d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f2c5d-120">Name</span></span>|<span data-ttu-id="f2c5d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2c5d-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2c5d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2c5d-122">Authorization</span></span>|<span data-ttu-id="f2c5d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2c5d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c5d-125">Request body</span></span>
<span data-ttu-id="f2c5d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2c5d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2c5d-127">Response</span></span>

<span data-ttu-id="f2c5d-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f2c5d-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f2c5d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2c5d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2c5d-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f2c5d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2c5d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_chat"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```
# <a name="c"></a>[<span data-ttu-id="f2c5d-132">C#</span><span class="sxs-lookup"><span data-stu-id="f2c5d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2c5d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2c5d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2c5d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2c5d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2c5d-135">Java</span><span class="sxs-lookup"><span data-stu-id="f2c5d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-members-from-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2c5d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2c5d-136">Response</span></span>
<span data-ttu-id="f2c5d-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f2c5d-137">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="f2c5d-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="f2c5d-138">See also</span></span>

- [<span data-ttu-id="f2c5d-139">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="f2c5d-139">Remove member from channel</span></span>](channel-delete-members.md)
- [<span data-ttu-id="f2c5d-140">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="f2c5d-140">Remove member from team</span></span>](team-delete-members.md)

