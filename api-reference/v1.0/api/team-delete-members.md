---
title: Remover membros da equipe
description: Remover um conversationMember de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e98aed4edc959314473d645934e8e8bfbba1143
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273687"
---
# <a name="remove-members-from-team"></a><span data-ttu-id="df553-103">Remover membros da equipe</span><span class="sxs-lookup"><span data-stu-id="df553-103">Remove members from team</span></span>
<span data-ttu-id="df553-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df553-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df553-105">Remover um [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="df553-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df553-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df553-106">Permissions</span></span>
<span data-ttu-id="df553-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df553-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df553-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df553-109">Permission type</span></span>|<span data-ttu-id="df553-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df553-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df553-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df553-111">Delegated (work or school account)</span></span>| <span data-ttu-id="df553-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df553-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="df553-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df553-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df553-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df553-114">Not supported.</span></span>    |
|<span data-ttu-id="df553-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df553-115">Application</span></span>| <span data-ttu-id="df553-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df553-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df553-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df553-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="df553-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df553-118">Request headers</span></span>
|<span data-ttu-id="df553-119">Nome</span><span class="sxs-lookup"><span data-stu-id="df553-119">Name</span></span>|<span data-ttu-id="df553-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="df553-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="df553-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="df553-121">Authorization</span></span>|<span data-ttu-id="df553-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df553-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df553-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df553-124">Request body</span></span>
<span data-ttu-id="df553-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df553-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df553-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="df553-126">Response</span></span>

<span data-ttu-id="df553-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="df553-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="df553-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="df553-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df553-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df553-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="df553-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="df553-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/teams/{teamsId}/members/{membership-id}
```
# <a name="c"></a>[<span data-ttu-id="df553-131">C#</span><span class="sxs-lookup"><span data-stu-id="df553-131">C#</span></span>](#tab/csharp)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df553-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df553-132">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df553-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df553-133">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="df553-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="df553-134">Response</span></span>
<span data-ttu-id="df553-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="df553-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
