---
title: Remover membros da equipe
description: Remover um conversationMember de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 06993e2a05fe4597df338d8e5548ee4c2a914a73
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330150"
---
# <a name="remove-members-from-team"></a><span data-ttu-id="35309-103">Remover membros da equipe</span><span class="sxs-lookup"><span data-stu-id="35309-103">Remove members from team</span></span>
<span data-ttu-id="35309-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35309-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35309-105">Remover um [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="35309-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35309-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="35309-106">Permissions</span></span>
<span data-ttu-id="35309-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35309-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35309-109">Permission type</span></span>|<span data-ttu-id="35309-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="35309-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35309-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35309-111">Delegated (work or school account)</span></span>| <span data-ttu-id="35309-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35309-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="35309-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35309-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35309-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35309-114">Not supported.</span></span>    |
|<span data-ttu-id="35309-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35309-115">Application</span></span>| <span data-ttu-id="35309-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35309-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35309-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35309-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{membership-id}
DELETE /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="35309-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35309-118">Request headers</span></span>
|<span data-ttu-id="35309-119">Nome</span><span class="sxs-lookup"><span data-stu-id="35309-119">Name</span></span>|<span data-ttu-id="35309-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="35309-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="35309-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="35309-121">Authorization</span></span>|<span data-ttu-id="35309-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35309-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="35309-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35309-124">Request body</span></span>
<span data-ttu-id="35309-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="35309-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35309-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="35309-126">Response</span></span>

<span data-ttu-id="35309-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="35309-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="35309-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="35309-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35309-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35309-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="35309-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="35309-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/{teamsId}/members/{membership-id}
```
# <a name="c"></a>[<span data-ttu-id="35309-131">C#</span><span class="sxs-lookup"><span data-stu-id="35309-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35309-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35309-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35309-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35309-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="35309-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="35309-134">Response</span></span>
<span data-ttu-id="35309-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="35309-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



