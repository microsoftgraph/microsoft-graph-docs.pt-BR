---
title: Remover membros da equipe
description: Remover um conversationMember de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7de64e529c86c8b8d5a185628a8d9eba6f64f6a9
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315511"
---
# <a name="remove-members-from-team"></a><span data-ttu-id="7a0e7-103">Remover membros da equipe</span><span class="sxs-lookup"><span data-stu-id="7a0e7-103">Remove members from team</span></span>
<span data-ttu-id="7a0e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a0e7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7a0e7-105">Remover um [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7a0e7-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7a0e7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a0e7-106">Permissions</span></span>
<span data-ttu-id="7a0e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a0e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a0e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a0e7-109">Permission type</span></span>|<span data-ttu-id="7a0e7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7a0e7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a0e7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a0e7-111">Delegated (work or school account)</span></span>| <span data-ttu-id="7a0e7-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a0e7-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="7a0e7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a0e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a0e7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a0e7-114">Not supported.</span></span>    |
|<span data-ttu-id="7a0e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a0e7-115">Application</span></span>| <span data-ttu-id="7a0e7-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a0e7-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a0e7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a0e7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="7a0e7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a0e7-118">Request headers</span></span>
|<span data-ttu-id="7a0e7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7a0e7-119">Name</span></span>|<span data-ttu-id="7a0e7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a0e7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7a0e7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a0e7-121">Authorization</span></span>|<span data-ttu-id="7a0e7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a0e7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a0e7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a0e7-124">Request body</span></span>
<span data-ttu-id="7a0e7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a0e7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a0e7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a0e7-126">Response</span></span>

<span data-ttu-id="7a0e7-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7a0e7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7a0e7-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a0e7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a0e7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a0e7-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a0e7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a0e7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/teams/{teamsId}/members/{membership-id}
```
# <a name="c"></a>[<span data-ttu-id="7a0e7-131">C#</span><span class="sxs-lookup"><span data-stu-id="7a0e7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a0e7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a0e7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a0e7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a0e7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a0e7-134">Java</span><span class="sxs-lookup"><span data-stu-id="7a0e7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-members-from-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="7a0e7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a0e7-135">Response</span></span>
<span data-ttu-id="7a0e7-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7a0e7-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
