---
title: Remover membros da equipe
description: Remover um conversationMember de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d76456123f3d60428feb213b0ef8901b03db3fa1
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124132"
---
# <a name="delete-members"></a><span data-ttu-id="5ace9-103">Excluir membros</span><span class="sxs-lookup"><span data-stu-id="5ace9-103">Delete members</span></span>
<span data-ttu-id="5ace9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ace9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ace9-105">Remover um [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="5ace9-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5ace9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ace9-106">Permissions</span></span>
<span data-ttu-id="5ace9-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5ace9-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5ace9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ace9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ace9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ace9-109">Permission type</span></span>|<span data-ttu-id="5ace9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ace9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ace9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ace9-111">Delegated (work or school account)</span></span>| <span data-ttu-id="5ace9-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ace9-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="5ace9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ace9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ace9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ace9-114">Not supported.</span></span>    |
|<span data-ttu-id="5ace9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ace9-115">Application</span></span>| <span data-ttu-id="5ace9-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ace9-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ace9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ace9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{member-id}
```

## <a name="request-headers"></a><span data-ttu-id="5ace9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ace9-118">Request headers</span></span>
|<span data-ttu-id="5ace9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5ace9-119">Name</span></span>|<span data-ttu-id="5ace9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ace9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5ace9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ace9-121">Authorization</span></span>|<span data-ttu-id="5ace9-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5ace9-122">Bearer {token}.</span></span> <span data-ttu-id="5ace9-123">Required.</span><span class="sxs-lookup"><span data-stu-id="5ace9-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ace9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ace9-124">Request body</span></span>
<span data-ttu-id="5ace9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ace9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ace9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ace9-126">Response</span></span>

<span data-ttu-id="5ace9-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5ace9-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5ace9-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5ace9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ace9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ace9-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5ace9-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ace9-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="5ace9-131">C#</span><span class="sxs-lookup"><span data-stu-id="5ace9-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ace9-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ace9-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ace9-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ace9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5ace9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ace9-134">Response</span></span>
<span data-ttu-id="5ace9-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ace9-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

