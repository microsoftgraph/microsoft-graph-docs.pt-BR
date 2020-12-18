---
title: Remover membro do bate-papo
description: Remover um conversationMember de um bate-papo.
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f1ed1c4b461bebf3bcef1e5e3a4149a043dad30e
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714351"
---
# <a name="remove-member-from-chat"></a><span data-ttu-id="3067d-103">Remover membro do bate-papo</span><span class="sxs-lookup"><span data-stu-id="3067d-103">Remove member from chat</span></span>
<span data-ttu-id="3067d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3067d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3067d-105">Remover um [conversationMember](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="3067d-105">Remove a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3067d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3067d-106">Permissions</span></span>
<span data-ttu-id="3067d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3067d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3067d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3067d-109">Permission type</span></span>|<span data-ttu-id="3067d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3067d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3067d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3067d-111">Delegated (work or school account)</span></span>| <span data-ttu-id="3067d-112">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3067d-112">ChatMember.ReadWrite.All</span></span> |
|<span data-ttu-id="3067d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3067d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3067d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3067d-114">Not supported.</span></span>    |
|<span data-ttu-id="3067d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3067d-115">Application</span></span>| <span data-ttu-id="3067d-116">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3067d-116">ChatMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3067d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3067d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /chats/{chat-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="3067d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3067d-118">Request headers</span></span>
|<span data-ttu-id="3067d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3067d-119">Name</span></span>|<span data-ttu-id="3067d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3067d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3067d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3067d-121">Authorization</span></span>|<span data-ttu-id="3067d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3067d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3067d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3067d-124">Request body</span></span>
<span data-ttu-id="3067d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3067d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3067d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3067d-126">Response</span></span>

<span data-ttu-id="3067d-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3067d-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3067d-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3067d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3067d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3067d-129">Request</span></span>

> [!NOTE]
> <span data-ttu-id="3067d-130">Há alguns problemas conhecidos com essa funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="3067d-130">There are some known issues with this functionality.</span></span> <span data-ttu-id="3067d-131">Para saber mais, confira [problemas conhecidos](/graph/known-issues.md#unable-to-remove-members-from-chat).</span><span class="sxs-lookup"><span data-stu-id="3067d-131">For details, see [known issues](/graph/known-issues.md#unable-to-remove-members-from-chat).</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_members_from_chat"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="response"></a><span data-ttu-id="3067d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3067d-132">Response</span></span>
<span data-ttu-id="3067d-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3067d-133">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="3067d-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="3067d-134">See also</span></span>

- [<span data-ttu-id="3067d-135">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="3067d-135">Remove member from channel</span></span>](channel-delete-members.md)
- [<span data-ttu-id="3067d-136">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="3067d-136">Remove member from team</span></span>](team-delete-members.md)

