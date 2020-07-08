---
title: Remover membros da equipe
description: Remover um conversationMember de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 03293bea7f74017985cb362e2e4c2fbd8c084dff
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081130"
---
# <a name="delete-members"></a><span data-ttu-id="da6bd-103">Excluir Membros</span><span class="sxs-lookup"><span data-stu-id="da6bd-103">Delete members</span></span>
<span data-ttu-id="da6bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da6bd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da6bd-105">Remover um novo [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="da6bd-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="da6bd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="da6bd-106">Permissions</span></span>
<span data-ttu-id="da6bd-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="da6bd-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="da6bd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da6bd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da6bd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da6bd-109">Permission type</span></span>|<span data-ttu-id="da6bd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da6bd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da6bd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da6bd-111">Delegated (work or school account)</span></span>| <span data-ttu-id="da6bd-112">TeamMember. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="da6bd-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="da6bd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da6bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da6bd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da6bd-114">Not supported.</span></span>    |
|<span data-ttu-id="da6bd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da6bd-115">Application</span></span>| <span data-ttu-id="da6bd-116">TeamMember. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="da6bd-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da6bd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da6bd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{teamsId}/members
```

## <a name="request-headers"></a><span data-ttu-id="da6bd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da6bd-118">Request headers</span></span>
|<span data-ttu-id="da6bd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="da6bd-119">Name</span></span>|<span data-ttu-id="da6bd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="da6bd-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="da6bd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="da6bd-121">Authorization</span></span>|<span data-ttu-id="da6bd-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="da6bd-122">Bearer {token}.</span></span> <span data-ttu-id="da6bd-123">Required.</span><span class="sxs-lookup"><span data-stu-id="da6bd-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da6bd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da6bd-124">Request body</span></span>
<span data-ttu-id="da6bd-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da6bd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da6bd-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="da6bd-126">Response</span></span>

<span data-ttu-id="da6bd-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="da6bd-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="da6bd-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="da6bd-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da6bd-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da6bd-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="da6bd-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="da6bd-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="da6bd-131">C#</span><span class="sxs-lookup"><span data-stu-id="da6bd-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da6bd-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da6bd-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da6bd-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da6bd-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="da6bd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="da6bd-134">Response</span></span>
<span data-ttu-id="da6bd-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="da6bd-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

